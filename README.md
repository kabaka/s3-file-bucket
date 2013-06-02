# S3 File Bucket

Upload files to S3 under a given prefix with a preconfigured expiration. Files
are *currently* named by the current epoch in base 36, so uploading many files
in a short time will result in files being skipped. I'll change that, soon.

Just a note: this is obscenely simple and barely deserves its own repository.

I got tired of all the bogus issues with quick image hosts for screen shots and
other files I needed to share quickly and temporarily, so I wrote this based on
my tiny Rake-based S3 web site creator.

## Usage

Run `s3up` with one or more files as arguments.

### Configuration

See `config.yaml.dist`. Create a `config.yaml` based on it.

