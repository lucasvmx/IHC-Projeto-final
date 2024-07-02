# Guia de Acessibilidade Digital

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
