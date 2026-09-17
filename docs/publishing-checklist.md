# Checklist antes de publicar um workflow n8n

## Credenciais

- [ ] Remover API keys, tokens, senhas e client secrets.
- [ ] Rotacionar qualquer segredo que já tenha sido exportado.
- [ ] Remover headers de autenticação escritos manualmente.
- [ ] Confirmar que apenas referências genéricas de credenciais permanecem.

## Identificadores e infraestrutura

- [ ] Remover tenant, workspace e dataset IDs.
- [ ] Remover URLs internas, IPs, domínios e caminhos privados.
- [ ] Remover números de telefone, e-mails e identificadores de usuários.
- [ ] Remover nomes reais de clientes, empresas, filiais e fornecedores.

## Propriedade intelectual

- [ ] Substituir prompts completos por descrições.
- [ ] Remover regras de negócio e roteamento.
- [ ] Remover bibliotecas DAX e SQL proprietárias.
- [ ] Substituir subworkflows privados por nós explicativos.
- [ ] Usar apenas exemplos e dados fictícios.

## Validação final

Pesquise no conteúdo antes do commit:

```text
apiKey
token
authorization
Bearer
password
secret
client_secret
webhook
http://
https://
tenant
workspace
dataset
phone
email
```

Depois, revise o diff completo e confirme que nenhum arquivo de produção entrou
no commit.
