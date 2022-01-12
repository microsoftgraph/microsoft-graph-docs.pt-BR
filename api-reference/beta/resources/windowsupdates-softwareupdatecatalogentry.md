---
title: Tipo de recurso softwareUpdateCatalogEntry
description: Metadados para uma atualização de software que você pode aprovar para implantação.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 7103fbb2f6ed62cec5a5e530a10e190ea46067e0
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61862773"
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
|displayName|String|O nome de exibição do conteúdo. Somente leitura. Herdado de [catalogEntry](../resources/windowsupdates-catalogentry.md).|
|id|String|O identificador exclusivo para a entrada do catálogo. Somente leitura. Herdado de [catalogEntry](../resources/windowsupdates-catalogentry.md).|
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

