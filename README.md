# license-gen

license-gen helps you generate, verify and enforce gitlab licenses. It is used in GitLab Enterprise Edition.

## Installation

Clone this project and then execute:

    $ bundle

## Usage

1. Prepare ruby env.

1. Then execute:

    ```shell
    ruby license_gen.rb
    ```

1. Follow the prompts to enter essential user info.

1. After the above steps, three license related files will be generated in current workspace folder:
    1. `license_key`: private key to encrypt the license
    1. `license_key.pub`: file contains public key to ship along with the main application
    1. `#{company}.gitlab-license`: the license file to send to a gitlab customer

1. Replace `/opt/gitlab/embedded/service/gitlab-rails/.license_encryption_key.pub` with generated public key.
 
## Learn more

1. [File: README — Documentation for gitlab-license](https://www.rubydoc.info/gems/gitlab-license).
