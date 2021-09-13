---
title: Tipo de recurso feedbackTokenSet
description: O tipo feedbackTokenSet
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2422c0d00e85d1cb6d7d6cf5934d4e498e796013
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59025556"
---
# <a name="feedbacktokenset-resource-type"></a>Tipo de recurso feedbackTokenSet

Namespace: microsoft.graph.callRecords

Esse é um _tipo aberto que_ representa o conjunto de tokens de feedback fornecidos pelo usuário deste ponto de extremidade para a Sessão. Este é um conjunto de propriedades Boolean. Os nomes de propriedade não devem ser confiados, pois eles podem mudar dependendo de quais tokens são oferecidos ao usuário.

## <a name="properties"></a>Propriedades

Os nomes de propriedades explícitos não serão documentados, pois os nomes de token de feedback podem mudar, portanto, esse é um [tipo aberto.](/aspnet/web-api/overview/odata-support-in-aspnet-web-api/odata-v4/use-open-types-in-odata-v4)

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.feedbackTokenSet",
  "baseType": null
}-->

```json
{
  "DistortedSpeech": true,
  "ElectronicFeedback": false,
  "BackgroundNoise": true,
  "MuffledSpeech": true,
  "Echo": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "feedbackTokenSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
