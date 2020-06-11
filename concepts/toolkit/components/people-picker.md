---
title: Componente de seletor de pessoas
description: Você pode usar o componente Web de gerenciamento de pessoas-seletor para pesquisar um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: e3e656c6aef0ab2af9878fb3e4738ade912c4685
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681883"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a>Componente de seletor de pessoas no Microsoft Graph Toolkit

Você pode usar o `mgt-people-picker` componente da Web para procurar pessoas e/ou grupos. Por padrão, o componente pesquisará todas as pessoas e usuários da organização, mas você pode alterar o comportamento para também pesquisar grupos ou apenas grupos. Você também pode filtrar a pesquisa para um grupo específico.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra o `mgt-people-picker` componente. Comece a pesquisar um nome para ver os resultados renderizar e usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[Abra este exemplo em gerenciamento de. dev](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a>Propriedades

Por padrão, o `mgt-people-picker` componente busca pessoas dos pontos de `/me/people` `/users` extremidade e. Use os atributos a seguir para alterar esse comportamento.

| Atributo | Propriedade | Descrição                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| show-Max | showMax   | Um valor numérico para indicar o número máximo de pessoas a serem mostradas. o valor padrão é 6.                                                                                             |
| ID de grupo    | groupId     | Um valor String que pertence a um grupo definido pelo Microsoft Graph para mais filtragem dos resultados da pesquisa.                                                                            |
| tipo     | tipo      | O tipo de entidades a serem pesquisadas. As opções disponíveis são: `person` , `group` , `any` . O valor padrão é `person`. Este atributo não terá efeito se a `group-id` propriedade for definida.                                                                            |
| tipo de grupo     | groupType      | O tipo de grupo a ser pesquisado. As opções disponíveis são: `unified` , `security` , `mailenabledsecurity` , `distribution` , `any` . O valor padrão é `any`. Este atributo não terá efeito se a `type` propriedade for definida como `person` .                                                                           |
|  selecionado-pessoas  | selectedPeople     | Uma matriz de pessoas selecionadas. Defina esse valor para selecionar pessoas de forma programática.|
| people   | people    | Uma matriz de pessoas encontrada e renderizada no resultado da pesquisa |

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

     >**Observação:** Se nenhum usuário for localizado para um `id` , nenhum dado será renderizado para isso `id` .

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a>Eventos

Os eventos a seguir são acionados do componente.

| Evento | Descrição |
| --- | --- |
| `selectionChanged` | O usuário adicionou ou removeu uma pessoa da lista de pessoas selecionadas/escolhidas.|

## <a name="css-custom-properties"></a>Propriedades personalizadas de CSS

O `mgt-people-picker` componente define as seguintes propriedades personalizadas de CSS.

```css
mgt-people-picker {
    --input-border: 2px rgba(255, 255, 255, 0.5) solid; /* sets all input area border */

      /* OR individual input border sides */
    --input-border-bottom: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-right: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-left: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-top: 2px rgba(255, 255, 255, 0.5) solid;

    --input-background-color: #1f1f1f; /* input area background color */
    --input-hover-color: #008394; /* input area border hover color */
    --input-focus-color: #0f78d4; /* input area border focus color */

    --dropdown-background-color: #1f1f1f; /* selection area background color */
    --dropdown-item-hover-background: #333d47; /* person background color on hover */

    --font-color: white; /* input area border focus color */
    --placeholder-default-color: #f1f1f1; /* placeholder text color default*/
    --placeholder-focus-color: rgba(255, 255, 255, 0.8); /* placeholder text focus color */
}
```

## <a name="templates"></a>Modelos

 `mgt-people-picker`o dá suporte a vários [modelos](../templates.md) que você pode usar para substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| Padrão. | nulo: não há dados | O modelo usado para substituir a renderização de todo o componente.
| carregando | nulo: não há dados | O modelo usado para renderizar o estado do seletor enquanto a solicitação ao gráfico está sendo feita. |
| erro | nulo: não há dados | O modelo usado se a pesquisa de usuário não retornar nenhum usuário. |
| sem dados | nulo: não há dados | Um modelo alternativo usado se a pesquisa de usuário não retornar nenhum usuário. |
| selecionado-pessoa | Person: o objeto de detalhes da pessoa | O modelo para renderizar as pessoas selecionadas. |
| vendedor | Person: o objeto de detalhes da pessoa | O modelo para renderizar pessoas na lista suspensa. |

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

| API                                                                                                              | Permission  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/me/people](/graph/api/user-list-people?view=graph-rest-1.0)                    | People.Read        |
| [/Users](/graph/api/user-list?view=graph-rest-1.0)  | User.ReadBasic.All |
| [/groups](/group-list?view=graph-rest-beta)  | Group.Read.All |
| [/groups/ \$ {GroupId}/Members](/graph/api/group-list-members?view=graph-rest-1.0) | User.ReadBasic.All        |
| [/Users/$ {userprincípioname}](/graph/api/user-get?view=graph-rest-1.0)  | User.Read |

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).

## <a name="extend-for-more-control"></a>Estender para mais controle

Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected render*` métodos para substituir em extensões de componente.

| Método | Descrição |
| - | - |
| renderInput | Renderiza a caixa de texto de entrada. |
| renderSelectedPeople | Renderiza os tokens de pessoas selecionados. |
| renderSelectedPerson | Renderiza um token de pessoa individual. |
| renderFlyout | Renderiza o cromo domenu. |
| renderFlyoutContent | Processa o estado apropriado no submenu de resultados. |
| renderLoading | Renderiza o estado de carregamento. |
| renderNoData | Renderiza o estado quando nenhum resultado é encontrado para a consulta de pesquisa. |
| renderSearchResults | Renderiza a lista de resultados de pesquisa. |
| renderPersonResult | Renderiza um resultado de pesquisa de pessoa individual. |
