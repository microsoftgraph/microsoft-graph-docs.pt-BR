---
title: Tipo de recurso externalItemContent
description: O conteúdo de um item indexado por meio de Pesquisa da Microsoft conexão.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4dd853ca32c918988f2f99e1f1238d9ac937da02
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467190"
---
# <a name="externalitemcontent-resource-type"></a>Tipo de recurso externalItemContent

Namespace: microsoft.graph.externalConnectors

O conteúdo de [um externalItem](externalconnectors-externalitem.md) indexado por meio de uma conexão Pesquisa da Microsoft [.](externalconnectors-externalconnection.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|type|microsoft.graph.externalConnectors.externalItemContentType|O tipo de conteúdo na propriedade value. Os valores possíveis são: `text`, `html`, `unknownFutureValue`.|
|value|Cadeia de caracteres|O conteúdo do externalItem. Obrigatório.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.externalItemContent"
}
-->
``` json
{
  "value": "String",
  "type": "String"
}
```

