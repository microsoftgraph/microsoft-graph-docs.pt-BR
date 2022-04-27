---
title: Tipo de recurso documentSetVersionItem
description: Representa um item que faz parte de uma versão capturada do conjunto de documentos.
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: ab6bc8f0084935e66d8fd772c6e1d13b59841012
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061168"
---
# <a name="documentsetversionitem-resource-type"></a>Tipo de recurso documentSetVersionItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um [item](../resources/listitem.md) que faz parte de um [documentSetVersion capturado](../resources/documentsetversion.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Itemid|String| O identificador exclusivo do item. |
|title|String| O título do item. |
|Versionid|String| A ID da versão do item.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.documentSetVersionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.documentSetVersionItem",
  "itemId": "String",
  "title": "String",
  "versionId": "String"
}
```

