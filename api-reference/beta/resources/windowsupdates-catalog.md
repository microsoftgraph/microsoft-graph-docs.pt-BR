---
title: tipo de recurso de catálogo
description: Entidade que representa o catálogo de conteúdo que você pode aprovar para implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 3fc0630a36d123e6c3e208838d81ee7c33c62853
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067828"
---
# <a name="catalog-resource-type"></a>tipo de recurso de catálogo

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Entidade que representa o catálogo de conteúdo que você pode aprovar para implantação.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar entradas](../api/windowsupdates-catalog-list-entries.md)|[coleção microsoft.graph.windowsUpdates.catalogEntry](../resources/windowsupdates-catalogentry.md)|Obter os [recursos catalogEntry](../resources/windowsupdates-catalogentry.md) da propriedade de navegação de entradas. Retorna **recursos catalogEntry** dos seguintes tipos derivados: [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md), [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Um identificador para o catálogo. Somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|entradas|[coleção microsoft.graph.windowsUpdates.catalogEntry](../resources/windowsupdates-catalogentry.md)|Lista o conteúdo que você pode aprovar para implantação. Somente leitura.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.catalog",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.catalog",
  "id": "String (identifier)"
}
```

