---
title: tipo de recurso agendar
description: Uma coleção de schedulingGroups, shifts, timeOffReasons e timesOff em uma equipe.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: b7ad28acfc03726d9645afce686b327d6d5414b9755f6f01791e21b544a5d8e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189342"
---
# <a name="schedule-resource-type"></a>tipo de recurso agendar

Namespace: microsoft.graph

Uma coleção de [objetos schedulingGroup,](schedulinggroup.md) [objetos shift,](shift.md) [objetos timeOffReason](timeoffreason.md) e [objetos timeOff](timeoff.md) dentro de uma [equipe](../resources/team.md). 

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar ou substituir agendamento](../api/team-put-schedule.md) | [cronograma](schedule.md) | Crie ou substitua um agendamento.|
|[Obter agendamento](../api/schedule-get.md) | [cronograma](schedule.md) | Obter um cronograma.|
|[Compartilhar](../api/schedule-share.md) | None | Compartilhe um intervalo de tempo de agendamento com membros de agendamento.|

## <a name="properties"></a>Propriedades
|Nome                   |Tipo           |Descrição                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    |string  |ID do agendamento.|
| enabled               |Boolean    | Indica se a agenda está habilitada para a equipe. Obrigatório.|
| timeZone              |string  | Indica o fuso horário da equipe de agendamento usando o formato de banco de dados tz. Obrigatório.|
| provisionStatus       |operationStatus    | O status do provisionamento de agendamento. Os valores possíveis `notStarted` são , , , `running` `completed` `failed` . |
| provisionStatusCode   |string  | Informações adicionais sobre por que o provisionamento de agendamento falhou. |
| timeClockEnabled                  |Booliano  | Indica se o relógio está habilitado para o agendamento.             |
| openShiftsEnabled                 |Booliano  | Indica se os turnos abertos estão habilitados para o agendamento.             | 
| swapShiftsRequestsEnabled                 |Booliano| Indica se as solicitações de turnos de troca estão habilitadas para o agendamento.             |
| offerShiftRequestsEnabled                 |Booliano  | Indica se as solicitações de turno de oferta estão habilitadas para o agendamento.             | 
| timeOffRequestsEnabled                    |Booliano | Indica se as solicitações de tempo de folga estão habilitadas para o agendamento.             | 



## <a name="relationships"></a>Relacionamentos
|Nome                   |Tipo           |Descrição                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| shifts   | [coleção shift](shift.md)  | Os turnos na agenda. |
| timesOff   |[Coleção timeOff](timeoff.md)  | As instâncias de horários de folga na agenda. |
| timeOffReasons   |[Coleção timeOffReason](timeoffreason.md)  | O conjunto de motivos para uma folga na agenda. |
| schedulingGroups   |[schedulingGroup](schedulinggroup.md) conjunto  | O agrupamento lógico de usuários na agenda (geralmente por função). |
| openshifts   |[Coleção openShift](openshift.md) | O conjunto de turnos abertos em um grupo de agendamento na agenda. |
| workforceintegrations   |[coleção workforceIntegration](workforceintegration.md)  | Uma instância de uma integração de força de trabalho por equipe com fluxo de dados de saída em notificações de alteração síncrona (para entidades com suporte). |
| swapshiftchangerequests   |[Coleção swapShiftsChangeRequest](swapshiftschangerequest.md)  | As solicitações de troca para turnos na agenda. |
| openshiftchangerequests   |[Coleção openShiftChangeRequest](openshiftchangerequest.md)  | As solicitações de turno aberto na agenda. |
| timeoffrequest   |[Coleção timeOffRequest](timeoffrequest.md)  | As solicitações de tempo de folga na agenda. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedule"
}-->

```json
{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

