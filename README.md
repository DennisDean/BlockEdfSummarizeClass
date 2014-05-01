BlockEdfSummarizeClass
======================

Summarize EDFs stored in a folder
  
  
Function takes a list of EDF/XML files created by the function GetMatchedSleepEdfXmlFiles and summarises the content into a single Excel file.

### Assumptions:

The search function assumes the following naming the convention:

     EDF: 'SubjectNamingConvention'.EDF
     XML: 'SubjectNamingConvention'.EDF.xml

The search is not case sensitive and 'EDF' can not be a substring of 'SubjectNamingConvention'.

### Function Prototype:

    besObj = BlockEdfSummarizeClass(xlsFileList, xlsFileSummaryOut);

### Public Methods:

     besObj = besObj.summarizeHeader;
     besObj = besObj.summarizeSignalLabels;
     besObj = besObj.summarizeSignalLabels(requiredSignals);
     besObj = besObj.summarizeHeaderWithCheck;

     requiredSignals:  Cell array of EDF signal labels {'EEG', 'ECG'}

#### Dependencies:

[BlockEdfLoadClass.m (54227)](http://www.mathworks.com/matlabcentral/fileexchange/45227-blockedfloadclass)
[GetMatchedSleepEdfXmlFiles.m](https://github.com/DennisDean/GetMatchedSleepEdfXmlFiles)
[dirr.m (8682)](http://www.mathworks.com/matlabcentral/fileexchange/8682-dirr--find-files-recursively-filtering-name--date-or-bytes-)


### Additional Information:

    https://github.com/DennisDean?tab=repositories
    https://sleepdata.org/
    http://sleep.partners.org/edf/
        
