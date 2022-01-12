---
title: Tipo de recurso catalogEntry
description: Metadados para um conteúdo que você pode aprovar para implantação.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 2e81fd688dde08522ff59322444b1c1cd0646054
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792131"
---
# <a name="catalogentry-resource-type"></a>Tipo de recurso catalogEntry

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Metadados para um conteúdo que você pode aprovar para implantação.

Todas as entradas de catálogo existem como um dos seguintes tipos derivados: [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) e [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md).

Tipo base para [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).

Esse é um tipo abstrato.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deployableUntilDateTime|DateTimeOffset|A data em que o conteúdo não está mais disponível para implantação usando o serviço. Somente leitura.|
|displayName|String|O nome de exibição do conteúdo. Somente leitura.|
|id|String|O identificador exclusivo para a entrada do catálogo. Somente leitura.|
|releaseDateTime|DateTimeOffset|A data de lançamento do conteúdo. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.catalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.catalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)"
}
```

