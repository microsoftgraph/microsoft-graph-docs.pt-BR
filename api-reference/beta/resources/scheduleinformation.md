---
title: tipo de recurso scheduleInformation
description: 'Representa a disponibilidade de um usuário, lista de distribuição ou recurso por um período de tempo especificado. '
localization_priority: Normal
ms.openlocfilehash: 6c809b9cf600d9b620164f253d2a37e57a0f5d4d
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869488"
---
# <a name="scheduleinformation-resource-type"></a>tipo de recurso scheduleInformation

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa a disponibilidade de um usuário, lista de distribuição ou recurso (sala ou equipamento) por um período de tempo especificado.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|availabilityView |String |Representa um modo de exibição mesclado de disponibilidade de todos os `scheduleItems`itens no. O modo de exibição consiste em intervalos de tempo. A disponibilidade durante cada intervalo de tempo é indicada `0`por: = `1`livre, = `2`provisório, = `3`ocupado, = ausência temporária `4`, = trabalhando em outro lugar.|
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
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
