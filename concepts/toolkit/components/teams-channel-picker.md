---
title: Componente seletor de canal do Microsoft Teams no Microsoft Graph Toolkit
description: Você pode usar o Requery-Teams-Channel-Picker para pesquisar canais e equipes associados ao usuário do Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: c8ade0fdfd41bde4d4a2ec643950b3faa8d24d98
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144381"
---
# <a name="microsoft-teams-channel-picker-component-in-the-microsoft-graph-toolkit"></a>Componente seletor de canal do Microsoft Teams no Microsoft Graph Toolkit

A você pode usar o `mgt-teams-channel-picker` componente para habilitar pesquisas para os canais do Microsoft Teams associados a um usuário. O componente pode pesquisar todas as equipes que o usuário ingressou e cada canal dessas equipes. 

## <a name="example"></a>Exemplo

O exemplo a seguir mostra `mgt-teams-channel-picker` o componente. Comece a pesquisar um canal ou uma equipe para ver os resultados renderizar.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-teams-channel-picker--teams-channel-picker&source=docs" height="450"></iframe>

[Abra este exemplo em gerenciamento de. dev](https://mgt.dev/?path=/story/components-mgt-teams-channel-picker--teams-channel-picker&source=docs)

## <a name="getting-the-selected-channel"></a>Obtendo o canal selecionado

Use a `selectedItem` propriedade para recuperar o canal e a equipe pai atualmente selecionados. Esse valor será NULL se nenhum canal tiver sido selecionado. `selectedItem`contém duas propriedades: `channel` ([MicrosoftGraph. Channel](/graph/api/resources/channel?view=graph-rest-1.0)) e `team` ([MicrosoftGraph. Team](/graph/api/resources/team?view=graph-rest-1.0)).

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
console.log(channelPicker.selectedItem.channel);
console.log(channelPicker.selectedItem.team);
```

## <a name="selecting-a-channel"></a>Selecionar um canal

Use o `selectChannelById(channelId: string)` método para selecionar um canal de forma programática.

> **Observação:** o seletor de canal do teams suporta apenas a seleção de canal único.

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
const channelId = 'some-channel-id';
channelPicker.selectChannelById(channelId);
```

> **Observação:** O canal fornecido (e a ID subsequente) deve pertencer a uma equipe que o usuário autenticado ingressou. 


## <a name="css-custom-properties"></a>Propriedades personalizadas de CSS

O `mgt-teams-channel-picker` componente define as seguintes propriedades personalizadas de CSS.

```css
mgt-teams-channel-picker {
    --input-border: 2px rgba(255, 255, 255, 0.5) solid; /* sets all input area border */

      /* OR individual input border sides */
    --input-border-bottom: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-right: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-left: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-top: 2px rgba(255, 255, 255, 0.5) solid;

    --input-background-color: #1f1f1f; /* input area background color */
    --input-hover-color: #008394; /* input area border hover color */
    --input-focus-color: #0f78d4; /* input area border focus color */

    --dropdown-background-color: #1f1f1f; /* channel background color */
    --dropdown-item-hover-background: #333d47; /* channel or team hover background */
    --dropdown-item-selected-background: #0F78D4; /* selected channel background color */

    --font-color: white; /* input area border focus color */
    --arrow-fill: #ffffff;
    --placeholder-focus-color: rgba(255, 255, 255, 0.8); /* place holder text focus color */
}
```

## <a name="events"></a>Eventos
| Evento | Detalhe | Descrição |
| --- | --- | --- |
| selectionChanged | O detalhe contém o item atualmente selecionado de `{channel : ` [MicrosoftGraph. Channel](/graph/api/resources/channel?view=graph-rest-1.0)`, team: `[MicrosoftGraph. Team](/graph/api/resources/team?view=graph-rest-1.0)`}` | Acionado quando o usuário faz uma alteração na seleção de um canal. |

## <a name="templates"></a>Modelos

 `mgt-teams-channel-picker`o dá suporte a vários [modelos](../templates.md) que você pode usar para substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| carregando | nulo: não há dados | O modelo usado para renderizar o estado do seletor enquanto a solicitação para o Microsoft Graph está sendo feita. |
| erro | nulo: não há dados| O modelo usado se a pesquisa de usuário não retornar nenhum usuário. |


O exemplo a seguir mostra como usar o `error` modelo.

```html
<mgt-teams-channel-picker>
  <template data-type="error">
    <p>Sorry, no Teams or Channels were found</p>
  </template>
</mgt-teams-channel-picker>
```

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Este componente usa as seguintes APIs e permissões do Microsoft Graph.

| API                                                                                                              | Permissão  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/me/joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-1.0)                    | User.Read.All        |
| [/equipes/$ {ID}/Channels](/graph/api/channel-list?view=graph-rest-1.0) | Group.Read.All        |

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).

## <a name="extend-for-more-control"></a>Estender para mais controle

Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected render*` métodos de substituição nas extensões de componente:

| Método | Descrição |
| - | - |
| renderSelected | Renderiza a equipe e canal selecionados na caixa de entrada. |
| renderInput | Renderiza a caixa de entrada. |
| renderDropdown | Renderiza o menu suspenso. |
| renderDropdownList | Renderiza os itens no menu suspenso recursivamente. |
| renderItem | Renderiza uma equipe ou um canal na lista suspensa. |
| renderHighlightedText | Renderiza o texto do canal, realçando a consulta de entrada. |
| renderLoading | Renderiza o estado do menu suspenso de carregamento. |
| renderError | Renderiza o estado de erro DropDown. |
