---
title: Tipo de recurso assignedPlan
description: A propriedade **assignedPlans** das entidades user e organization é uma coleção de **assignedPlan**.
localization_priority: Normal
author: jpettere
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 182ef3239437234c74945fa37483924429f2200b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958091"
---
# <a name="assignedplan-resource-type"></a>Tipo de recurso assignedPlan

Namespace: microsoft.graph

A propriedade **assignedPlans** das entidades [user](user.md) e [organization](organization.md) é uma coleção de **assignedPlan**.


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignedDateTime|DateTimeOffset|A data e a hora em que o plano foi atribuído. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|capabilityStatus|Cadeia de caracteres|Condição da atribuição de recursos. Os valores possíveis `Enabled` são , , , , `Warning` `Suspended` `Deleted` `LockedOut` . Consulte [uma descrição detalhada](#capabilitystatus-values) de cada valor.|
|service|Cadeia de caracteres|O nome do serviço; por exemplo, "Exchange".|
|servicePlanId|Guid|Um GUID que identifica o plano de serviço.|


### <a name="capabilitystatus-values"></a>valores de capabilityStatus

| Member | Descrição  |
|:---------------|:--------|
| Habilitado | Disponível para uso normal. |
| Aviso | Disponível para uso normal, mas está em um período de carência. |
| Suspenso | Indisponível, mas todos os dados associados à funcionalidade devem ser preservados. |
| Excluída | Indisponíveis e quaisquer dados associados à funcionalidade podem ser excluídos. |
| LockedOut | Indisponível para todos os administradores e usuários, mas todos os dados associados à funcionalidade devem ser preservados. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedPlan"
}-->

```json
{
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "string",
  "service": "string",
  "servicePlanId": "guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

