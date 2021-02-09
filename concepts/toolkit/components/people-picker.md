---
title: People-Picker componente
description: Você pode usar o componente web mgt-people-picker para pesquisar um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 691955aa64ff0afc42b5f8912658a6f36e1d77ec
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161373"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a>People-Picker componente no Kit de Ferramentas do Microsoft Graph

Você pode usar o `mgt-people-picker` componente web para pesquisar pessoas e/ou grupos. Por padrão, o componente pesquisa todas as pessoas e usuários na organização, mas você pode alterar o comportamento para também pesquisar grupos ou apenas grupos. Você também pode filtrar a pesquisa para um grupo específico.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra o `mgt-people-picker` componente. Comece procurando um nome para ver os resultados renderizar [](#properties) e use o editor de código para ver como as propriedades alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[Abra este exemplo em mgt.dev](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a>Propriedades

Por padrão, o `mgt-people-picker` componente busca pessoas dos pontos de extremidade e dos pontos de `/me/people` `/users` extremidade. Use os atributos a seguir para alterar esse comportamento.

| Atributo | Propriedade | Descrição                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| show-max | showMax   | Um valor de número para indicar o número máximo de pessoas a mostrar. o valor padrão é 6.                                                                                             |
| group-id    | groupId     | Um valor de cadeia de caracteres que pertence a um grupo definido pelo Microsoft Graph para filtrar ainda mais os resultados da pesquisa.                                                                            |
| type     | type      | O tipo de entidades a ser pesquisada. As opções disponíveis são: `person` , `group` , `any` . O valor padrão é `person`. Esse atributo não terá efeito se `group-id` a propriedade for definida.         
| transitive-search     | transitiveSearch      | Um valor Boolean para executar uma pesquisa transitiva retornando uma lista simples de todos os membros aninhados - por padrão, a pesquisa transitiva não é usada.|
| tipo de grupo     | groupType      | O tipo de grupo a ser pesquisado. As opções disponíveis são: `unified` , , , , `security` `mailenabledsecurity` `distribution` `any` . O valor padrão é `any`. Esse atributo não terá efeito se a `type` propriedade estiver definida como `person` .                                                                           |
|  selected-people  | selectedPeople     | Uma matriz de pessoas selecionadas. De definir esse valor para selecionar pessoas de forma programática.|
| people   | people    | Uma matriz de pessoas encontradas e renderizadas no resultado da pesquisa |
| espaço reservado   | espaço reservado    | O texto padrão que parece explicar como usar o componente. O valor padrão é `Start typing a name`.
| default-selected-user-ids | defaultSelectedUserIds | Quando fornecida uma cadeia de caracteres de IDs de usuário separadas por vírgulas do Microsoft Graph, o componente renderiza os respectivos usuários conforme selecionado na inicialização.
| modo de seleção | selectionMode | Usado para indicar se é para permitir a seleção de vários itens (usuários ou grupos) ou apenas um único item. As opções disponíveis são: `single` , `multiple` . O valor padrão é `multiple`.

A seguir está um `show-max` exemplo.

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a>Pessoas selecionadas

A seção de pessoas selecionada do componente renderiza cada pessoa escolhida pelo desenvolvedor ou usuário. 

![mgt-people-picker](./images/selected-people.png)

Você pode preencher dados de pessoas selecionadas seguindo um dos seguintes:

- Definir a `selectedPeople` propriedade diretamente, conforme mostrado no exemplo a seguir.  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- Usando o método, que aceita uma matriz de IDs de usuário do Microsoft Graph para `selectUsersById()` encontrar detalhes de usuário associados para seleção. [](/graph/api/resources/users)

     >**Observação:** Se nenhum usuário for encontrado para `id` um , nenhum dado será renderizado para `id` isso.

    ```javascript
    // id = Microsoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a>Eventos

Os eventos a seguir são disparados do componente.

| Evento | Descrição |
| --- | --- |
| `selectionChanged` | O usuário adicionou ou removeu uma pessoa da lista de pessoas selecionadas/selecionadas.|

## <a name="css-custom-properties"></a>Propriedades personalizadas css

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

 `mgt-people-picker` oferece suporte [a vários modelos](../customize-components/templates.md) que você pode usar para substituir determinadas partes do componente. Para especificar um modelo, inclua um elemento dentro de um componente e de definir `<template>` o valor como um dos `data-type` seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| Padrão. | null: sem dados | O modelo usado para substituir a renderização do componente inteiro.
| carregando | null: sem dados | O modelo usado para renderizar o estado do selador enquanto a solicitação para o gráfico está sendo feita. |
| erro | null: sem dados | O modelo usado se a pesquisa do usuário não retornar usuários. |
| no-data | null: sem dados | Um modelo alternativo usado se a pesquisa do usuário não retornar usuários. |
| selected-person | pessoa: O objeto de detalhes da pessoa | O modelo para renderizar as pessoas selecionadas. |
| person | pessoa: O objeto de detalhes da pessoa | O modelo para renderizar pessoas no menu suspenso. |

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
| [/groups/ \$ {groupId}/members](/graph/api/group-list-members) | User.ReadBasic.All        |
| [/users/${userPrincipleName} ](/graph/api/user-get)  | User.Read |

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação.](../providers/providers.md)

## <a name="extend-for-more-control"></a>Estender para obter mais controle

Para cenários mais complexos ou uma experiência de trabalho realmente personalizada, esse componente expõe vários métodos para substituição `protected render*` em extensões de componente.

| Método | Descrição |
| - | - |
| renderInput | Renderiza a caixa de texto de entrada. |
| renderSelectedPeople | Renderiza os tokens de pessoas selecionadas. |
| renderSelectedPerson | Renderiza um token de pessoa individual. |
| renderFlyout | Renderiza o cromado do flyout. |
| renderFlyoutContent | Renderiza o estado apropriado no flyout de resultados. |
| renderLoading | Renderiza o estado de carregamento. |
| renderNoData | Renderiza o estado quando nenhum resultado é encontrado para a consulta de pesquisa. |
| renderSearchResults | Renderiza a lista de resultados da pesquisa. |
| renderPersonResult | Renderiza um resultado de pesquisa de pessoa individual. |
