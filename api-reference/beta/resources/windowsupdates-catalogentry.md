---
title: Tipo de recurso catalogEntry
description: Metadados para um conteúdo que você pode aprovar para implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 5c9766fd93c0a550556cb7f47e3275f65c238de7
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067248"
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
|displayName|Cadeia de caracteres|O nome de exibição do conteúdo. Somente leitura.|
|id|Cadeia de caracteres|O identificador exclusivo para a entrada do catálogo. Somente leitura.|
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

