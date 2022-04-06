---
title: Microsoft Teams do Selador de Canal no Microsoft Graph Toolkit
description: Você pode usar o mgt-teams-channel-picker para pesquisar canais e equipes associadas ao usuário no microsoft Graph.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 0b37085f580258abb14737384d4a3d4c0a535b45
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589258"
---
# <a name="microsoft-teams-channel-picker-component-in-the-microsoft-graph-toolkit"></a>Microsoft Teams do Selador de Canal no Microsoft Graph Toolkit

Você pode usar o componente `mgt-teams-channel-picker` para habilitar pesquisas Microsoft Teams canais associados a um usuário. O componente pode pesquisar todas as equipes que o usuário ingressou e cada canal nessas equipes. 

## <a name="example"></a>Exemplo

O exemplo a seguir mostra o `mgt-teams-channel-picker` componente. Comece a procurar um canal ou equipe para ver os resultados renderizar.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-teams-channel-picker--teams-channel-picker&source=docs" height="450"></iframe>

[Abrir este exemplo no mgt.dev](https://mgt.dev/?path=/story/components-mgt-teams-channel-picker--teams-channel-picker&source=docs)

## <a name="getting-the-selected-channel"></a>Obter o canal selecionado

Use a `selectedItem` propriedade para recuperar o canal selecionado no momento e a equipe pai. Esse valor será nulo se nenhum canal tiver sido selecionado. `selectedItem` contém duas propriedades: `channel` ([MicrosoftGraph.Channel](/graph/api/resources/channel)) e `team` ([MicrosoftGraph.Team](/graph/api/resources/team)).

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
console.log(channelPicker.selectedItem.channel);
console.log(channelPicker.selectedItem.team);
```

## <a name="selecting-a-channel"></a>Selecionar um canal

Use o `selectChannelById(channelId: string)` método para selecionar programaticamente um canal.

> **Observação:** o Teams seletor de canal só dá suporte à seleção de canal único.

```javascript
const channelPicker = document.querySelector('mgt-teams-channel-picker');
const channelId = 'some-channel-id';
channelPicker.selectChannelById(channelId);
```

> **Observação:** O canal fornecido (e a ID subsequente) deve pertencer a uma equipe que o usuário autenticado ingressou. 


## <a name="css-custom-properties"></a>Propriedades personalizadas CSS

O `mgt-teams-channel-picker` componente define as seguintes propriedades personalizadas CSS.

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

Evento | Quando é emitido | Dados personalizados | Cancelável | Bolhas | Funciona com modelo personalizado
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`selectionChanged` | Disparado quando o usuário faz uma alteração na seleção de um canal | O item selecionado no momento como `{ channel: `[channelteam](/graph/api/resources/team)[](/graph/api/resources/channel)`, team: ``}` | Não | Não | Sim

Para obter mais informações sobre como lidar com eventos, consulte [eventos](../customize-components/events.md).

## <a name="templates"></a>Modelos

`mgt-teams-channel-picker` oferece suporte [a vários modelos](../customize-components/templates.md) que você pode usar para substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e de `data-type` definir o valor como um dos seguintes.

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| loading | null: sem dados | O modelo usado para renderizar o estado do selador enquanto a solicitação à Microsoft Graph está sendo feita. |
| erro | null: sem dados| O modelo usado se a pesquisa do usuário não retornar usuários. |

O exemplo a seguir mostra como usar o `error` modelo.

```html
<mgt-teams-channel-picker>
  <template data-type="error">
    <p>Sorry, no Teams or Channels were found</p>
  </template>
</mgt-teams-channel-picker>
```

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Esse componente usa as seguintes APIs Graph Microsoft e permissões por padrão.

| API                                                                                                              | Permissão  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/me/joinedTeams](/graph/api/user-list-joinedteams)                    | User.Read.All        |
| [/teams/${id}/channels](/graph/api/channel-list) | Group.Read.All        |

Na versão 2.2, as permissões necessárias foram atualizadas para as permissões menos restritivas Teams baseadas em dados. Para evitar uma alteração de quebra, você precisa optar pelas novas permissões por meio de uma configuração global.

```ts
import {MgtTeamsChannelPicker} from "@microsoft/mgt-components";

MgtTeamsChannelPicker.config.useTeamsBasedScopes = true;
```

Com `useTeamsBasedScopes` definido como `true`, o Teams Selador de Canal usará os seguintes escopos. 

| API                                                                                                              | Permissão  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/me/joinedTeams](/graph/api/user-list-joinedteams)                    | Team.ReadBasic.All        |
| [/teams/${id}/channels](/graph/api/channel-list) | Channel.ReadBasic.All        |

Essas serão as permissões padrão na próxima grande atualização.

## <a name="authentication"></a>Autenticação

O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).

## <a name="cache"></a>Cache

O `mgt-teams-channel-picker` componente não armazena dados em cache.

## <a name="extend-for-more-control"></a>Estender para obter mais controle

Para cenários mais complexos ou um UX realmente personalizado, `protected render*` esse componente expõe vários métodos para substituição em extensões de componentes:

| Método | Descrição |
| - | - |
| renderSelected | Renderiza a equipe e o canal selecionados na caixa de entrada. |
| renderInput | Renderiza a caixa de entrada. |
| renderDropdown | Renderiza o menu suspenso. |
| renderDropdownList | Renderiza os itens no menu suspenso recursivamente. |
| renderItem | Renderiza uma equipe ou um canal na lista de menus suspensos. |
| renderHighlightedText | Renderiza o texto do canal, realçando a consulta de entrada. |
| renderLoading | Renderiza o estado suspenso de carregamento. |
| renderError | Renderiza o estado de erro suspenso. |
