---
title: Tipo de recurso softwareUpdateCatalogEntry
description: Metadados para uma atualização de software que você pode aprovar para implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 3e6d0017860acbfc1371c1555279566e808da1eb
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067808"
---
# <a name="softwareupdatecatalogentry-resource-type"></a>Tipo de recurso softwareUpdateCatalogEntry

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Metadados para uma atualização de software que você pode aprovar para implantação.

Herda de [catalogEntry](../resources/windowsupdates-catalogentry.md). Tipo base [para featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) e [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md).

Esse é um tipo abstrato.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deployableUntilDateTime|DateTimeOffset|A data em que o conteúdo não está mais disponível para implantação usando o serviço. Somente leitura. Herdado de [catalogEntry](../resources/windowsupdates-catalogentry.md).|
|displayName|Cadeia de caracteres|O nome de exibição do conteúdo. Somente leitura. Herdado de [catalogEntry](../resources/windowsupdates-catalogentry.md).|
|id|Cadeia de caracteres|O identificador exclusivo para a entrada do catálogo. Somente leitura. Herdado de [catalogEntry](../resources/windowsupdates-catalogentry.md).|
|releaseDateTime|DateTimeOffset|A data de lançamento do conteúdo. Somente leitura. Herdado de [catalogEntry](../resources/windowsupdates-catalogentry.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.catalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)"
}
```

