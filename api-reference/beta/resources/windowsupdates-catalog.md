---
title: tipo de recurso de catálogo
description: Entidade que representa o catálogo de conteúdo que você pode aprovar para implantação.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 0150875b940c9568212ae6a4acee0a0d01057feb
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61863368"
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
|id|String|Um identificador para o catálogo. Somente leitura.|

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

