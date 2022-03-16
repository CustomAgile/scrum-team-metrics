#Feature Burnup
Cumulative view of the total features and delivered features for each day during the selected release period.   

The data set for the burnup contains all features associated with the selected release at some point between the release start date and the release end date for the current workspace's default timezone. 

A delivered feature is one that is in State = "Operate" or State = "Done"

###Notes
This app relies on the assumption that the lowest level Portfolio Item is a "Feature".  
It also relies on the existence of certain feature and story custom fields as well as the Feature State of Done.  

The dataset used for the calculations in this app is all features in the current project scope that were associated with the selected release at the time of the release start date (which is midnight on the ReleaseStartDate in the default timezone of the workspace).

Planned and Total will be the same for a release with a start date in the future since it will return the features currently associated with the release (if it is before the release start date).