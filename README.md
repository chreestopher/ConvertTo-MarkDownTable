    $proc = get-process 
    
    $proc | select Name, Handles, Npm -First 3| convertto-markdownTable -includeOpen -allColumnsAllignment Left
    
    $proc | select Name, Handles, Npm -First 3| convertto-markdownTable -allColumnsAllignment Center
    
    $proc | select Name, Handles, Npm -First 3 | convertto-markdownTable -includeOpen -columnAlignment @{Handles="Right"} 
    
    $proc | select Name, Handles, Npm -First 3 | convertto-markdownTable -columnAlignment @{NPM="Center"}   



|Name                |Handles             |NPM                 |
|:------------------ |:------------------ |:------------------ |
|aaHMSvc             |147                 |13576               |
|AdaptiveSleepService|118                 |7824                |
|AiChargerPlus       |143                 |10112               |

Name                |Handles             |NPM                 |
:------------------:|:------------------:|:------------------:|
aaHMSvc             |147                 |13576               |
AdaptiveSleepService|118                 |7824                |
AiChargerPlus       |143                 |10112               |

|Name                |Handles             |NPM                 |
| ------------------ | ------------------:| ------------------ |
|aaHMSvc             |147                 |13576               |
|AdaptiveSleepService|118                 |7824                |
|AiChargerPlus       |143                 |10112               |

Name                |Handles             |NPM                 |
------------------ | ------------------ |:------------------:|
aaHMSvc             |147                 |13576               |
AdaptiveSleepService|118                 |7824                |
AiChargerPlus       |143                 |10112               |    
