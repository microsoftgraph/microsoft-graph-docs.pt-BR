---
title: Tipo de recurso teamworkContentCameraConfiguration
description: Representa detalhes de configuração de uma câmera de conteúdo conectada a um dispositivo Microsoft Teams habilitado para Microsoft Teams.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 00db0e0fbd61afe3f113a903d60aeb5bf02f6581
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262294"
---
# <a name="teamworkcontentcameraconfiguration-resource-type"></a>Tipo de recurso teamworkContentCameraConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa detalhes de configuração de uma câmera de conteúdo conectada a um dispositivo Microsoft Teams habilitado [para Microsoft Teams.](../resources/teamworkdevice.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isContentCameraInverted|Booliano|`True` se a câmera de conteúdo for invertida.|
|isContentCameraOptional|Booliano|`True` se a câmera de conteúdo for opcional.|
|isContentEnhancementEnabled|Booliano|`True` se o aprimoramento de conteúdo estiver habilitado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkContentCameraConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkContentCameraConfiguration",
  "isContentCameraInverted": "Boolean",
  "isContentCameraOptional": "Boolean",
  "isContentEnhancementEnabled": "Boolean"
}
```

