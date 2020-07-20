---
title: Componente pessoas no Microsoft Graph Toolkit
description: Você pode usar o `mgt-people` componente da Web para exibir um grupo de pessoas ou contatos usando suas fotos ou iniciais.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 8e942ad0cca446dc8bf982249a7593b8299fe22e
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/20/2020
ms.locfileid: "45183971"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a>Componente pessoas no Microsoft Graph Toolkit

Você pode usar o `mgt-people` componente da Web para exibir um grupo de pessoas ou contatos usando suas fotos ou iniciais. Por padrão, ele exibirá os contatos mais frequentes para o usuário conectado.

Este componente usa vários controles de [pessoal de gerenciamento](./person.md) , mas pode ser vinculado a um conjunto de descritores de pessoas. Se houver mais pessoas para exibir o `show-max` valor, um número será adicionado para indicar o número de contatos adicionais.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra um grupo de pessoas exibidas usando o `mgt-people` componente. Você pode usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[Abra este exemplo em gerenciamento de. dev](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a>Propriedades

Por padrão, o `mgt-people` componente busca eventos do ponto de `/me/people` extremidade com o `personType/class eq 'Person'` filtro para exibir os usuários contatados com frequência. Você pode usar várias propriedades para alterar esse comportamento.

| Atributo | Propriedade | Descrição |
| --- | --- | --- |
| show-Max | showMax | Indica o número máximo de pessoas a serem mostradas. O valor padrão é 3. |
| people | people | Uma matriz de pessoas para obter ou definir a lista de pessoas renderizadas pelo componente. Use essa propriedade para acessar as pessoas carregadas pelo componente. Defina esse valor para carregar suas próprias pessoas. |
| ID de grupo | groupId | Recupera pessoas de um Microsoft Graph específico da respectiva ID. |
| User-IDs | userIds | Dada uma matriz de usuário do Microsoft Graph `ids` , o componente renderizará esses usuários.  |
| pessoas – consultas | peopleQueries | Dada uma matriz de consultas de pessoa (nomes, UPNs, emails), o componente renderiza esses usuários. |
| cartão de pessoa | personCard | Uma enumeração para determinar a ação do usuário necessária para ativar o painel ou o menu suspenso `hover` `click` . O valor padrão é `none`. |
| show-Presence | a presença | Um booliano para determinar se deve mostrar o crachá de presença de pessoa na imagem de pessoa. |


O exemplo a seguir define o número máximo de pessoas a serem mostradas.

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a>Propriedades personalizadas de CSS

O `mgt-people` componente define as seguintes propriedades personalizadas de CSS.

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
}
```

## <a name="templates"></a>Modelos

O `mgt-people` dá suporte a vários [modelos](../templates.md) que você pode usar para substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| `default` | `people`: lista de objetos Person | O modelo padrão substitui todo o componente pelo seu. |
| `person` | `person`: objeto Person | O modelo usado para renderizar cada pessoa. |
| `overflow` | `people`: lista de objetos Person <br> `max`: número de pessoas mostradas <br> `extra`: número de pessoas extras | O modelo usado para renderizar o número além do máximo à direita da lista de pessoas. |
| `no-data` | Nenhum contexto de dados é passado | O modelo usado quando não há dados disponíveis. |
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
| [/me/people](/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |

Ao usar os modelos padrão, são necessárias APIs e permissões adicionais. O modelo padrão para este componente usa um componente de [pessoa de gerenciamento](person.md) , que requer o seguinte.

| Recurso | Permissão |
| - | - |
| [/Users](/graph/api/user-list?view=graph-rest-1.0) | Users. ReadBasic. All |
| [/me/calendarview](/graph/api/user-list-contacts?view=graph-rest-1.0) | Contacts.Read |

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).

## <a name="extend-for-more-control"></a>Estender para mais controle

Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected render*` métodos para substituir em extensões de componente.

| Método | Descrição |
| - | - |
| renderLoading | Renderiza o estado de carregamento. |
| renderNoData | Renderiza o estado de dados vazio. |
| renderPeople | Renderiza uma lista de pessoas, até o `show-max` valor. |
| renderPerson | Renderiza uma pessoa individual. |
| renderOverflow | Renderiza uma representação de pessoas restantes além do `show-max` valor. |
