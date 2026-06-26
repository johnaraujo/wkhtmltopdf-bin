# wkhtmltopdf-bin

Binário **wkhtmltopdf 0.12.3 (with patched qt)** — amd64, estático — usado pelo
Minerva2 para gerar PDFs (lavratura/ficha/certidão) com layout idêntico à
produção.

> Por que 0.12.3 e não a 0.12.4 do composer (`h4cc/wkhtmltopdf-amd64`)? A 0.12.4
> renderiza a **largura das tabelas** diferente. Produção usa a 0.12.3.

## Arquivo
- `wkhtmltopdf-amd64-0.12.3` — sha256 em `SHA256SUMS`
  (`b0838a02fcad27c2e80cafeb1a570b4eb474f034fdff7f80af44235a6dcebd24`)

## Uso (Docker do Minerva2 L13)
Baixado via `curl` no `Dockerfile.php84` para `/usr/local/bin/wkhtmltopdf` e
apontado por `WKHTMLTOPDF_BINARY` no `.env`. Ver `docker/l10/` no minerva2.
