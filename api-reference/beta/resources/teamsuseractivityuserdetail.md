---
title: Tipo de recurso teamsUserActivityUserDetail
description: Representa detalhes sobre a atividade do usuário do Microsoft Teams por usuário.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4afa7f17acac13eaa1c517953517fcfbe344aaa7
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766431"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>Tipo de recurso teamsUserActivityUserDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa detalhes sobre a atividade do usuário do Microsoft Teams por usuário.

## <a name="properties"></a>Propriedades

| Propriedade                                 | Tipo              | Descrição                                                  |
| :--------------------------------------- | :---------------- | ------------------------------------------------------------ |
| reportRefreshDate                        | Data              | A data mais recente do conteúdo.                              |
| userPrincipalName                        | String            | O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. |
| isLicensed                               | Booliano           | Se o usuário recebeu uma licença do Teams.          |
| lastActivityDate                         | Data              | A última data em que o usuário participou de uma atividade do Microsoft Teams. |
| isDeleted                                | Booliano           | Se esse usuário foi excluído ou excluído.          |
| deletedDate                              | Data              | A data em que a operação de exclusão aconteceu. O valor padrão é "null" quando o usuário não foi excluído. |
| assignedProducts                         | Coleção de cadeias de caracteres | Produtos aos que o usuário atribuiu.                             |
| teamChatMessageCount                     | Int64             | O número de mensagens exclusivas que o usuário postou em um chat de equipe. |
| privateChatMessageCount                  | Int64             | O número de mensagens exclusivas que o usuário postou em um chat privado. |
| callCount                                | Int64             | O número de chamadas 1:1 nas que o usuário participou.       |
| meetingCount                             | Int64             | O número de reuniões online em que o usuário participou. |
| meetingsOrganizedCount                   | Int64             | A soma de reuniões agendadas, recorrentes, ad hoc e não classificadas que um usuário organizou. |
| meetingsAttendedCount                    | Int64             | A soma das reuniões agendadas, recorrentes, ad hoc e não classificadas em que um usuário participou. |
| adHocMeetingsOrganizedCount              | Int64             | O número de reuniões ad hoc que um usuário organizou.              |
| adHocMeetingsAttendedCount               | Int64             | O número de reuniões ad hoc que um usuário participou.        |
| scheduledOneTimeMeetingsOrganizedCount   | Int64             | O número de reuniões agendadas única que um usuário organizou.  |
| scheduledOneTimeMeetingsAttendedCount    | Int64             | O número das reuniões agendadas de uma vez em que um usuário participou. |
| scheduledRecurringMeetingsOrganizedCount | Int64             | O número de reuniões recorrentes que um usuário organizou.           |
| scheduledRecurringMeetingsAttendedCount  | Int64             | O número de reuniões recorrentes que um usuário participou. |
| audioDuration                            | Duration          | Duração do áudio em que o usuário participou.                     |
| videoDuration                            | Duration          | Duração do vídeo em que o usuário participou.                     |
| screenShareDuration                      | Duration          | Duração de compartilhamento de tela em que o usuário participou.            |
| hasOtherAction                           | Booliano           | O Usuário está ativo, mas realizou outras atividades que não os tipos de ação expostos oferecidos no relatório (enviando ou respondendo a mensagens de canal e mensagens de chat, agendando ou participando de chamadas e reuniões 1:1). Exemplos de ações são quando um usuário altera o status do Teams ou a mensagem de status do Teams ou abre uma postagem mensagem de canal, mas não responde. |
| reportPeriod                             | String            | O número de dias que o relatório aborda.                        |

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isLicensed": true, 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "assignedProducts": ["String"],
  "teamChatMessageCount": 1024, 
  "privateChatMessageCount": 1024, 
  "callCount": 1024, 
  "meetingCount": 1024, 
  "meetingsOrganizedCount": 1024, 
  "meetingsAttendedCount": 1024, 
  "adHocMeetingsOrganizedCount": 1024, 
  "adHocMeetingsAttendedCount": 1024, 
  "scheduledOneTimeMeetingsOrganizedCount": 1024, 
  "scheduledOneTimeMeetingsAttendedCount": 1024, 
  "scheduledRecurringMeetingsOrganizedCount": 1024, 
  "scheduledRecurringMeetingsAttendedCount": 1024, 
  "audioDuration": "Duration", 
  "videoDuration": "Duration", 
  "screenShareDuration": "Duration", 
  "hasOtherAction": true, 
  "reportPeriod": "String"
}
```


