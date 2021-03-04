---
title: Tipo de recurso dataSource
description: A entidade dataSource é uma classe base abstrata usada para identificar fontes de conteúdo para Descoberta eDiscovery.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 2f945ba74a5576a35146ee1832f3740b537ed23b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445902"
---
# <a name="datasource-resource-type"></a>Tipo de recurso dataSource

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A entidade dataSource é uma classe base abstrata usada para identificar fontes de conteúdo para Descoberta eDiscovery.

## <a name="methods"></a>Methods

Nenhum(a)

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou **o dataSource**.|
|createdDateTime|DateTimeOffset|A data e a hora **em que dataSource** foi criado.|
|displayName|String|O nome de exibição **do dataSource**. Esse será o nome do site do SharePoint.|
|id|String| A ID do **dataSource**. Essa não é a ID do site real.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.dataSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
