---
title: tipo de recurso scheduleInformation
description: 'Representa a disponibilidade de um usuário, lista de distribuição ou recurso por um período de tempo especificado. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: harini84
ms.openlocfilehash: d503ec6241bd73492a5790f3f0f7b76a44b6245e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985815"
---
# <a name="scheduleinformation-resource-type"></a>tipo de recurso scheduleInformation

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a disponibilidade de um usuário, lista de distribuição ou recurso (sala ou equipamento) por um período de tempo especificado.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|availabilityView |String |Representa um modo de exibição mesclado de disponibilidade de todos os itens no `scheduleItems` . O modo de exibição consiste em intervalos de tempo. A disponibilidade durante cada intervalo de tempo é indicada por: `0` = livre, `1` = provisório, `2` = ocupado, `3` = ausência temporária, `4` = trabalhando em outro lugar.|
|erro |[freeBusyError](freebusyerror.md) |Informações de erro da tentativa de obter a disponibilidade do usuário, lista de distribuição ou recurso. |
|ScheduleID |String |Um endereço SMTP do usuário, lista de distribuição ou recurso, identificando uma instância do **scheduleInformation**. |
|scheduleItems |coleção [scheduleItem](scheduleitem.md) |Contém os itens que descrevem a disponibilidade do usuário ou do recurso. |
|workingHours |[workingHours](workinghours.md) |Os dias da semana e as horas de um fuso horário específico que o usuário trabalha. Eles são definidos como parte do [mailboxSettings](mailboxsettings.md)do usuário.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleInformation"
}-->

```json
{
  "availabilityView": "String",
  "error": {"@odata.type": "microsoft.graph.freeBusyError"},
  "scheduleId": "String",
  "scheduleItems": [{"@odata.type": "microsoft.graph.scheduleItem"}],
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


