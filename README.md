# Analysis-pipeline-ROI-
Analysis-pipeline from AB for ROI placement. 

CHANGE DIRECTORY - line # 7 

clear; clc; close all;
mainDir = '/Volumes/T5-Alex/OneDrive - Perspectum Ltd/biobank-t2dm-pipe-results/dataset_t2dm_matx_subjects_forTW_AB/';
matList = dir([mainDir filesep '*.mat']);
for ii=1:numel(matList)
    placeROIs([matList(ii).folder filesep matList(ii).name])
end
disp('Done')
