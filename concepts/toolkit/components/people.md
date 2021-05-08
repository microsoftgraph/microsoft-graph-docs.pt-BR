---
title: Componente Pessoas no microsoft graph Toolkit
description: Você pode usar o componente web para exibir um grupo de pessoas ou contatos usando `mgt-people` suas fotos ou iniciais.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 0cdade8720112dc623e617514f31ab63151b80ff
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266847"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a>Componente Pessoas no microsoft graph Toolkit

Você pode usar o componente web para exibir um grupo de pessoas ou contatos usando `mgt-people` suas fotos ou iniciais. Por padrão, ele exibirá os contatos mais frequentes para o usuário que entrou.

Esse componente usa vários [controles mgt-person,](./person.md) mas pode ser vinculado a um conjunto de descritores de pessoas. Se houver mais pessoas para exibir do que o valor, um número será adicionado para indicar o `show-max` número de contatos adicionais.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra um grupo de pessoas exibidas usando o `mgt-people` componente. Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[Abra este exemplo em mgt.dev](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a>Propriedades

Por padrão, o componente busca eventos do ponto de extremidade com o filtro para `mgt-people` `/me/people` exibir usuários `personType/class eq 'Person'` contatados com frequência. Você pode usar várias propriedades para alterar esse comportamento.

| Atributo | Propriedade | Descrição |
| --- | --- | --- |
| show-max | showMax | Indica o número máximo de pessoas a mostrar. O valor padrão é 3. |
| people | people | Uma matriz de pessoas para obter ou definir a lista de pessoas renderizadas pelo componente. Use essa propriedade para acessar as pessoas carregadas pelo componente. De definir esse valor para carregar suas próprias pessoas. |
| group-id | groupId | Recupera pessoas de um Microsoft Graph específico da respectiva ID. |
| user-ids | userIds | Devido a uma matriz de usuário do Microsoft `ids` Graph, o componente renderizará esses usuários.  |
| people-queries | peopleQueries | Devido a uma matriz de consultas de pessoas (nomes, upns, emails), o componente renderizará esses usuários. |
| person-card | personCard | Uma enumeração para determinar a ação do usuário necessária para ativar o painel do sub-sub-plano - `hover` ou `click` . O valor padrão é `none`. |
| show-presence | showPresence | Um booleano para determinar se deve mostrar o selo de presença da pessoa na imagem da pessoa. |


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
  --color: #000000 /* Text color *?
}
```

## <a name="templates"></a>Modelos

O `mgt-people` suporte a vários modelos [que](../customize-components/templates.md) você pode usar para substituir determinadas partes do componente. Para especificar um modelo, inclua um elemento dentro de um componente e de definir o `<template>` valor como um dos `data-type` seguintes.

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

Este componente usa as seguintes APIs e permissões do Microsoft Graph:

| Recurso | Permissão |
| - | - |
| [/me/people](/graph/api/user-list-people) | `People.Read` |

Ao usar os modelos padrão, APIs e permissões adicionais são necessárias. O modelo padrão para esse componente usa um [componente mgt-person,](person.md) que exige o seguinte.

| Recurso | Permissão |
| - | - |
| [/users](/graph/api/user-list) | User.ReadBasic.All |

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).

## <a name="cache"></a>Cache

|Armazenamento de objetos|Dados armazenados em cache|Comentários|
|---------|-----------|-------|
|`people`|Informações sobre pessoas que coincidem com a consulta|Usado quando `resource` especificado|
|`users`|Informações sobre usuários correspondentes à consulta|Usado quando `groupId` , ou nenhuma propriedade `userIds` `peopleQueries` especificada|
|`presence`|Presença para o conjunto especificado de pessoas|Usado quando `showPresence` definido como `true`|

> [!NOTE]
> Por padrão, o `mgt-people` componente usa o componente para exibir informações sobre [`mgt-person`](./person.md) pessoas. O `mgt-person` componente baixa automaticamente e armazena em cache a foto para cada pessoa.

Consulte [Cache para](../customize-components/cache.md) obter mais detalhes sobre como configurar o cache.
## <a name="extend-for-more-control"></a>Estender para obter mais controle

Para cenários mais complexos ou um UX realmente personalizado, esse componente expõe vários métodos para substituição `protected render*` em extensões de componentes.

| Método | Descrição |
| - | - |
| renderLoading | Renderiza o estado de carregamento. |
| renderNoData | Renderiza o estado de dados vazio. |
| renderPeople | Renderiza uma lista de pessoas, até o `show-max` valor. |
| renderPerson | Renderiza uma pessoa individual. |
| renderOverflow | Renderiza uma representação de pessoas restantes além do `show-max` valor. |
