---
title: tipo de recurso threatAssessmentResult
description: Representa um item de resultado de avaliação de ameaça.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5e90c574ba5c89dc527f5cee236d721514834875
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519768"
---
# <a name="threatassessmentresult-resource-type"></a>tipo de recurso threatAssessmentResult

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um item de resultado de avaliação de ameaça.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|id|Cadeia de caracteres|A ID do resultado da avaliação da ameaça é um identificador global exclusivo (GUID).|
|mensagem|String|A mensagem de resultado para cada avaliação de ameaça.|
|resultType|[threatAssessmentResultType](enums.md#threatassessmentresulttype-values)|O tipo de resultado de avaliação da ameaça. Os valores possíveis são: `checkPolicy` e `rescan`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.threatAssessmentResult",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "message": "String",
  "resultType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "threatAssessmentResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
