# vozdoestudante.com.br → www.vozdoestudante.com.br

Este repositório só redireciona o domínio raiz `vozdoestudante.com.br` para `https://www.vozdoestudante.com.br`, onde está a página do Voz do Estudante (serviço `student-voice-download-landing` no Railway).

O DNS do domínio fica no Registro.br, que não aceita apontar o domínio raiz para o Railway (não há CNAME flattening nem ALIAS). Por isso o domínio raiz tem registros A e AAAA para o GitHub Pages, que serve esta página com HTTPS. O `index.html` e o `404.html` mandam para o mesmo caminho no `www`.

Não apague este repositório nem desligue o GitHub Pages enquanto os registros A e AAAA do domínio raiz apontarem para o GitHub. Se o DNS for para um provedor com CNAME flattening, aponte o domínio raiz direto para o Railway e remova os registros do GitHub.
