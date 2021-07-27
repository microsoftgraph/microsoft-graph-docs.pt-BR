---
title: Tipo de recurso eventMessageDetail
description: Representa o tipo base para detalhes da mensagem de evento.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: da40b7413bc52a2ec0d663e2b7e0467f0e5e06fd
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535677"
---
# <a name="eventmessagedetail-resource-type"></a>Tipo de recurso eventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Esse tipo abstrato representa detalhes de uma mensagem de evento do sistema.

As mensagens do sistema são mensagens geradas para eventos como membros adicionados a um canal, membros adicionados a um chat e a descrição da equipe atualizada.

Lista de eventos suportados

| Evento | Descrição |
| :---- | :---------- |
| [callEndedEventMessageDetail](../resources/callStartedEventMessageDetail.md) | Uma chamada foi encerrada. |
| [callRecordingEventMessageDetail](../resources/callRecordingEventMessageDetail.md) | A gravação de chamada está disponível. |
| [callStartedEventMessageDetail](../resources/callStartedEventMessageDetail.md) | Uma chamada foi iniciada. |
| [callTranscriptEventMessageDetail](../resources/callTranscriptEventMessageDetail.md) | A transcrição de chamada está disponível. |
| [channelAddedEventMessageDetail](../resources/channelAddedEventMessageDetail.md) | Um canal foi adicionado. |
| [channelDeletedEventMessageDetail](../resources/channelDeletedEventMessageDetail.md) | Um canal foi excluído. |
| [channelDescriptionUpdatedEventMessageDetail](../resources/channelDescriptionUpdatedEventMessageDetail.md) | A descrição do canal foi atualizada. |
| [channelRenamedEventMessageDetail](../resources/channelRenamedEventMessageDetail.md) | Um canal foi renomeado. |
| [channelSetAsFavoriteByDefaultEventMessageDetail](../resources/channelSetAsFavoriteByDefaultEventMessageDetail.md) | Um canal foi definido como favorito por padrão. |
| [channelUnsetAsFavoriteByDefaultEventMessageDetail](../resources/channelUnsetAsFavoriteByDefaultEventMessageDetail.md) | Um canal foi desaprisado como favorito por padrão. |
| [chatRenamedEventMessageDetail](../resources/chatRenamedEventMessageDetail.md) | Um chat foi renomeado. |
| [conversationMemberRoleUpdatedEventMessageDetail](../resources/conversationMemberRoleUpdatedEventMessageDetail.md) | A função foi atualizada para um membro. |
| [meetingPolicyUpdatedEventMessageDetail](../resources/meetingPolicyUpdatedEventMessageDetail.md) | A política de reunião foi atualizada. |
| [membersAddedEventMessageDetail](../resources/membersAddedEventMessageDetail.md) | Membros foram adicionados. |
| [membersDeletedEventMessageDetail](../resources/membersDeletedEventMessageDetail.md) | Membros foram removidos. |
| [membersJoinedEventMessageDetail](../resources/membersJoinedEventMessageDetail.md) | Membros ingressaram. |
| [membersLeftEventMessageDetail](../resources/membersLeftEventMessageDetail.md) | Membros foram embora. |
| [tabUpdatedEventMessageDetail](../resources/tabUpdatedEventMessageDetail.md) | Uma guia foi atualizada. |
| [teamArchivedEventMessageDetail](../resources/teamArchivedEventMessageDetail.md) | Uma equipe foi arquivada. |
| [teamCreatedEventMessageDetail](../resources/teamCreatedEventMessageDetail.md) | Uma equipe foi criada. |
| [teamDescriptionUpdatedEventMessageDetail](../resources/teamDescriptionUpdatedEventMessageDetail.md) | A descrição da equipe foi atualizada. |
| [teamJoiningDisabledEventMessageDetail](../resources/teamJoiningDisabledEventMessageDetail.md) | A junção de equipe foi desabilitada. |
| [teamJoiningEnabledEventMessageDetail](../resources/teamJoiningEnabledEventMessageDetail.md) | A junção de equipe foi habilitada. |
| [teamRenamedEventMessageDetail](../resources/teamRenamedEventMessageDetail.md) | Uma equipe foi renomeada. |
| [teamsAppInstalledEventMessageDetail](../resources/teamsAppInstalledEventMessageDetail.md) | Teams aplicativo foi instalado. |
| [teamsAppRemovedEventMessageDetail](../resources/teamsAppRemovedEventMessageDetail.md) | Teams aplicativo foi removido. |
| [teamsAppUpgradedEventMessageDetail](../resources/teamsAppUpgradedEventMessageDetail.md) | Teams aplicativo foi atualizado. |
| [teamUnarchivedEventMessageDetail](../resources/teamUnarchivedEventMessageDetail.md) | Uma equipe foi desarquivada. |

## <a name="properties"></a>Propriedades
Nenhum.



## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eventMessageDetail"
}
```

