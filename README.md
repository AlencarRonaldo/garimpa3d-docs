# Garimpa3D

Site da extensão Garimpa3D: página de vendas, calculadora, Termos de Uso e Política de Privacidade.

## Publicar na Vercel

O projeto é estático (HTML, CSS e JavaScript). Não precisa instalar dependências, executar build ou configurar variáveis de ambiente.

1. Envie os arquivos, incluindo `vercel.json`, para o repositório `AlencarRonaldo/garimpa3d-docs` no GitHub.
2. Na Vercel, escolha **Add New → Project** e importe esse repositório.
3. Use **Framework Preset: Other** e a raiz do repositório como **Root Directory** (`./`). Não selecione a pasta `docs` de outro projeto.
4. O `vercel.json` configura a saída na raiz (`.`), sem comandos de instalação ou build.
5. Clique em **Deploy**. Use o endereço fornecido pela Vercel após a conclusão da publicação.

Configure `main` como branch de produção. Depois de conectar o repositório, novos pushes nessa branch podem gerar publicações automáticas.

### Páginas para conferir após publicar

| Endereço | Página |
| --- | --- |
| `/` | Página de vendas |
| `/calculadora` | Calculadora online |
| `/termos` | Termos de Uso |
| `/privacidade` | Política de Privacidade |

Com `cleanUrls`, os endereços com `.html` redirecionam para as versões sem extensão. Os links existentes foram preservados para que o site também continue funcionando no GitHub Pages e ao abrir os arquivos localmente.

Confira os botões dos planos, os cálculos da calculadora e os links do rodapé. O pagamento continua nos checkouts da Kiwify.

## Prévia local

Na pasta deste projeto, execute:

```sh
python -m http.server 8765
```

Abra `http://localhost:8765/`. A prévia simples usa os arquivos `.html`; os redirecionamentos de URLs limpas são aplicados pela Vercel.

## Arquivos

- `index.html`: página de vendas, com estilos e ícones incorporados.
- `calculadora.html`: calculadora com JavaScript no próprio arquivo.
- `termos.html` e `privacidade.html`: documentos públicos.
- `estilo.css`: estilos dos documentos públicos.
- `vercel.json`: configuração da hospedagem.

Referências: [configuração de projetos](https://vercel.com/docs/project-configuration/vercel-json) e [configuração de build](https://vercel.com/docs/builds/configure-a-build).
