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
| CNAME | `www` | `SEU_USUARIO.github.io` |

Apague registros A/AAAA/CNAME antigos do `@` e do `www` que apontem para a página de estacionamento da Hostinger. Sem isso o domínio não chega no GitHub.

O `SEU_USUARIO.github.io` aparece depois do login no GitHub. Eu te passo o valor exato.

### 2. pinhoeletrica.com → redireciona para o .com.br

No hPanel do `.com`, use **Redirecionar domínio** (ou **Redirects**):

- De: `pinhoeletrica.com` e `www.pinhoeletrica.com`
- Para: `https://pinhoeletrica.com.br`
- Tipo: permanente (301)

Não aponte o `.com` para o GitHub. Um site no Pages só aceita um domínio; o outro deve só encaminhar.

## Publicar

Pasta raiz da branch `main` no GitHub Pages. Hospedagem do site: R$ 0. Você só paga os dois domínios.
