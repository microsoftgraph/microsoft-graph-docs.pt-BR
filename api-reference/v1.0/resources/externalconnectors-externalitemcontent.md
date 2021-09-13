---
title: Tipo de recurso externalItemContent
description: O conteúdo de um item indexado por meio de Pesquisa da Microsoft conexão.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: eade917bcee86acbc44917d8809fb26a1776bf42
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123423"
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

