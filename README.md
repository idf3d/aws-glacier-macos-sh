# aws-glacier-macos-sh

## upload.sh

This is macOS version of [https://damienradtke.com/post/glacier-backup-bash/
]()

Differences:

* Added archive description and vault name parameters
* macOS commands (slightly different from linux)
* Prints out some more information on start

## Usage

You need to have installed and configured AWS CLI on your mac, and then just run:

`./upload.sh <file> <description> <vault name>`

## Features

* Multipart upload for large files
* Clean-up (removes temp directory and cancels upload) if failed
* Retry on timeout
* Tree-checksum computation to finalize upload

## License

WTFPL, as original script

## Contribution

Please feel free to submit Pull Requests
