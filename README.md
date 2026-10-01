# Histórico de Custos de Manutenção · LOC Frotas

Painel: https://gabrielpitter77.github.io/historico-manutencao/

- `index.html`: a página do painel. Só muda quando o painel ganha funcionalidade nova.
- `base.enc`: a base de dados, **criptografada** (AES-256). Sem usuário e senha, o conteúdo é ilegível.

## Atualização diária (administrador)

1. Baixe a planilha **Custos Despesas Analítico** do sistema.
2. Abra `https://gabrielpitter77.github.io/historico-manutencao/?admin=1` e faça login.
3. Clique em **Carregar base** e escolha a planilha (30 s a 1 min).
4. Confira os totais na mensagem verde e clique em **Gerar base.enc para publicar**.
5. Neste repositório: **Add file → Upload files**, arraste o `base.enc` baixado (substitui o antigo) e clique em **Commit changes**.
6. Em até ~10 minutos todos os analistas veem a base nova pelo link normal.

## Cuidados

- Nunca suba a planilha (.xlsx) nem CSVs aqui: o repositório é público.
- Trocar a senha exige gerar um novo `base.enc` com a senha nova.
- Cada atualização acrescenta ~8 MB ao histórico do repositório. Zere o histórico periodicamente.
