---
title: Componente pessoas no microsoft Graph Toolkit
description: Você pode usar o componente `mgt-people` web para exibir um grupo de pessoas ou contatos usando suas fotos ou iniciais.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 43bc1016a462a1463437f3090361dfdd997c860c
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587102"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a>Componente pessoas no microsoft Graph Toolkit

Você pode usar o componente `mgt-people` web para exibir um grupo de pessoas ou contatos usando suas fotos ou iniciais. Por padrão, ele exibirá os contatos mais frequentes para o usuário que entrou.

Esse componente usa vários [controles mgt-person](./person.md) , mas pode ser vinculado a um conjunto de descritores de pessoas. Se houver mais pessoas para exibir do que o `show-max` valor, um número será adicionado para indicar o número de contatos adicionais.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra um grupo de pessoas exibidas usando o `mgt-people` componente. Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[Abrir este exemplo no mgt.dev](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a>Propriedades

Por padrão, o `mgt-people` componente busca eventos do `/me/people` ponto de extremidade com o `personType/class eq 'Person'` filtro para exibir usuários contatados com frequência. Você pode usar várias propriedades para alterar esse comportamento.

| Atributo | Propriedade | Descrição |
| --- | --- | --- |
| show-max | showMax | Indica o número máximo de pessoas a mostrar. O valor padrão é 3. |
| people | people | Uma matriz de pessoas para obter ou definir a lista de pessoas renderizadas pelo componente. Use essa propriedade para acessar as pessoas carregadas pelo componente. De definir esse valor para carregar suas próprias pessoas. |
| group-id | groupId | Recupera pessoas de um microsoft Graph da respectiva ID. |
| user-ids | userIds | Devido a uma matriz de usuários Graph Microsoft`ids`, o componente renderizará esses usuários.  |
| people-queries | peopleQueries | Devido a uma matriz de consultas de pessoas (nomes, upns, emails), o componente renderizará esses usuários. |
| person-card | personCard | Uma enumeração para determinar a ação do usuário necessária para ativar o painel do sub-sub-plano - `hover`, ou `click``none`. O valor padrão é `hover`. |
| show-presence | showPresence | Um Boolean para determinar se deve mostrar o selo de presença da pessoa na imagem da pessoa. |
| recurso | recurso | O recurso a ser Graph microsoft (por exemplo, `/me/people`). |
| escopos | escopos | Matriz opcional de cadeias de caracteres se estiver usando a propriedade ou um escopo delimitado por vírgula se estiver usando o atributo. O componente usará esses escopos (com um provedor com suporte) para garantir que o usuário tenha consentido com a permissão certa. |
| versão | versão | Versão da API opcional a ser usada ao fazer a solicitação GET. O padrão é `v1.0`.  |
| fallback-details| fallbackDetails| Matriz de objetos IDynamicPerson que representam uma pessoa ou várias pessoas quando nenhum usuário/pessoa/contato é encontrado no gráfico.

O exemplo a seguir define o número máximo de pessoas a mostrar.

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a>Propriedades personalizadas CSS

O `mgt-people` componente define as seguintes propriedades personalizadas CSS.

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
  --color: #000000 /* Text color */
}
```

## <a name="templates"></a>Modelos

O `mgt-people` suporte a [vários modelos que](../customize-components/templates.md) você pode usar para substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e de `data-type` definir o valor como um dos seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| `default` | `people`: lista de objetos de pessoa | O modelo padrão substitui todo o componente por seu próprio. |
| `person` | `person`: objeto person | O modelo usado para renderizar cada pessoa. |
| `overflow` | `people`: lista de objetos de pessoa <br> `max`: número de pessoas mostradas <br> `extra`: número de pessoas extras | O modelo usado para renderizar o número além do máximo à direita da lista de pessoas. |
| `no-data` | Nenhum contexto de dados é passado | O modelo usado quando nenhum dado está disponível. |
| `loading` | Nenhum contexto de dados é passado | O modelo usado enquanto o componente carrega o estado.

Os exemplos a seguir mostram como usar o `person` modelo.

```html
<mgt-people>
  <template>
    <ul><li data-for="person in people">
      <mgt-person person-query="{{ person.userPrincipalName }}"></mgt-person>
      <h3>{{ person.displayName }}</h3>
      <p>{{ person.jobTitle }}</p>
      <p>{{ person.department }}</p>
    </li></ul>
  </template>
</mgt-people>
```

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Este componente usa as seguintes APIs Graph Microsoft e permissões:

| Configuração | Permissão | API
| --- | ---------- | ------- |
| `groupId` set | GroupMember.Read.All | [/groups/\${groupId}/members](/graph/api/group-list-members) |
| `userIds` set | User.ReadBasic.All | [/users/${userId}](/graph/api/user-get) |
| `peopleQueries` set | People.Read | [/me/people](/graph/api/user-list-people) |
| `resource` set | Permissões especificadas em `scopes` | Especificado em `resource` |
| configuração padrão | People.Read | [/me/people](/graph/api/user-list-people) |
| `showPresence` set | Presence.Read.All | [/communications/getPresencesByUserId](/graph/api/cloudcommunications-getpresencesbyuserid) |

Ao usar os modelos padrão, APIs e permissões adicionais são necessárias. O modelo padrão para esse componente usa um [componente mgt-person](person.md) . Consulte sua documentação para ver a lista de permissões necessárias.

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).

## <a name="cache"></a>Cache

|Armazenamento de objetos|Dados armazenados em cache|Comentários|
|---------|-----------|-------|
|`people`|Informações sobre pessoas que coincidem com a consulta|Usado quando `resource` especificado|
|`users`|Informações sobre usuários correspondentes à consulta|Usado quando `groupId`, `userIds`ou `peopleQueries` nenhuma propriedade especificada|
|`presence`|Presença para o conjunto especificado de pessoas|Usado quando `showPresence` definido como `true`|

> [!NOTE]
> Por padrão, o `mgt-people` componente usa o [`mgt-person`](./person.md) componente para exibir informações sobre pessoas. O `mgt-person` componente baixa automaticamente e armazena em cache a foto para cada pessoa.

Para obter detalhes sobre como configurar o cache, [consulte Caching](../customize-components/cache.md).
## <a name="extend-for-more-control"></a>Estender para obter mais controle

Para cenários mais complexos ou um UX realmente personalizado, `protected render*` esse componente expõe vários métodos para substituição em extensões de componentes.

| Método | Descrição |
| - | - |
| renderLoading | Renderiza o estado de carregamento. |
| renderNoData | Renderiza o estado de dados vazio. |
| renderPeople | Renderiza uma lista de pessoas, até o `show-max` valor. |
| renderPerson | Renderiza uma pessoa individual. |
| renderOverflow | Renderiza uma representação de pessoas restantes além do `show-max` valor. |
