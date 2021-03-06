---
title: People-Picker componente
description: Você pode usar o componente web do se picker mgt-people para pesquisar um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 138c87a004838ae4f1f431e1f553d75ea3a57401
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516658"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a>People-Picker componente no microsoft graph Toolkit

Você pode usar o `mgt-people-picker` componente web para pesquisar pessoas e/ou grupos. Por padrão, o componente procurará por todas as pessoas e usuários na organização, mas você pode alterar o comportamento para também pesquisar grupos ou somente grupos. Você também pode filtrar a pesquisa para um grupo específico.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra o `mgt-people-picker` componente. Comece a procurar um nome para ver os resultados [](#properties) renderizar e use o editor de código para ver como as propriedades alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[Abra este exemplo em mgt.dev](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a>Propriedades

Por padrão, `mgt-people-picker` o componente busca pessoas dos pontos de extremidade `/me/people` `/users` e. Use os atributos a seguir para alterar esse comportamento.

| Atributo | Propriedade | Descrição                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| show-max | showMax   | Um valor de número para indicar o número máximo de pessoas a mostrar. o valor padrão é 6.                                                                                             |
| group-id    | groupId     | Um valor de cadeia de caracteres que pertence a um grupo definido pelo Microsoft Graph para filtrar ainda mais os resultados da pesquisa.                                                                            |
| tipo     | tipo      | O tipo de entidades a ser pesquisada. As opções disponíveis são: `person` , `group` , `any` . O valor padrão é `person`. Esse atributo não terá efeito se `group-id` a propriedade for definida.         
| transitive-search     | transitiveSearch      | Um valor Boolean para executar uma pesquisa transitiva retornando uma lista simples de todos os membros aninhados - por padrão, a pesquisa transitiva não é usada.|
| tipo de grupo     | groupType      | O tipo de grupo a ser pesquisado. As opções disponíveis são: `unified` , , , , `security` `mailenabledsecurity` `distribution` `any` . O valor padrão é `any`. Esse atributo não terá efeito se a `type` propriedade for definida como `person` .                                                                           |
|  selected-people  | selectedPeople     | Uma matriz de pessoas selecionadas. De definir esse valor para selecionar pessoas programaticamente.|
| people   | people    | Uma matriz de pessoas encontradas e renderizadas no resultado da pesquisa |
| placeholder   | placeholder    | O texto padrão que parece explicar como usar o componente. O valor padrão é `Start typing a name`.
| default-selected-user-ids | defaultSelectedUserIds | Quando fornecido uma cadeia de caracteres de IDs de usuário separadas por vírgulas do Microsoft Graph, o componente renderiza os respectivos usuários como selecionados após a inicialização.
| modo de seleção | selectionMode | Usado para indicar se é possível selecionar vários itens (usuários ou grupos) ou apenas um único item. As opções disponíveis são: `single` , `multiple` . O valor padrão é `multiple`.
| desabilitadas | desabilitadas | Define se o se picker de pessoas está desabilitado. Quando desabilitado, o usuário não é capaz de pesquisar ou selecionar pessoas.

A seguir, um `show-max` exemplo.

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a>Pessoas selecionadas

A seção pessoas selecionadas do componente renderiza cada pessoa escolhida pelo desenvolvedor ou usuário. 

![mgt-people-picker](./images/selected-people.png)

Você pode preencher dados de pessoas selecionadas fazendo um dos seguintes:

- Definir a `selectedPeople` propriedade diretamente, conforme mostrado no exemplo a seguir.  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- Usando o método, que aceita uma matriz de IDs de usuário do Microsoft Graph para `selectUsersById()` encontrar detalhes de usuário [associados](/graph/api/resources/users) para seleção.

     >**Observação:** Se nenhum usuário for encontrado para `id` um , nenhum dado será renderizado para isso `id` .

    ```javascript
    // id = Microsoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a>Eventos

Os eventos a seguir são disparados do componente.

| Evento | Descrição |
| --- | --- |
| `selectionChanged` | O usuário adicionou ou removeu uma pessoa da lista de pessoas selecionadas/selecionadas.|

## <a name="css-custom-properties"></a>Propriedades personalizadas CSS

O `mgt-people-picker` componente define as seguintes propriedades personalizadas CSS.

```css
mgt-people-picker {
    --input-border: 2px rgba(255, 255, 255, 0.5) solid; /* sets all input area border */

      /* OR individual input border sides */
    --input-border-bottom: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-right: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-left: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-top: 2px rgba(255, 255, 255, 0.5) solid;

    --input-background-color: #1f1f1f; /* input area background color */
    --input-border-color--hover: #008394; /* input area border hover color */
    --input-border-color--focus: #0f78d4; /* input area border focus color */

    --dropdown-background-color: #1f1f1f; /* selection area background color */
    --dropdown-item-hover-background: #333d47; /* person background color on hover */
    
    --selected-person-background-color: #f1f1f1; /* person item background color */
    
    --color: white; /* input area border focus color */
    --placeholder-color: #f1f1f1; /* placeholder text color */
    --placeholder-color--focus: rgba(255, 255, 255, 0.8); /* placeholder text focus color */
}
```

## <a name="templates"></a>Modelos

 `mgt-people-picker` oferece suporte [a vários modelos](../customize-components/templates.md) que você pode usar para substituir determinadas partes do componente. Para especificar um modelo, inclua um elemento dentro de um componente e de definir o `<template>` valor como um dos `data-type` seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| Padrão. | null: sem dados | O modelo usado para substituir a renderização de todo o componente.
| loading | null: sem dados | O modelo usado para renderizar o estado do selador enquanto a solicitação ao gráfico está sendo feita. |
| erro | null: sem dados | O modelo usado se a pesquisa do usuário não retornar usuários. |
| no-data | null: sem dados | Um modelo alternativo usado se a pesquisa do usuário não retornar usuários. |
| selected-person | pessoa: o objeto de detalhes da pessoa | O modelo para renderizar as pessoas selecionadas. |
| person | pessoa: o objeto de detalhes da pessoa | O modelo para renderizar pessoas no menu suspenso. |

Os exemplos a seguir mostram como usar o `error` modelo.

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Esse componente usa as seguintes APIs e permissões do Microsoft Graph.

| API                                                                                                              | Permissão  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/me/people](/graph/api/user-list-people)                    | People.Read        |
| [/users](/graph/api/user-list)  | User.ReadBasic.All |
| [/groups](/group-list)  | Group.Read.All |
| [/groups/ \$ {groupId}/members](/graph/api/group-list-members) | GroupMember.Read.All        |
| [/users/${userPrincipleName} ](/graph/api/user-get)  | User.Read |

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).

## <a name="extend-for-more-control"></a>Estender para obter mais controle

Para cenários mais complexos ou um UX realmente personalizado, esse componente expõe vários métodos para substituição `protected render*` em extensões de componentes.

| Método | Descrição |
| - | - |
| renderInput | Renderiza a caixa de texto de entrada. |
| renderSelectedPeople | Renderiza os tokens de pessoas selecionados. |
| renderSelectedPerson | Renderiza um token de pessoa individual. |
| renderFlyout | Renderiza o cromado do flyout. |
| renderFlyoutContent | Renderiza o estado apropriado no sobrevoo de resultados. |
| renderLoading | Renderiza o estado de carregamento. |
| renderNoData | Renderiza o estado quando nenhum resultado é encontrado para a consulta de pesquisa. |
| renderSearchResults | Renderiza a lista de resultados da pesquisa. |
| renderPersonResult | Renderiza um resultado de pesquisa de pessoa individual. |
