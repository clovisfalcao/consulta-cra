# Consulta anônima de posição do CRA

Ferramenta informativa para estudantes do Bacharelado em Direito — Unidade Santa Rita — consultarem uma estimativa da sua posição na distribuição dos Coeficientes de Rendimento Acadêmico (CRA).

A página está disponível em [clovisfalcao.github.io/consulta-cra](https://clovisfalcao.github.io/consulta-cra).

## O que a ferramenta faz

A consulta permite informar o CRA e visualizar:

- posição e percentil estimados no curso;
- comparação estimada com o grupo de ingresso, quando informado;
- indicação estimada de posição acima do percentil 90;
- mediana, média, mínimo e máximo da base;
- gráficos da distribuição dos CRAs e da comparação entre turmas.

O CRA é utilizado em processos seletivos internos, como monitoria, pesquisa, extensão e reopção de curso, além de compor o critério de nota da láurea acadêmica.

## Privacidade

A página funciona inteiramente no navegador, sem login ou senha.

Os dados de referência são agregados e anônimos: não incluem nomes nem matrículas completas. O CRA e a matrícula eventualmente informados pelo estudante não são enviados, salvos ou armazenados.

## Como usar

1. Informe seu CRA. São aceitos vírgula ou ponto (`7,43`) e também apenas dígitos (`743`).
2. Opcionalmente, informe a matrícula para estimar o ano de ingresso pelos quatro primeiros dígitos.
3. Para matrículas antigas ou de numeração especial, selecione manualmente o ano de ingresso quando o campo for exibido.
4. Consulte o resultado estimado.

## Limites e atualização dos dados

Os resultados são estimativas calculadas a partir de dados agregados, atualizados até **07/07/2026**. Eles não substituem os registros oficiais da UFPB ou as informações disponíveis no SIGAA.

Em caso de divergência, entre em contato com a Coordenação do Bacharelado em Direito — Unidade Santa Rita: [direitosantarita@ccj.ufpb.br](mailto:direitosantarita@ccj.ufpb.br).

## Manutenção

Os dados são mantidos diretamente em `index.html`, no bloco `DADOS_CSV`. Ao atualizá-los, preserve apenas as colunas `ano` e `cra`; não inclua nomes nem matrículas completas.

## Desenvolvimento

A ferramenta foi desenvolvida com apoio do **Codex** e do **Claude**.

## Licença

Este projeto é distribuído sob a [Licença MIT](LICENSE).
