# JSON Dictionary
In order to upload a dataset to data.buspark.io, you need to create a JSON file that contains metadata about the dataset. These five fields are required to upload a new dataset.

`project_name`: This is the name of the dataset or project. It's important that this name is unique and descriptive enough so that users can easily understand what data the project contains just by looking at the name. In CKAN, it's often used as the identifier for the dataset and is included in the dataset's URL.

`description`: This field provides a summary of what the dataset is about. It usually includes information about what kind of data the dataset contains, how the data was collected, and what the data can be used for. It can also include information about the structure of the data, such as what each column in a table represents.

`more_information`: This field contains a URL for more information about the dataset. In most cases, it links to the project's GitHub repository. This is where users can find more detailed information about the project, potentially including the methodology, raw code, and additional documentation used during the project.

`uris`: This field contains a list of paths to the folder(s) that contains the resources associated with the dataset. Remember, resources in CKAN usually represent individual data files. For example, if your dataset includes data from multiple years, you might have one CSV file for each year, compile each CSV into one folder and use that folder's name for this field.

`owner_org`: This field represents the organization that owns the dataset. In CKAN, datasets can be organized by organizations to make it easier for users to find datasets that are relevant to them. For example, "buspark" could be used for this field.

Example:
```
{
	"project_name": "police_arrests_summer2021",
	"description": "Collecting a record of adult/juvenile arrests, offenses reported, offenses cleared, classification, and year associated with offenses ",
	"more_information" : "https://github.com/BU-Spark/summer2021internship/tree/master/Police%20Arrest%20Analysis",
	"uris": "PoliceArrestsS21",
	"owner_org": "buspark"
}
```
