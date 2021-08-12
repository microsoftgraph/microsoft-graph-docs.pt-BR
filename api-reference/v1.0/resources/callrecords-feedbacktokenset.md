---
title: Tipo de recurso feedbackTokenSet
description: O tipo feedbackTokenSet
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 054b77c64f61bd100db45ce6ed83772fd6e1fd2c0d502a4e6f578058ec8f097f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205931"
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