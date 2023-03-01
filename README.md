1. `bash env` then execute displayed export command
2. `helmfile apply -i`
3. Notice how `cert-unencrypted` displays a diff of N bytes for tls.key
4. Notice how `cert-encrypted` encrypted displays a diff of 0 bytes for tls.key
6. Confirm apply to show error message 
5. `helm secret decrypt manifests/certs-encrypted.yaml` shows the same tls.key field as `manifests/certs-unencrypted.yaml`
