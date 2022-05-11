---
title: Componente do seletor de pessoas
description: Você pode usar o componente Web mgt-people-picker para pesquisar um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: d35e801dd851a4bb6f8ace37eb706bdb6182af92
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314890"
---
# <a name="people-picker-component-in-microsoft-graph-toolkit"></a>Componente seletor de pessoas no Microsoft Graph Toolkit

Você pode usar o componente `mgt-people-picker` Web para pesquisar pessoas e/ou grupos. Por padrão, o componente pesquisará todas as pessoas e usuários na organização, mas você pode alterar o comportamento para também pesquisar grupos ou apenas grupos. Você também pode filtrar a pesquisa para um grupo específico. Além disso, você pode permitir que o usuário insira e selecione qualquer endereço de email.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra o `mgt-people-picker` componente. Comece a pesquisar um nome para ver os resultados renderizarem e use o editor de código [](#properties) para ver como as propriedades alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[Abrir este exemplo no mgt.dev](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a>Propriedades

Por padrão, o `mgt-people-picker` componente busca pessoas dos pontos `/me/people` de `/users` extremidade e das pessoas. Use os atributos a seguir para alterar esse comportamento.

| Atributo | Propriedade | Descrição                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| show-max | showMax   | Um valor numérico para indicar o número máximo de pessoas a serem mostradas. o valor padrão é 6.                                                                                             |
| group-id    | groupId     | Um valor de cadeia de caracteres que pertence a um grupo Graph microsoft para filtragem adicional dos resultados da pesquisa.                                                                            |
| transitive-search     | transitiveSearch      | Um valor booliano para executar uma pesquisa transitiva retornando uma lista simples de todos os membros aninhados – por padrão, a pesquisa transitiva não é usada.|
| type     | type      | O tipo de entidades a serem pesquisadas. As opções disponíveis são: `person`, `group`, `any`. O valor padrão é `person`. Esse atributo não terá efeito se a `group-id` propriedade for definida.         
| tipo de usuário     | userType      | O tipo de usuário a ser pesquisado. As opções disponíveis são: `any`, `user` para usuários organizacionais ou `contact` para contatos. O valor padrão é `any`. |
| tipo de grupo     | groupType      | O tipo de grupo a ser pesquisado. As opções disponíveis são: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`. O valor padrão é `any`. Esse atributo não terá efeito se a `type` propriedade for definida como `person`.  |
| pessoas selecionadas  | selectedPeople     | Uma matriz de pessoas selecionadas. Defina esse valor para selecionar pessoas programaticamente.|
| people   | people    | Uma matriz de pessoas encontradas e renderizadas no resultado da pesquisa |
| Espaço   | Espaço    | O texto padrão que aparece para explicar como usar o componente. O valor padrão é `Start typing a name`.
| default-selected-user-ids | defaultSelectedUserIds | Quando fornecida uma cadeia de caracteres de IDs de usuário do Microsoft Graph separada por vírgulas, o componente renderiza os respectivos usuários conforme selecionado na inicialização.
| default-selected-group-ids | defaultSelectedGroupIds | Semelhante às IDs de usuário selecionadas por padrão, quando fornecida uma cadeia de caracteres de IDs de grupo do Microsoft Graph separadas por vírgulas, o componente renderiza os respectivos grupos conforme selecionado na inicialização.
| modo de seleção | selectionMode | Usado para indicar se deseja permitir a seleção de vários itens (usuários ou grupos) ou apenas um único item. As opções disponíveis são: `single`, `multiple`. O valor padrão é `multiple`.
| desabilitadas | desabilitadas | Define se o seletor de pessoas está desabilitado. Quando desabilitado, o usuário não é capaz de pesquisar ou selecionar pessoas.
| disable-images | disableImages | Define se a busca e a exibição de imagens da pessoa devem ser desabilitadas. Quando definido como `true`, as iniciais do usuário são exibidas.
| allow-any-email | allowAnyEmail | Indica se o seletor de pessoas pode aceitar endereços de email sem selecionar uma pessoa. O valor padrão é `false`. Ao terminar de digitar um endereço de email, você pode pressionar vírgula (`,`), ponto e vírgula (`;`), tabulação ou inserir teclas para adicioná-lo.
| user-ids | userIds | Uma cadeia de caracteres de IDs de usuário separadas por vírgulas. Eles só aparecerão no menu suspenso ou nos resultados da pesquisa quando você digitar uma consulta. Por exemplo `48d31887-5fad-4d73-a9f5-3c356e68a038,24fcbca3-c3e2-48bf-9ffc-c7f81b81483d` , só exibirá os dois usuários na lista suspensa quando a entrada estiver focada. Quando você digita um texto de pesquisa, ele retorna resultados que correspondem apenas aos usuários nas duas IDs de usuário.
| filtros de usuário | userFilters | Especifica os critérios de filtro a serem usado ao consultar o ponto de extremidade dos usuários. Ele requer que `user-type` seja definido como `user` ou `contact`. Por padrão, é `user-type` e `any` isso leva a consulta a ocorrer no bloco `people` de ponto de extremidade. Exemplo: `user-filters="startsWith(displayName,'a')"`. Esse atributo é opcional. Saiba mais sobre [o suporte para filtro nas propriedades do usuário Azure AD de diretório](/graph/aad-advanced-queries?tabs=http#user-properties).
| filtros de grupo | groupFilters | Especifica os critérios de filtro a serem usado ao consultar o ponto `groups` de extremidade. Ele requer que `type` seja definido como `group`. Exemplo: `group-filters="startsWith(displayName,'a')"`. Esse atributo é opcional.
| filtros de pessoas | peopleFilters | Especifica os critérios de filtro a serem usado ao consultar o ponto `people` de extremidade. Ele é usado como está. Exemplo: `people-filters="jobTitle eq 'Web Marketing Manager'"`. Esse atributo é opcional. Saiba mais sobre [a filtragem e os recursos com suporte no recurso de pessoas](/graph/people-example).
| group-ids | groupIds | Uma cadeia de caracteres de IDs de grupo separadas por vírgulas. Os resultados disponíveis devem ser limitados aos grupos especificados. Os usuários que aparecerão no menu suspenso e por meio da experiência de pesquisa só devem vir das IDs de grupo especificadas. Por exemplo, `02bd9fd6-8f93-4758-87c3-1fb73740a315,06f62f70-9827-4e6e-93ef-8e0f2d9b7b23` exibirá apenas os usuários que pertencem a esses grupos. Quando você digita um texto de pesquisa, ele retorna resultados que correspondem apenas aos usuários nas duas IDs de grupo. Essa propriedade não será usada se `group-id` estiver definida. Se a propriedade for definida, ela `type` será definida `group` por padrão e `trnsitive-search` será `true` por padrão. Se o `group-type` conjunto for com a propriedade, poderá `type` ser `any` ou `group`. Se for `type` , `person`a propriedade não será usada.

A seguir está um `show-max` exemplo.

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a>Pessoas selecionadas

A seção de pessoas selecionadas do componente renderiza cada pessoa escolhida pelo desenvolvedor ou usuário. 

![mgt-people-picker](./images/selected-people.png)

Você pode popular os dados das pessoas selecionadas seguindo um dos seguintes procedimentos:

- Definir a `selectedPeople` propriedade diretamente, conforme mostrado no exemplo a seguir.  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- Usando o `selectUsersById()` método, que aceita uma matriz de [IDs](/graph/api/resources/users) de usuário do Microsoft Graph para localizar detalhes de usuário associados para seleção.

     >**Nota:** Se nenhum usuário for encontrado para um `id`, nenhum dado será renderizado para isso `id`.

    ```javascript
    // id = Microsoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

- Usando o `selectGroupsById()` método, que aceita uma matriz de [IDs](/graph/api/resources/group) de grupo do Microsoft Graph para localizar os grupos com usuários associados.

    ```javascript
    // groupid = Microsoft graph group "id"
    document.querySelector('mgt-people-picker').selectGroupsById(["groupid","groupid"])
    ```

## <a name="events"></a>Eventos

Os eventos a seguir são disparados do componente.

Evento | Quando ele é emitido | Dados personalizados | Cancelável | Bolhas | Funciona com modelo personalizado
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`selectionChanged` | O usuário adicionou ou removeu uma pessoa da lista de pessoas selecionadas/selecionadas | Matriz de pessoas selecionadas, em que uma pessoa pode ser Graph [](/graph/api/resources/person) [](/graph/api/resources/contact) [usuário,](/graph/api/resources/user)`personImage` pessoa ou contato com uma propriedade adicional que contém a URL da foto do usuário | Não | Não | Sim, a menos que você substitua o modelo padrão

Para obter mais informações sobre como manipular eventos, consulte [eventos](../customize-components/events.md).

## <a name="css-custom-properties"></a>Propriedades personalizadas css

O `mgt-people-picker` componente define as seguintes propriedades personalizadas css.

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

 `mgt-people-picker` dá suporte [a vários modelos](../customize-components/templates.md) que você pode usar para substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| Padrão. | null: sem dados | O modelo usado para substituir a renderização de todo o componente.
| Carregar | null: sem dados | O modelo usado para renderizar o estado do seletor enquanto a solicitação para o grafo está sendo feita. |
| erro | null: sem dados | O modelo usado se a pesquisa do usuário não retornar nenhum usuário. |
| sem dados | null: sem dados | Um modelo alternativo usado se a pesquisa de usuário não retornar nenhum usuário. |
| pessoa selecionada | pessoa: o objeto de detalhes da pessoa | O modelo para renderizar as pessoas selecionadas. |
| person | pessoa: o objeto de detalhes da pessoa | O modelo para renderizar pessoas na lista suspensa. |

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

| Configuração | Permissão | API
| --- | ---------- | ------- |
| `group-id` Definir | People.Read, User.Read.All, GroupMember.Read.All | [/groups/\${groupId}/members](/graph/api/group-list-members) |
| `type` definido como `Person` ou `any` | People.Read | [/me/people](/graph/api/user-list-people) |
| `type` definido como `Group` ou pesquisando usuários e `type` definido como `Group` ou `any` | Group.Read.All | [/groups](/graph/api/group-list) |
| `default-selected-user-ids` Definir | User.ReadBasic.All | [/users](/graph/api/user-list) |
| pesquisando usuários e definido `type` como `Person` ou `any` | People.Read, User.ReadBasic.All | [/me/people](/graph/api/user-list-people), [/users](/graph/api/user-list) |

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).

