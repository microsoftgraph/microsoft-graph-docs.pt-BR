---
title: Tipo de recurso softwareUpdateReference
description: Representa conteúdo de atualização específico.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 13e71a5b08100a74884ae0f4f69b69b86bec9b2c
ms.sourcegitcommit: 94dc71a6d4fbdc46f2681a1add13416bc9b4a6e9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2021
ms.locfileid: "60115309"
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

