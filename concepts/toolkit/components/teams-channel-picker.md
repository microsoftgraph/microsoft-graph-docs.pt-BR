---
title: Componente seletor de canal do Microsoft Teams no Microsoft Graph Toolkit
description: Você pode usar o Requery-Teams-Channel-Picker para pesquisar canais e equipes associados ao usuário do Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: c0b6e818f0c9c30314b5342fcfb6ef44978ec830
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660005"
---
# <a name="microsoft-teams-channel-picker-component-in-the-microsoft-graph-toolkit"></a>Componente seletor de canal do Microsoft Teams no Microsoft Graph Toolkit

A você pode usar o `mgt-teams-channel-picker` componente para habilitar pesquisas para os canais do Microsoft Teams associados a um usuário. O componente pode pesquisar todas as equipes que o usuário ingressou e cada canal dessas equipes. 

## <a name="example"></a>Exemplo

O exemplo a seguir mostra o `mgt-teams-channel-picker` componente. Comece a pesquisar um canal ou uma equipe para ver os resultados renderizar.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-teams-channel-picker--teams-channel-picker&source=docs" height="450"></iframe>

[Abra este exemplo em gerenciamento de. dev](https://mgt.dev/?path=/story/components-mgt-teams-channel-picker--teams-channel-picker&source=docs)

## <a name="getting-the-selected-channel"></a>Obtendo o canal selecionado

Use a `selectedItem` propriedade para recuperar o canal e a equipe pai atualmente selecionados. Esse valor será NULL se nenhum canal tiver sido selecionado. `selectedItem` contém duas propriedades: `channel` ([MicrosoftGraph. Channel](/graph/api/resources/channel)) e `team` ([MicrosoftGraph. Team](/graph/api/resources/team)).

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
    --input-border-color--hover: #008394; /* input area border hover color */
    --input-border-color--focus: #0f78d4; /* input area border focus color */

    --dropdown-background-color: #1f1f1f; /* channel background color */
    --dropdown-item-hover-background: #333d47; /* channel or team hover background */
    --dropdown-item-selected-background: #0F78D4; /* selected channel background color */

    --color: white; /* input area border focus color */
    --arrow-fill: #ffffff;
    --placeholder-color: #f1f1f1; /* placeholder text color */
    --placeholder-color--focus: rgba(255, 255, 255, 0.8); /* place holder text focus color */
}
```

## <a name="events"></a>Eventos
| Evento | Detalhe | Descrição |
| --- | --- | --- |
| selectionChanged | O detalhe contém o item atualmente selecionado de `{channel : ` [MicrosoftGraph. Channel](/graph/api/resources/channel) `, team: ` [MicrosoftGraph. Team](/graph/api/resources/team)`}` | Acionado quando o usuário faz uma alteração na seleção de um canal. |

## <a name="templates"></a>Modelos

 `mgt-teams-channel-picker` o dá suporte a vários [modelos](../customize-components/templates.md) que você pode usar para substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.

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
| [/me/joinedTeams](/graph/api/user-list-joinedteams)                    | User.Read.All        |
| [/equipes/$ {ID}/Channels](/graph/api/channel-list) | Group.Read.All        |

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).

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
