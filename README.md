# Guia de Acessibilidade Digital

# Sumário
- [Orientações de Acessibilidade](#Orientações-de-Acessibilidade)
  * [Deficiência Visual](#Deficiência-Visual)
  * [Deficiência Física](#Deficiência-Física)
  * [Deficiência Auditiva](#Deficiência-Auditiva)
  * [Deficiência de Fala](#Deficiência-de-Fala)
  * [Limitações Relacionadas à Idade](#Limitações-Relacionadas-à-Idade)
  * [Neurodivergentes](#Neurodivergentes)
- [Padrões de codificação](#Padrões-de-codificação)
  * [Utilizar arquivos externos para as Folhas de estilo (CSS) e Javascript](#Utilizar-arquivos-externos-para-as-Folhas-de-estilo-(CSS)-e-Javascript)
  
# Orientações de Acessibilidade

## Deficiência Visual

O site, de modo geral, não possui uma acessibilidade aceitável para deficientes visuais. Ele conta com um modo de contraste para daltônicos e pessoas com dificuldades em perceber contraste de cores. No entanto, o botão para ativar esse modo está em uma posição pouco intuitiva, e o texto do botão possui um contraste ruim com a página. O site permite a alteração do tamanho da fonte, o que ajuda pessoas com problemas de visão como miopia, astigmatismo e hipertrofia. Porém, não há descrições de imagens, o que dificulta a navegação para deficientes visuais. Pessoas cegas enfrentariam ainda mais dificuldades, pois o site não oferece leitura automática de textos nem navegação por comandos de voz.

As imagens apresentadas no site não possuem legendas descritivas, essenciais para deficientes visuais.


## Deficiência Física

O site apresenta barreiras significativas para pessoas com deficiência física. A navegação exige o uso de botões pequenos, o que pode ser estressante e desafiador para pessoas com tremores, movimentos involuntários ou dores que limitam movimentos. Em casos mais graves, a ausência de uma ferramenta de acesso que não exija clicar em botões torna o site inavegável para pessoas com paralisia, dores severas ou ausência de membros.

## Deficiência Auditiva

O site não utiliza meios auditivos para realizar ações, garantindo que nenhum deficiente auditivo seja prejudicado ao utilizá-lo.

## Deficiência de Fala

O site não requer o uso da fala para nenhuma ação, garantindo que nenhum usuário com deficiência de fala seja prejudicado ao utilizá-lo.

## Neurodivergentes

O site não possui cores agressivas que poderiam assustar ou afastar pessoas neurodivergentes, apresentando um ambiente acolhedor para a maioria das neurodivergências visuais. Além disso, o site não utiliza recursos auditivos ou de fala, evitando problemas relacionados. A interface é fácil de entender, com gráficos coloridos e interativos e vídeos explicativos. O único ponto negativo são as tabelas detalhadas, que podem ser pouco atrativas para pessoas neurodivergentes.

## Limitações Relacionadas à Idade

Pessoas idosas podem usar o site com relativa facilidade, embora possam enfrentar dificuldades em clicar nos botões caso sofram de deterioração física. Outro problema potencial é a cegueira causada por problemas de saúde, o que tornaria a utilização do site praticamente impossível para esses usuários.


# Padrões de codificação

## Utilizar arquivos externos para as Folhas de estilo (CSS) e Javascript

Exemplo:

```html
<link rel="stylesheet" type="text/css" media="screen" href="style.css" />
```

## Limitar as requisições HTTP

Muitas requisições HTTP reduzem o desempenho do navegador

## Evitar o uso de popups

Pop-ups são janelas de diversos tamanhos que abrem com avisos e publicidade. Esse recurso deve ser evitado a todo o custo em sítios governamentais.

Alguns motivos para o não uso de pop-ups:

- Os navegadores mais modernos bloqueiam pop-ups. Sendo assim, se algum informe importante é dado pelo pop-up ele não é visto.
- Pop-ups não são acessíveis. Usuários que usam programas leitores de tela podem se perder, sem saber onde estão ou se realmente entraram no sitio pretendido.
- Alguns pop-ups mais modernos costumam burlar o sistema anti-pop-up dos navegadores carregando na própria página, atrapalhando a leitura do onteúdo.
- Informações importantes devem sempre estar em destaque dentro da página. Na diagramação reserve um espaço para os destaques, que pode ser desativado caso não esteja sendo usado. Nunca use pop-ups para avisos importantes, como recadastro de usuários ou para carregar aplicações ou novas instâncias da página.

## Utilizar URL's amigáveis

Cada página de um sítio deve ser identificada com sua URL única e compreensível.

```
Certo: http://www.portal.gov.br/contato

Errado: http://www.portal.gov.br/default.php?reg=2&p_secao=18
```

## Declarar o doctype correto da página

Todo documento HTML e XHTML deve declarar o doctype correto para ser considerado válido. O doctype informa ao navegador o tipo de documento que deve ser usado ao carregar a página. É também por meio da declaração de doctype que as ferramentas de validação analisam o código da página e indicam correções.

Existem três tipos: 

- Frameset
- Strict
- Transational
