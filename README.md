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

Matrículas iniciadas por 1 correspondem a ingresso anterior a 2017. Esse grupo, assim como a turma mais recente (2026), não entra na comparação entre turmas, mas continua na posição geral no curso. A posição geral, a mediana, a média e o percentil 90 da láurea usam a lista completa do curso, inclusive os registros com CRA 0,00 de estudantes ainda sem notas lançadas.

## Limites e atualização dos dados

Os resultados são estimativas calculadas a partir de dados agregados, atualizados até a data informada na página. Eles não substituem os registros oficiais da UFPB ou as informações disponíveis no SIGAA.

Em caso de divergência, entre em contato com a Coordenação do Bacharelado em Direito — Unidade Santa Rita: [direitosantarita@ccj.ufpb.br](mailto:direitosantarita@ccj.ufpb.br).

## Manutenção

Para atualizar a consulta, troque apenas o arquivo `dados.js`. Ele reúne a tabela de ano e CRA, o ano da lista, a data de atualização e a turma mais recente, e o comentário no início dele explica cada item e os formatos de tabela aceitos. O `index.html` não precisa ser alterado. Na tabela, não incluir nomes nem matrículas completas.

A próxima atualização deve ocorrer entre fevereiro e março de 2027, com a lista de 2027.

## Desenvolvimento

A ferramenta foi desenvolvida com uso dos aplicativos **Codex** e **Claude**.

## Licença

Este projeto é distribuído sob a [Licença MIT](LICENSE).
