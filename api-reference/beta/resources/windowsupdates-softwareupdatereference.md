---
title: Tipo de recurso softwareUpdateReference
description: Representa conteúdo de atualização específico.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 66f7f895bd3d7556ad5e3d35066236663b474f41
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067824"
---
# <a name="softwareupdatereference-resource-type"></a>Tipo de recurso softwareUpdateReference

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa conteúdo de atualização específico.

Em uma implantação, o mesmo **softwareUpdateReference** pode resultar em dispositivos que recebem revisões de atualização diferentes, mas o conteúdo é considerado contextualmente equivalente para todos os dispositivos na implantação.

Todas as referências de atualização de software existem como um dos seguintes tipos derivados: [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md).

Herda de [deployableContent](../resources/windowsupdates-deployablecontent.md). Tipo base [para windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md).

Esse é um tipo abstrato.

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.softwareUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.softwareUpdateReference"
}
```

