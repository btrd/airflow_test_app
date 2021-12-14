# Env variables

See .env.example

To generate a fernet key you can run this command `dd if=/dev/urandom bs=32 count=1 2>/dev/null | openssl base64`

# Setup database

`airflow db init`

# Create first user

`airflow users create -e email@example.com -r Admin -p temporary-password -u username --firstname Name --lastname Name`

Don't forget to change your password to something secure on the interface.
