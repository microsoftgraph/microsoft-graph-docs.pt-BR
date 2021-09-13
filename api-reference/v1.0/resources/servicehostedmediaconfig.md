---
title: Tipo de recurso serviceHostedMediaConfig
description: O tipo serviceHostedMediaConfig.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8179b27817627b95925e3ab84c3ea5b84b57d119
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126664"
---
# <a name="servicehostedmediaconfig-resource-type"></a>Tipo de recurso serviceHostedMediaConfig

Namespace: microsoft.graph

A mídia hospedada remotamente. Isso é herdado de [mediaConfig](mediaconfig.md).

## <a name="properties"></a>Propriedades

| Propriedade                    | Tipo                                                        | Descrição                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| preFetchMedia               | [Coleção mediaInfo](mediainfo.md)                        | A lista de mídia a ser pré-buscada.                   |


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "preFetchMedia"
  ],
  "baseType": "microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [ { "@odata.type": "microsoft.graph.mediaInfo" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "serviceHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

