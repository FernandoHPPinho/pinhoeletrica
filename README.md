# Pinho Soluções em Eletricidade

Site de uma página: [pinhoeletrica.com.br](https://pinhoeletrica.com.br)

O domínio `pinhoeletrica.com` só redireciona para o `.com.br`.

## DNS na Hostinger

### 1. pinhoeletrica.com.br → GitHub Pages

No hPanel do `.com.br`, abra **Domínios → DNS / Zona DNS** e deixe assim:

| Tipo | Nome | Valor |
|---|---|---|
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| CNAME | `www` | `FernandoHPPinho.github.io` |

Apague registros A/AAAA/CNAME antigos do `@` e do `www` que apontem para a página de estacionamento da Hostinger. Sem isso o domínio não chega no GitHub.

O CNAME do `www` já pode usar `FernandoHPPinho.github.io`.

### 2. pinhoeletrica.com → redireciona para o .com.br

No hPanel do `.com`, use **Redirecionar domínio** (ou **Redirects**):

- De: `pinhoeletrica.com` e `www.pinhoeletrica.com`
- Para: `https://pinhoeletrica.com.br`
- Tipo: permanente (301)

Não aponte o `.com` para o GitHub. Um site no Pages só aceita um domínio; o outro deve só encaminhar.

## Repositório

O código fica em um repositório **privado** no GitHub. Ninguém de fora vê os arquivos.

GitHub Pages grátis só publica repositório público. Com o código privado, o site no ar precisa de outra hospedagem (Hostinger Single é a mais barata) ou do GitHub Pro.
