# ssl-prova

# SSL e Certificados Digitais

**Aluno:** Clovis Campanha Junior  
**Disciplina:** Segurança de Sistemas Computacionais  
**Professor:** Clerivaldo  
**Instituição:** Escola de Engenharia de Piracicaba (EEP)  

---

## Ambiente

| Item | Detalhe |
| --- | --- |
| **Sistema Operacional** | Debian Linux  |
| **IP utilizado** | 127.0.0.1 (localhost) |
| **OpenSSL** | Já incluso no sistema |

---

## Estrutura do Repositório

```text
ssl-prova/
├── exercicio1/   # Preparação do ambiente — instalação e verificação do OpenSSL
├── exercicio2/   # Estrutura de diretórios SSL
├── exercicio3/   # Geração da chave privada RSA 2048 bits
├── exercicio4/   # Criação do CSR com dados do aluno
├── exercicio5/   # Certificado auto-assinado X.509 (365 dias)
├── exercicio6/   # Transferência do certificado via SCP
├── exercicio7/   # Servidor HTTPS com Python + SSL
├── exercicio8/   # Validação do certificado no navegador
└── README.md
```

---

## Dificuldades Encontradas

1. **Permissões da chave privada:** O arquivo `clovis.key` em `/etc/ssl/certificates/` tinha permissões restritas (root). Foi necessário dar a permissão ao usuario para manipular o diretório.

2. **`http.server` sem HTTPS nativo:** O módulo Python `http.server` não suporta SSL nativamente. Foi necessário criar um script para configurar o servidor como HTTPS.

3. Entender conceitos que ainda não foram adiquiridos (redes e python)

---

## Conclusão

A atividade ajudou a melhorar o aprendizado sobre criação e utilização de certificados SSL/TLS
Atraves da atividade houve oportunidade de revisar conceitos ja adquiridos como alteração de permissão em pastas e arquivos bem como comandos comuns do ambiente.
Com essa atividade pude aprender conceitos novos que ainda não possuia a respeito de python e criação de servidores

Atrave dessa atividade consegui entender melhor sobre o funcionamento de certificados e as principais diferenças entre CAs e certificados autoassinados.
