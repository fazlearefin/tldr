# ssh-keygen

> Gera chaves SSH usadas para autenticação, logins sem senha e outras finalidades.
> Mais informações: <https://man.openbsd.org/ssh-keygen>.

- Gera uma chave interativamente:

`ssh-keygen`

- Gera uma chave ed25519 com 32 rounds de função de derivação de chave e salva a chave em um arquivo específico:

`ssh-keygen -t {{ed25519}} -a {{32}} -f {{~/.ssh/nome_do_arquivo}}`

- Gera uma chave RSA de 4096 bits com um comentário de email:

`ssh-keygen -t {{rsa}} -b {{4096}} -C "{{comentário|email}}"`

- Remove as chaves de um servidor do arquivo known_hosts (útil quando um servidor conhecido tem uma nova chave):

`ssh-keygen -R {{servidor_remoto}}`

- Obtém a impressão digital de uma chave em MD5 Hex:

`ssh-keygen -l -E {{md5}} -f {{~/.ssh/nome_do_arquivo}}`

- Altera a senha de uma chave:

`ssh-keygen -p -f {{~/.ssh/nome_do_arquivo}}`

- Altera o tipo de formato da chave (por exemplo, de formato OPENSSH para PEM), o arquivo será reescrito no local:

`ssh-keygen -p -N "" -m {{PEM}} -f {{~/.ssh/chave_privada_OpenSSH}}`

- Obtém a chave pública a partir da chave secreta:

`ssh-keygen -y -f {{~/.ssh/chave_privada_OpenSSH}}`
