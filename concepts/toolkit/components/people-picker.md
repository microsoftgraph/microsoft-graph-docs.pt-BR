---
title: People-Picker componente
description: Você pode usar o componente web mgt-people-picker para pesquisar um número especificado de pessoas e renderizar a lista de resultados por meio do Microsoft Graph.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: c66f28ec02ea45f74f7590fb98f3cf17e5cbec0d
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587417"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a>People-Picker componente no microsoft Graph Toolkit

Você pode usar o componente `mgt-people-picker` web para pesquisar pessoas e/ou grupos. Por padrão, o componente procurará por todas as pessoas e usuários na organização, mas você pode alterar o comportamento para também pesquisar grupos ou somente grupos. Você também pode filtrar a pesquisa para um grupo específico. Além disso, você pode permitir que o usuário insira e selecione qualquer endereço de email.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra o `mgt-people-picker` componente. Comece a procurar um nome para ver os resultados renderizar e use o editor de código para [](#properties) ver como as propriedades alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[Abrir este exemplo no mgt.dev](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a>Propriedades

Por padrão, o `mgt-people-picker` componente busca pessoas dos pontos `/me/people` de `/users` extremidade e. Use os atributos a seguir para alterar esse comportamento.

| Atributo | Propriedade | Descrição                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| show-max | showMax   | Um valor de número para indicar o número máximo de pessoas a mostrar. o valor padrão é 6.                                                                                             |
| group-id    | groupId     | Um valor de cadeia de caracteres que pertence a um grupo Graph da Microsoft para filtrar ainda mais os resultados da pesquisa.                                                                            |
| transitive-search     | transitiveSearch      | Um valor Boolean para executar uma pesquisa transitiva retornando uma lista simples de todos os membros aninhados - por padrão, a pesquisa transitiva não é usada.|
| type     | type      | O tipo de entidades a ser pesquisada. As opções disponíveis são: `person`, , `group`. `any` O valor padrão é `person`. Esse atributo não terá efeito se a `group-id` propriedade for definida.         
| tipo de usuário     | userType      | O tipo de usuário a ser pesquisado. As opções disponíveis são: `any`, para `user` usuários organizacionais ou `contact` para contatos. O valor padrão é `any`. |
| tipo de grupo     | groupType      | O tipo de grupo a ser pesquisado. As opções disponíveis são: `unified`, `security`, `mailenabledsecurity`, , `distribution`. `any` O valor padrão é `any`. Esse atributo não terá efeito se a `type` propriedade for definida como `person`.  |
| selected-people  | selectedPeople     | Uma matriz de pessoas selecionadas. De definir esse valor para selecionar pessoas programaticamente.|
| people   | people    | Uma matriz de pessoas encontradas e renderizadas no resultado da pesquisa |
| placeholder   | placeholder    | O texto padrão que parece explicar como usar o componente. O valor padrão é `Start typing a name`.
| default-selected-user-ids | defaultSelectedUserIds | Quando fornecido uma cadeia de caracteres de IDs de usuário separadas por vírgulas da Microsoft Graph, o componente renderiza os respectivos usuários como selecionados após a inicialização.
| default-selected-group-ids | defaultSelectedGroupIds | Semelhante a IDs de grupo padrão selecionadas-user-ids, quando fornecida uma cadeia de caracteres de IDs de grupo do Microsoft Graph separadas por vírgulas, o componente renderiza os respectivos grupos como selecionados após a inicialização.
| modo de seleção | selectionMode | Usado para indicar se é possível selecionar vários itens (usuários ou grupos) ou apenas um único item. As opções disponíveis são: `single`, `multiple`. O valor padrão é `multiple`.
| desabilitadas | desabilitadas | Define se o se picker de pessoas está desabilitado. Quando desabilitado, o usuário não é capaz de pesquisar ou selecionar pessoas.
| disable-images | disableImages | Define se deve desabilitar a busca e a exibição de imagens de pessoas. Quando definido como `true`, as iniciais do usuário são exibidas em vez disso.
| allow-any-email | allowAnyEmail | Indica se o seletor de pessoas pode aceitar endereços de email sem selecionar uma pessoa. O valor padrão é `false`. Ao concluir a digitação de um endereço de email, você pode pressionar vírgula (`,`), ponto e vírgula (`;`), guia ou inserir teclas para adicioná-lo.
| user-ids | userIds | Uma cadeia de caracteres de IDs de usuário separadas por vírgulas. Eles aparecerão apenas no menu suspenso ou nos resultados da pesquisa quando você digitar uma consulta. Por exemplo `48d31887-5fad-4d73-a9f5-3c356e68a038,24fcbca3-c3e2-48bf-9ffc-c7f81b81483d` , exibirá apenas os dois usuários no menu suspenso quando a entrada estiver focalizada. Quando você digitar um texto de pesquisa, ele retornará resultados que corresponderão apenas aos usuários nas duas IDs de usuário.
| user-filters | userFilters | Especifica os critérios de filtro a ser usado ao consultar o ponto de extremidade dos usuários. Ele exige que `user-type` seja definido como `user` ou `contact`. Por padrão, o `user-type` é `any` e isso leva a consulta a ocorrer no bloco `people` do ponto de extremidade. Exemplo: `user-filters="startsWith(displayName,'a')"`. Esse atributo é opcional. Saiba mais sobre [o suporte para filtro em propriedades de usuário de objetos de diretório do Azure AD](/graph/aad-advanced-queries?tabs=http#user-properties).
| group-filters | groupFilters | Especifica os critérios de filtro a ser usado ao consultar o `groups` ponto de extremidade. Ele exige que `type` seja definido como `group`. Exemplo: `group-filters="startsWith(displayName,'a')"`. Esse atributo é opcional.
| people-filters | peopleFilters | Especifica os critérios de filtro a ser usado ao consultar o `people` ponto de extremidade. Ele é usado como está. Exemplo: `people-filters="jobTitle eq 'Web Marketing Manager'"`. Esse atributo é opcional. Saiba mais sobre [a filtragem e os recursos com suporte no recurso de pessoas](/graph/people-example).

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

- Usando o `selectUsersById()` método, que aceita uma matriz de [IDs](/graph/api/resources/users) de usuário do Microsoft Graph para encontrar detalhes de usuário associados para seleção.

     >**Observação:** Se nenhum usuário for encontrado para um `id`, nenhum dado será renderizado para isso `id`.

    ```javascript
    // id = Microsoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

- Usando o `selectGroupsById()` método, que aceita uma matriz de [IDs](/graph/api/resources/group) de grupo do Microsoft Graph para encontrar os grupos com usuários associados.

    ```javascript
    // groupid = Microsoft graph group "id"
    document.querySelector('mgt-people-picker').selectGroupsById(["groupid","groupid"])
    ```

## <a name="events"></a>Eventos

Os eventos a seguir são disparados do componente.

Evento | Quando é emitido | Dados personalizados | Cancelável | Bolhas | Funciona com modelo personalizado
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`selectionChanged` | O usuário adicionou ou removeu uma pessoa da lista de pessoas selecionadas/selecionadas | Matriz de pessoas selecionadas, onde uma pessoa pode ser [Graph usuário,](/graph/api/resources/user)[](/graph/api/resources/contact) `personImage` pessoa ou contato [](/graph/api/resources/person) com uma propriedade adicional que contém a URL da foto do usuário | Não | Não | Sim, a menos que você substitua o modelo padrão

Para obter mais informações sobre como lidar com eventos, consulte [eventos](../customize-components/events.md).

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

 `mgt-people-picker` oferece suporte [a vários modelos](../customize-components/templates.md) que você pode usar para substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e de `data-type` definir o valor como um dos seguintes.

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

Esse componente usa as seguintes APIs Graph Microsoft e permissões.

| Configuração | Permissão | API
| --- | ---------- | ------- |
| `group-id` set | People.Read, User.Read.All, GroupMember.Read.All | [/groups/\${groupId}/members](/graph/api/group-list-members) |
| `type` definir como `Person` ou `any` | People.Read | [/me/people](/graph/api/user-list-people) |
| `type` definir ou `Group` pesquisar usuários e `type` definir como `Group` ou `any` | Group.Read.All | [/groups](/graph/api/group-list) |
| `default-selected-user-ids` set | User.ReadBasic.All | [/users](/graph/api/user-list) |
| procurando usuários e `type` definido como `Person` ou `any` | People.Read, User.ReadBasic.All | [/me/people](/graph/api/user-list-people), [/users](/graph/api/user-list) |

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).

## <a name="cache"></a>Cache

|Armazenamento de objetos|Dados armazenados em cache|Comentários|
|---------|-----------|-------|
|`groups`|Lista de grupos|Usado quando `type` está definido como `PersonType.group`|
|`people`|Lista de pessoas|Usado quando `type` está definido como `PersonType.person` ou `PersonType.any`|
|`users`|Lista de usuários|Usado quando `groupId` especificado|

Consulte [Caching](../customize-components/cache.md) para obter mais detalhes sobre como configurar o cache.

## <a name="extend-for-more-control"></a>Estender para obter mais controle

Para cenários mais complexos ou um UX realmente personalizado, `protected render*` esse componente expõe vários métodos para substituição em extensões de componentes.

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
