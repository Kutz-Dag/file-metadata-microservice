# File Metadata Microservice

### Description

You can submit a form that includes a file upload. You will receive the file name and size in bytes within the JSON response when you submit something. The results will be similar to the image below:

### Project Preview:

![time-stamp microservice](https://github.com/user-attachments/assets/7db61e4e-f40e-46f2-b353-7873b93da480)

### User Stories/Tests to pass:

- [x] You should provide your own project, not the example URL.
- [x] A request to /api/:date? with a valid date should return a JSON object with a unix key that is a Unix timestamp of the input date in milliseconds (as type Number)
- [x] A request to /api/:date? with a valid date should return a JSON object with a utc key that is a string of the input date in the format: Thu, 01 Jan 1970 00:00:00 GMT
- [x] A request to /api/1451001600000 should return { unix: 1451001600000, utc: "Fri, 25 Dec 2015 00:00:00 GMT" }
- [x] Your project can handle dates that can be successfully parsed by new Date(date_string)
- [x] If the input date string is invalid, the API returns an object having the structure { error : "Invalid Date" }
- [x] An empty date parameter should return the current time in a JSON object with a unix key
- [x] An empty date parameter should return the current time in a JSON object with a utc key