## <a name="cache"></a>Cache

|Repositório de objetos|Dados armazenados em cache|Comentários|
|---------|-----------|-------|
|`groups`|Lista de grupos|Usado quando `type` é definido como `PersonType.group`|
|`people`|Lista de pessoas|Usado quando `type` é definido como `PersonType.person` ou `PersonType.any`|
|`users`|Lista de usuários|Usado quando `groupId` especificado|

Consulte [Caching](../customize-components/cache.md) para obter mais detalhes sobre como configurar o cache.

## <a name="extend-for-more-control"></a>Estender para obter mais controle

Para cenários mais complexos ou uma experiência do usuário realmente personalizada, esse componente expõe `protected render*` vários métodos para substituição em extensões de componente.

| Método | Descrição |
| - | - |
| renderInput | Renderiza a caixa de texto de entrada. |
| renderSelectedPeople | Renderiza os tokens de pessoas selecionados. |
| renderSelectedPerson | Renderiza um token de pessoa individual. |
| renderFlyout | Renderiza o cromado do submenu. |
| renderFlyoutContent | Renderiza o estado apropriado no submenu de resultados. |
| renderLoading | Renderiza o estado de carregamento. |
| renderNoData | Renderiza o estado quando nenhum resultado é encontrado para a consulta de pesquisa. |
| renderSearchResults | Renderiza a lista de resultados da pesquisa. |
| renderPersonResult | Renderiza um resultado de pesquisa de pessoa individual. |
