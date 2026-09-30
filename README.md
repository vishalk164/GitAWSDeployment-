# GitAWSDeployment-

## EC2 deployment

The `Deploy to EC2` workflow requires these repository Actions secrets:

- `EC2_SSH_KEY_B64`: the EC2 SSH private key encoded as base64
- `EC2_USERNAME`: the SSH login user
- `EC2_HOST`: the EC2 host name or IP address

For example, encode the private key locally with `base64 -w 0 < path/to/key`
and save the output as `EC2_SSH_KEY_B64`. Do not commit the private key or its
encoded value to the repository.