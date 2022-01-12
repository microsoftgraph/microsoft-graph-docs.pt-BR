---
title: Tipo de recurso windowsUpdateReference
description: Representa o conteúdo Windows 10 de atualização específica.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a25cc6995979922ed2e7a8fb8e7f74350dec71c5
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791991"
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

