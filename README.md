# FileUploadWebAppUsingJavaAndAzure
This project is done as an exercice following the preparation for Azure Data Engineer Certification(DP 203)<br>

This project implements a service for interacting with Azure Blob Storage. The service provides methods for listing the names of blobs in a container, saving a blob to the container, and reading a blob from the container. It uses the Azure Storage Java SDK to perform these operations.

To use this service, you need to provide a valid Azure Storage connection string and the name of the container in which you want to store the blobs. These values can be set using the STORAGE_CONNECTION_STRING and STORAGE_CONTAINER_NAME environment variables, respectively. The service will automatically create the container if it doesn't already exist.

The listNames method returns a list of the names of all blobs in the container. The save method takes a name, an InputStream containing the data to be saved, and the length of the data in bytes, and saves it to the container with the specified name. The read method takes a name and returns an InputStream that can be used to read the data of the blob with that name from the container.
