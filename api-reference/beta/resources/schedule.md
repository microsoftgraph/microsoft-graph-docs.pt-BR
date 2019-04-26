---
title: tipo de recurso Schedule
description: Uma coleção de schedulingGroups, Shifts, timeOffReasons e timesOff dentro de uma equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 48b3b5c118a39442469bc6155068664fcebe0ec2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343518"
---
# <a name="schedule-resource-type"></a>tipo de recurso Schedule

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma coleção de objetos de grupo de [agendamento](schedulinggroup.md) , objetos [Shift](shift.md) , objetos [timeOffReason](timeoffreason.md) e objetos [timeOff](timeoff.md) dentro de uma [equipe](../resources/team.md). 

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar ou substituir agendamento](../api/team-put-schedule.md) | [futebol](schedule.md) | Criar ou substituir um `schedule`.|
|[Obter cronograma](../api/schedule-get.md) | [futebol](schedule.md) | Obter um `schedule`.|
|[share](../api/schedule-share.md) | Nenhum | Compartilhar um `schedule` intervalo de tempo com membros de agendamento.|

## <a name="properties"></a>Propriedades
|Nome                   |Tipo           |Descrição                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    |`string`  |A ID da tarefa `schedule`.|
| enabled               |`bool`    | Indica se o cronograma está habilitado para a equipe. Obrigatório.|
| timeZone              |`string`  | Indica o fuso horário da equipe de agendamento usando o formato de banco de dados da TZ. Obrigatório.|
| provisionStatus       |`operationStatus`    | O status do provisionamento de agendamento. Os valores possíveis são `notStarted`: `running` `completed`,, `failed`,. |
| provisionStatusCode   |`string`  | Informações adicionais sobre por que o provisionamento de agendamento falhou. |


## <a name="relationships"></a>Relacionamentos
|Nome                   |Tipo           |Descrição                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| desloca   |`collection(shift)`  | Os turnos no cronograma. |
| timesOff   |`collection(timeOff)`  | As instâncias de folgas no cronograma. |
| timeOffReasons   |`collection(timeOffReason)`  | O conjunto de motivos para uma folga no cronograma. |
| schedulingGroups   |`collection(schedulingGroup)`  | O agrupamento lógico de usuários no cronograma (geralmente por função). |


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
