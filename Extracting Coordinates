# GeoSurvey
Extracting Coordinates from GeoSurvey
 # Malawi GeoSurvey 1000 Sample Set Up
 # W. Simbila February 2018

 # Setting directory -------------------------------
 setwd("~")
 dir.create("MW_GS_data", showWarnings = F)
 setwd("./MW_GS_data")
    
 # Loading data -----------------------------------------
 xy <- read.csv("MW_geos_2018.csv", header = T, sep = "," )
    
 # Extracting------------------------------------------------
 left = function(text, num_char) {
      substr(text, 1, num_char)
    }
 mid = function(text, start_num, num_char) {
      substr(text, start_num, start_num + num_char - 1)
    }
 right = function(text, num_char) {
      substr(text, nchar(text) - (num_char-1), nchar(text))
    }
    
 # Write output file--------------------------------------------
 dir.create("Results", showWarnings = F)
 write.csv(xy, "./Results/MW_gsdat.csv", row.names = F)
    
