---
title: Tipo de recurso externalItemContent
description: O conteúdo de um item indexado por meio de Pesquisa da Microsoft conexão.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: dbd84ff788cf79e212fa4031d85a6578d52343facdeee06a0bd5a4bde9af8fe7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249311"
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

