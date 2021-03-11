---
title: Tipo de recurso synchronizationSchedule
description: Define o cronograma usado para executar um Trabalho de sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 3d0b0a45515be459c436d24f8427f7b84ef1419f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722059"
---
# <a name="synchronizationschedule-resource-type"></a>Tipo de recurso synchronizationSchedule

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define o cronograma usado para executar uma [sincronizaçãoJob](synchronization-synchronizationjob.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|expiration|DateTimeOffset|Data e hora em que esse trabalho expirará. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|interval|Duration|O intervalo entre iterações de sincronização.|
|estado|Cadeia de caracteres| Os valores possíveis são: `Active` e `Disabled`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchedule"
}-->

```json
{
  "expiration": "String (timestamp)",
  "interval": "String (duration)",
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


