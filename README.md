# S3 File Bucket

Upload files to S3 under a given prefix with a preconfigured expiration. Files
are given a pseudorandom base 64 name. Before upload, a name is generated and
checked for existence. If it exists, it will try again. Presently, names are 6
characters long, so collisions are unlikely and will be very infrequent.

Just a note: this is obscenely simple and barely deserves its own repository.

I got tired of all the bogus issues with quick image hosts for screen shots and
other files I needed to share quickly and temporarily, so I wrote this based on
my tiny Rake-based S3 web site creator.

## Usage

Run `s3up` with one or more files as arguments.

### Configuration

See `config.yaml.dist`. Create a `config.yaml` based on it.

