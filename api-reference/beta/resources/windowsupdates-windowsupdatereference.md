---
title: Tipo de recurso windowsUpdateReference
description: Representa o conteúdo Windows 10 de atualização específica.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a75f1afe1c2689760848283bf078b957bb8739ba
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067226"
---
# <a name="windowsupdatereference-resource-type"></a>Tipo de recurso windowsUpdateReference

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o conteúdo Windows 10 de atualização específica.

Em uma implantação, a mesma Windows de atualização pode resultar em dispositivos que recebem revisões de atualização diferentes, mas o conteúdo é considerado contextually equivalente para todos os dispositivos na implantação.

Todas Windows de atualização existem como um dos seguintes tipos derivados: [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md) e [expeditedQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md).

Herda de [softwareUpdateReference](../resources/windowsupdates-softwareupdatereference.md). Tipo base [para featureUpdateReference](../resources/windowsupdates-featureupdatereference.md) [e qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).

Esse é um tipo abstrato.

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.windowsUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.windowsUpdateReference"
}
```

