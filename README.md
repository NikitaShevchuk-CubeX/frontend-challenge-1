### Setup

# Frontend

```
npm install
npm run dev
```

# Backend

```
npm install
npm run dev

```

### Application flow

# Frontend

Routes:

/ - home page
/upload - a page to upload your file
/uploaded-files = a page to see all uploaded files

State:

UploadedFilesData state contains information about uploaded files along with the request status & a function to load uploaded files to the state

Components:

Layout - main application layout
upload/Page - the main page for uploads functionality
uploade/UploadResults - shows the result of file upload (success or error)
uploade/UploadedFilePreview - displays a preview of the uploaded file in a convenient table
uploaded-files/Page - displays a list of previously uploaded files

Interaction with API:

The main service for API interaction is UploadsService since it's the only app's functionality

# Backend

Endpoints:

/mrf/upload - accepts, parses, validates, and saves an uploaded file
/mrf/list - returns a list of previously uploaded files
