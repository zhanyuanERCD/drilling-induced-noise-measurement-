                                            Resort the Raw Measurement Files of Labview
after measurement, we can get 1 raw calibration and 4 raw accleration labview files:  calibration.tdms; implant_bed_data_accel.tdms; Mastoiddectomy_data_accel.tdms; posteriore_tymp._data_accel.tdms;implant_bed_data_accel.tdms     put them into the folder: R:\Labor_ERCD\projekte\bohrlaerm\Experimente_studien\2021_ci_studie\00_measurement_data_op\Temporary Data for Instant Demostration\

open originlab software, alt+4, open the code builder panel, import all .ogs files.

run 2calibration.org(measurements after 19.07.2022)/1calibration.org(measurements before 19.07.2022) we can get the optimized FRFcurve in the new calibration.tdms(same teporal folder).  Defautly extract coherence>=0.3.

open the labview file correct_accel.vi(R:\Labor_ERCD\projekte\bohrlaerm\Programme_Simulationen\labview\cochleostomy_correction2),  input 1 in the 'linear part' box; in the 'calib file path' input the new calibration file; in "file path" box, choose a new input and output path, meanwhile, open the Block diagram, revise the new output name,e.g.implant_bed_data_level;  for cochleostomy, open the correction button, add correction coeffience.  Finally, we can get the 4 new Sound Pressure Level-time-Burr files:implant_bed_data_level.tdms    Mastoiddectomy_data_level.tdms  posteriore_tymp._data_level.tdms  Cochleostomy_data_level.tdms  insure they are all in the folder: R:\Labor_ERCD\projekte\bohrlaerm\Experimente_studien\2021_ci_studie\00_measurement_data_op\Temporary Data for Instant Demostration\

                                             Single  Measurement Calculation by Originlab 
release the template files of Anwenderdateien.zip into oringinlab folder in system e.g. C:\Users\zhanyuan\Documents\OriginLab\Anwenderdateien\
in the code builder panel of originlab, run singleOP.ogs files,  we can present the measurement results and plots.
the sigle measurement summary file is autosaved into summary folder(R:\Labor_ERCD\projekte\bohrlaerm\Experimente_studien\2021_ci_studie\00_measurement_data_op\Temporary Data for Instant Demostration\summary\XX.opju)

                                              Summary of all measurements
run 'input measurements into files.ogs'   iuput all sigle measurements summary into orginlab
run the each section of 'statistics.ogs' get each statistics that we want, you can edit or add the section regarding to the amounts you want to analysis.
