---
title: Tipo de recurso eventMessageDetail
description: Representa o tipo base para detalhes da mensagem de evento.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 70151180d99ed4d83b1a36dfbb804c65e1966ec0
ms.sourcegitcommit: 191b797b178f40fde6419719fcd75461e6869401
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2022
ms.locfileid: "66118351"
---
# <a name="eventmessagedetail-resource-type"></a>Tipo de recurso eventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Esse tipo abstrato representa detalhes de uma mensagem de evento do sistema.

As mensagens do sistema são mensagens geradas para eventos como membros adicionados a um canal, membros adicionados a um chat e descrição da equipe atualizada.

A tabela a seguir lista os eventos com suporte.

| Evento | Descrição |
| :---- | :---------- |
| [callEndedEventMessageDetail](../resources/callEndedEventMessageDetail.md) | Uma chamada foi encerrada. |
| [callRecordingEventMessageDetail](../resources/callRecordingEventMessageDetail.md) | A gravação de chamada está disponível. |
| [callStartedEventMessageDetail](../resources/callStartedEventMessageDetail.md) | Uma chamada foi iniciada. |
| [callTranscriptEventMessageDetail](../resources/callTranscriptEventMessageDetail.md) | A transcrição de chamadas está disponível. |
| [channelAddedEventMessageDetail](../resources/channelAddedEventMessageDetail.md) | Um canal foi adicionado. |
| [channelDeletedEventMessageDetail](../resources/channelDeletedEventMessageDetail.md) | Um canal foi excluído. |
| [channelDescriptionUpdatedEventMessageDetail](../resources/channelDescriptionUpdatedEventMessageDetail.md) | A descrição do canal foi atualizada. |
| [channelRenamedEventMessageDetail](../resources/channelRenamedEventMessageDetail.md) | Um canal foi renomeado. |
| [channelSetAsFavoriteByDefaultEventMessageDetail](../resources/channelSetAsFavoriteByDefaultEventMessageDetail.md) | Um canal foi definido como favorito por padrão. |
| [channelUnsetAsFavoriteByDefaultEventMessageDetail](../resources/channelUnsetAsFavoriteByDefaultEventMessageDetail.md) | Um canal foi desmarcado como favorito por padrão. |
| [chatRenamedEventMessageDetail](../resources/chatRenamedEventMessageDetail.md) | Um chat foi renomeado. |
| [conversationMemberRoleUpdatedEventMessageDetail](../resources/conversationMemberRoleUpdatedEventMessageDetail.md) | A função foi atualizada para um membro. |
| [meetingPolicyUpdatedEventMessageDetail](../resources/meetingPolicyUpdatedEventMessageDetail.md) | A política de reunião foi atualizada. |
| [membersAddedEventMessageDetail](../resources/membersAddedEventMessageDetail.md) | Membros foram adicionados. |
| [membersDeletedEventMessageDetail](../resources/membersDeletedEventMessageDetail.md) | Membros foram removidos. |
| [membersJoinedEventMessageDetail](../resources/membersJoinedEventMessageDetail.md) | Membros ingressaram. |
| [membersLeftEventMessageDetail](../resources/membersLeftEventMessageDetail.md) | Os membros foram embora. |
| [messagePinnedEventMessageDetail](../resources/messagepinnedeventmessagedetail.md) | Uma mensagem foi fixada. |
| [messageUnpinnedEventMessageDetail](../resources/messageunpinnedeventmessagedetail.md) | Uma mensagem foi desafixada. |
| [tabUpdatedEventMessageDetail](../resources/tabUpdatedEventMessageDetail.md) | Uma guia foi atualizada. |
| [teamArchivedEventMessageDetail](../resources/teamArchivedEventMessageDetail.md) | Uma equipe foi arquivada. |
| [teamCreatedEventMessageDetail](../resources/teamCreatedEventMessageDetail.md) | Uma equipe foi criada. |
| [teamDescriptionUpdatedEventMessageDetail](../resources/teamDescriptionUpdatedEventMessageDetail.md) | A descrição da equipe foi atualizada. |
| [teamJoiningDisabledEventMessageDetail](../resources/teamJoiningDisabledEventMessageDetail.md) | O ingresso em equipe foi desabilitado. |
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

