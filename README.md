Resume Book
==========
Literally completely recycled code. Midterms = laziness. 

Heroku
---

Access the app here: http://eecs-resume-book.herokuapp.com/

We still need S3 credentials, and its being hosted by me (Sidd) on my Heroku account, but let me know if H@B has its own Heroku, so I can transfer it over.

Usage
---

1. Clone the repository or download and extract the files.
2. Install Node.js if you haven't already.
3. Go to the directory where index.js etc. are.
4. Edit config.js if you wish to change the upload directory or the port number.
5. Run the application using `node index.js`
6. Go to `http://<IP_ADDRESS>:<PORT>` where `<IP_ADDRESS>` is the IP address of the machine where the application is running and the `<PORT>` is the port number defined in `config.js` which is `8000` by default.
7. Drag and drop files to the marked area to upload the files to the `upload_dir` defined in `config.js`.

**To use with AWS S3:**

1. Install knox using `npm install knox`.
2. Edit config.js to fill in the values for the keys `key`, `secret` and `bucket`, and replace the last line with `exports.s3_enabled = true;`.

License
---

This application is released under the MIT License. See the `LICENSE` file for details.