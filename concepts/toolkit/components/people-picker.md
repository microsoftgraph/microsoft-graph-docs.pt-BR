---
title: Componente de seletor de pessoas
description: Você pode usar o componente Web de gerenciamento de pessoas-seletor para pesquisar um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 2a0680a70ddfd5410e82911e5280c0b1a7e7dcaf
ms.sourcegitcommit: 3e7769ad097e9c34233fa5fea83afa23c34e14a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822792"
---
# <a name="people-picker-component"></a>Componente de seletor de pessoas

Você pode usar a `mgt-people-picker` pesquisa de componente da Web para um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph. Por padrão, o componente pesquisará todas as pessoas; Você também pode definir uma propriedade de grupo para filtrar os resultados.

Se o número de pessoas a serem exibidas exceder o `show-max` valor, nem todas as pessoas retornadas serão exibidas na lista de pesquisa.

## <a name="example"></a>Exemplo

[exemplo de jsfiddle](https://jsfiddle.net/metulev/jdv38fg0/)

```html
<mgt-people-picker></mgt-people-picker>
```

![gerenciamento de pessoas-seletor](./images/mgt-people-picker-image.png)

## <a name="properties"></a>Propriedades

Por padrão, o `mgt-people-picker` componente busca eventos do `/me/people` ponto de extremidade. Use os atributos a seguir para alterar esse comportamento.

| Propriedade | Atributo | Descrição                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| showMax  | show-Max  | Um valor inteiro para indicar o número máximo de pessoas a serem mostradas. o valor padrão é 6.                                                                                             |
| people   | people    | Uma matriz de pessoas para obter ou definir a lista de pessoas renderizadas pelo componente. Use essa propriedade para acessar as pessoas carregadas pelo componente. Defina esse valor para carregar suas próprias pessoas. |
| group    | group     | Um valor String que pertence a um grupo definido pelo Microsoft Graph para mais filtragem dos resultados da pesquisa.                                                                            |

Apresentamos um exemplo a seguir.

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="css-custom-properties"></a>Propriedades personalizadas de CSS

O `mgt-people-picker` componente define as seguintes propriedades personalizadas de CSS.

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Este componente usa as seguintes APIs e permissões do Microsoft Graph.

| API                                                                                                              | Permissão  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/me/people](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0)                    | People.Read |
| [/groups/\${GroupId}/Members](https://docs.microsoft.com/en-us/graph/api/group-list-members?view=graph-rest-1.0) | People.Read |

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).
