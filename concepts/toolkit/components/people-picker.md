---
title: Componente de seletor de pessoas
description: Você pode usar o componente Web de gerenciamento de pessoas-seletor para pesquisar um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 91b11006df02d563902b99c79c4b1ec09bb7e50a
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639937"
---
# <a name="people-picker-component"></a>Componente de seletor de pessoas

Você pode usar a `mgt-people-picker` pesquisa de componente da Web para um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph. Por padrão, o componente pesquisará todas as pessoas; Você também pode definir uma propriedade de grupo para filtrar os resultados.

Se o número de pessoas a serem exibidas exceder o `show-max` valor, nem todas as pessoas retornadas serão exibidas na lista de pesquisa.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra `mgt-people-picker` o componente. Comece a pesquisar um nome para ver os resultados renderizar e usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[Abra este exemplo em gerenciamento de. dev](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a>Propriedades

Por padrão, o `mgt-people-picker` componente busca eventos do `/me/people` ponto de extremidade. Use os atributos a seguir para alterar esse comportamento.

| Atributo | Propriedade | Descrição                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| show-Max | showMax   | Um valor numérico para indicar o número máximo de pessoas a serem mostradas. o valor padrão é 6.                                                                                             |
| people   | people    | Uma matriz de pessoas para obter ou definir a lista de pessoas renderizadas pelo componente. Use essa propriedade para acessar as pessoas carregadas pelo componente. Defina esse valor para carregar suas próprias pessoas. |
| group    | group     | Um valor String que pertence a um grupo definido pelo Microsoft Graph para mais filtragem dos resultados da pesquisa.                                                                            |
|  selecionado-pessoas  | selectedPeople     | Uma matriz do tipo `person`, representando pessoas selecionadas no componente. Defina esse valor para escolher as pessoas selecionadas por padrão.|

Este é um `show-max` exemplo.

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a>Pessoas selecionadas

A seção de pessoas selecionada do componente renderiza cada pessoa escolhida pelo desenvolvedor ou pelo usuário. 

![gerenciamento de pessoas-seletor](./images/selected-people.png)

Você pode preencher dados de pessoas selecionados executando um dos seguintes procedimentos:

- Definir a `selectedPeople` propriedade diretamente, conforme mostrado no exemplo a seguir.  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- Usando o `selectUsersById()` método, que aceita uma matriz de IDs de [usuário](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) do Microsoft Graph para localizar os detalhes do usuário associado para seleção.

     >**Observação:** Se nenhum usuário for localizado para um `id`, nenhum dado será renderizado para isso `id`.

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="css-custom-properties"></a>Propriedades personalizadas de CSS

O `mgt-people-picker` componente define as seguintes propriedades personalizadas de CSS.

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="templates"></a>Modelos

 `mgt-people-picker`o dá suporte a vários [modelos](../templates.md) que você pode usar para substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| carregando | nulo: não há dados | O modelo usado para renderizar o estado do seletor enquanto a solicitação ao gráfico está sendo feita. |
| erro | nulo: não há dados| O modelo usado se a pesquisa de usuário não retornar nenhum usuário. |
| selecionado-pessoa |Person: o objeto de detalhes da pessoa| O modelo para renderizar as pessoas selecionadas. |
| vendedor | Person: o objeto de detalhes da pessoa| O modelo para renderizar pessoas na lista suspensa. |

Os exemplos a seguir mostram como usar o `error` modelo.

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Este componente usa as seguintes APIs e permissões do Microsoft Graph.

| API                                                                                                              | Permissão  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/me/people](/graph/api/user-list-people?view=graph-rest-1.0)                    | People.Read        |
| [/groups/\${GroupId}/Members](/graph/api/group-list-members?view=graph-rest-1.0) | People.Read        |
| [/Users/$ {userprincípioname}](/graph/api/user-list-people?view=graph-rest-1.0)  | User. Readbasic. All |

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).
