---
title: tipo de recurso Schedule
description: Uma coleção de schedulingGroups, Shifts, timeOffReasons e timesOff dentro de uma equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 6bc92b18bd0529066ef9ade2df9c6ccee9628add
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895375"
---
# <a name="schedule-resource-type"></a>tipo de recurso Schedule

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma coleção de objetos de grupo de [agendamento](schedulinggroup.md) , objetos [Shift](shift.md) , objetos [timeOffReason](timeoffreason.md) e objetos [timeOff](timeoff.md) dentro de uma [equipe](../resources/team.md). 

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar ou substituir agendamento](../api/team-put-schedule.md) | [Cronograma](schedule.md) | Criar ou substituir uma agenda.|
|[Obter cronograma](../api/schedule-get.md) | [Cronograma](schedule.md) | Obter um cronograma.|
|[Compartilhar](../api/schedule-share.md) | Nenhum | Compartilhar um intervalo de tempo de agendamento com membros de agendamento.|

## <a name="properties"></a>Propriedades
|Nome                   |Tipo           |Descrição                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    |string  |ID do cronograma.|
| enabled               |Boolean    | Indica se o cronograma está habilitado para a equipe. Obrigatório.|
| timeZone              |string  | Indica o fuso horário da equipe de agendamento usando o formato de banco de dados da TZ. Obrigatório.|
| provisionStatus       |operationStatus    | O status do provisionamento de agendamento. Os valores possíveis são `notStarted`: `running` `completed`,, `failed`,. |
| provisionStatusCode   |string  | Informações adicionais sobre por que o provisionamento de agendamento falhou. |
| timeClockEnabled                  |Booliano  | Indica se o relógio de hora está habilitado para o cronograma.             |
| openShiftsEnabled                 |Booliano  | Indica se os turnos abertos estão habilitados para o cronograma.             | 
| swapShiftsRequestsEnabled                 |Booliano| Indica se as solicitações de troca alternadas estão habilitadas para o cronograma.             |
| offerShiftRequestsEnabled                 |Booliano  | Indica se as solicitações de mudança de oferta estão habilitadas para o cronograma.             | 
| timeOffRequestsEnabled                    |Booliano | Indica se as solicitações de folga estão habilitadas para o cronograma.             | 



## <a name="relationships"></a>Relacionamentos
|Nome                   |Tipo           |Descrição                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| desloca   | coleção [Shift](shift.md)  | Os turnos no cronograma. |
| timesOff   |coleção [timeOff](timeoff.md)  | As instâncias de folgas no cronograma. |
| timeOffReasons   |coleção [timeOffReason](timeoffreason.md)  | O conjunto de motivos para uma folga no cronograma. |
| schedulingGroups   |[schedulingGroup](schedulinggroup.md) conjunto  | O agrupamento lógico de usuários no cronograma (geralmente por função). |
| openshifts   |coleção [openShift](openshift.md) | O conjunto de turnos abertos em um grupo de agendamento no cronograma. |
| workforceintegrations   |coleção [workforceIntegration](workforceintegration.md)  | Uma instância de uma integração de força de funcionários por equipe com fluxo de dados de saída em notificações de alteração síncrona (para entidades com suporte). |
| swapshiftchangerequests   |coleção [swapShiftsChangeRequest](swapshiftschangerequest.md)  | As solicitações de troca de turnos no cronograma. |
| openshiftchangerequests   |coleção [openShiftChangeRequest](openshiftchangerequest.md)  | As solicitações de mudança abertas no cronograma. |
| timeoffrequest   |coleção [timeOffRequest](timeoffrequest.md)  | As solicitações de folga no cronograma. |

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
