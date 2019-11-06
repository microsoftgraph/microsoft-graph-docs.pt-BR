---
title: tipo de recurso appHostedMediaConfig
description: Pilha de mídia hospedada pelo aplicativo.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6bafd755ef2c806b703bf9ec5ac872f826de1e1c
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006772"
---
# <a name="apphostedmediaconfig-resource-type"></a>tipo de recurso appHostedMediaConfig

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
