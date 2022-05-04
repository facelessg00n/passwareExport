## Passware Ripper

---

Rips passwords and attributes from recovered password reports output from Passware

This project was created to to assist in password sharing and ingestion of passwords into other tools.

Proposed password Sharing model

```json

{
    "passCategory": Category of job password involved in,

    "passwordObject":{
        "fileHash":"MD5 hash of the file of interest",
        "fileName":"Name of the file of interest",
        "fileExtension":"File extension for the file of interest",
        "encryptionType":"Encryption type used",
        "password":"Plaintext password for the file"
    },
    objectDetails:{
        "dateCracked":"date the password was cracked", 
    }
    uploadDetails:{
        "uploadComments":" Comments attached to the upload for validation purposes"
    },
 }
 
```

----

Log

**5/5/22**

Regex used to parse data from HTML file as JSON data is in a HTML comments section at the end of the file.

**28/4/2022**

Initial proof of concept to parse data
