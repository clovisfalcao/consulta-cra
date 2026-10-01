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

1. Informe seu CRA. São aceitos vírgula ou ponto (`7,43`) e também apenas dígitos (`743`). `10` é lido como 10,00.
2. Opcionalmente, informe a matrícula. A turma é definida pelo ano dos quatro primeiros dígitos, que pode ser diferente do ano em que as aulas começaram por causa do calendário atrasado.
3. Se a matrícula não for reconhecida, escolha o ano da matrícula no campo que aparece. Escolher o ano dispensa a matrícula, e informar a matrícula dispensa o ano.
4. Consulte o resultado estimado.

Matrículas iniciadas por 1 correspondem a ingresso anterior a 2017. Esse grupo, assim como a turma mais recente (2026), não entra na comparação entre turmas, mas continua na posição geral no curso. Os registros da turma mais recente com CRA 0,00, de estudantes ainda sem notas lançadas, ficam fora das estimativas gerais. O percentil 90 da láurea usa a lista completa, como o sistema da UFPB.

## Limites e atualização dos dados

Os resultados são estimativas calculadas a partir de dados agregados, atualizados até **23/08/2026**. Eles não substituem os registros oficiais da UFPB ou as informações disponíveis no SIGAA.

Em caso de divergência, entre em contato com a Coordenação do Bacharelado em Direito — Unidade Santa Rita: [direitosantarita@ccj.ufpb.br](mailto:direitosantarita@ccj.ufpb.br).

## Manutenção

Os dados são mantidos diretamente em `index.html`, no bloco `DADOS_CSV`. Ao atualizá-los, preservar apenas as colunas `ano` e `cra`; não incluir nomes nem matrículas completas. Ano em branco indica matrícula iniciada por 1 (ingresso anterior a 2017).

A próxima atualização deve ocorrer entre fevereiro e março de 2027, com a lista de 2027. Nela, além de `DADOS_CSV`, é preciso trocar `ANO_BASE` para 2027, atualizar `DATA_ATUALIZACAO` e a data citada neste README e revisar `ANO_TURMA_SEM_COMPARACAO`. O comentário no início do script de `index.html` lista esses pontos.

## Desenvolvimento

A ferramenta foi desenvolvida com uso dos aplicativos **Codex** e **Claude**.

## Licença

Este projeto é distribuído sob a [Licença MIT](LICENSE).
