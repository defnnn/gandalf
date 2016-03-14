# Generate gandalf's key

    gandalf key gandalf@middle.earth

Don't run `gandalf key` twice as it wil create two keys wth the same email
address.

# Create a new secrets with gandalf's key

Secrets are referenced in `config/gandalf.yml`.  The moria secrets is already
defined as an example and uses gandalf's key.

    gandalf secrets moria

# View the secrets

The secrets should be encrypted with gandalf's key and unlocked with his
passphrase.

    gandalf show moria

# Edit the secrets

Will decrypt the secrets into a temporary file and edit with $EDITOR

    gandalf edit moria
