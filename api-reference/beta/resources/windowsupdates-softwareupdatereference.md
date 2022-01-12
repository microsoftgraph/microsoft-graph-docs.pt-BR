---
title: Tipo de recurso softwareUpdateReference
description: Representa conteúdo de atualização específico.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 9278900d85bc1ec6fc626200f0bf814dd3097b34
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860422"
---
# <a name="softwareupdatereference-resource-type"></a>Tipo de recurso softwareUpdateReference

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa conteúdo de atualização específico.

Em uma implantação, o mesmo **softwareUpdateReference** pode resultar em dispositivos que recebem revisões de atualização diferentes, mas o conteúdo é considerado contextualmente equivalente para todos os dispositivos na implantação.

Todas as referências de atualização de software existem como um dos seguintes tipos derivados: [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md) e [expeditedQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md).

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

