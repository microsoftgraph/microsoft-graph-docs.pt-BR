---
title: tipo de recurso appHostedMediaConfig
description: Pilha de mídia hospedada pelo aplicativo.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 70bd631631dd5d4fdebe55d379ea61f98fba19a6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508307"
---
# <a name="apphostedmediaconfig-resource-type"></a>tipo de recurso appHostedMediaConfig

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Pilha de mídia hospedada pelo aplicativo.

## <a name="properties"></a>Propriedades

| Propriedade                          | Tipo    | Descrição                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| blob                              | String  | O blob de configuração de mídia gerado pelo agente de mídia inteligente.    |
| removeFromDefaultAudioGroup       | Booliano | Remover o áudio do grupo de áudio padrão                       |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.appHostedMediaConfig"
}-->
```json
{
  "blob": "String",
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
