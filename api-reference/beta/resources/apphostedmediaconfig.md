---
title: tipo de recurso appHostedMediaConfig
description: Pilha de mídia hospedada pelo aplicativo.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0cb34d0673404c90607a8f1ac442ca1b7c504ce9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339178"
---
# <a name="apphostedmediaconfig-resource-type"></a>tipo de recurso appHostedMediaConfig

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Pilha de mídia hospedada pelo aplicativo.

## <a name="properties"></a>Propriedades

| Propriedade                          | Tipo    | Descrição                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| blob                              | String  | O blob de configuração de mídia gerado pelo agente de mídia inteligente.    |
| removeFromDefaultAudioGroup       | Boolean | Remover o áudio do grupo de áudio padrão                       |

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
