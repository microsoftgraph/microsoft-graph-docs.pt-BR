---
title: Tipo de recurso channelIdentity
description: Representa a identidade de um canal no Microsoft Teams.
author: Kanaka
doc_type: resourcePageType
localization_priority: Normal
ms.prod: teamwork
ms.openlocfilehash: 866469745a4dd3aaf7b22c2a6710e327992e9fee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952800"
---
# <a name="channelidentity-resource-type"></a>Tipo de recurso channelIdentity

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Contém informações básicas de identificação sobre um canal no Microsoft Teams.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|channelId|cadeia de caracteres|  A identidade do canal no qual a mensagem foi postada.|
|teamId|cadeia de caracteres|  A identidade da equipe na qual a mensagem foi postada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    
  ],
  "@odata.type": "microsoft.graph.channelIdentity"
}-->

```json
{
  "channelId": "string",
  "teamId": "string",
  
}
```

<!-- uuid: 4DFA000D-1A5F-4299-B3DD-835E4DD2F3BF
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel identity  resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
