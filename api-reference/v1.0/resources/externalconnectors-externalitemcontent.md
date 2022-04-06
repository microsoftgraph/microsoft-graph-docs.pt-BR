---
title: Tipo de recurso externalItemContent
description: O conteúdo de um item indexado por meio de uma Pesquisa da Microsoft conexão.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 35a410a12608ad43f75196b41b3d747e56b10d59
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/17/2022
ms.locfileid: "63560023"
---
# <a name="externalitemcontent-resource-type"></a>Tipo de recurso externalItemContent

Namespace: microsoft.graph.externalConnectors

O conteúdo de [um externalItem](externalconnectors-externalitem.md) indexado por meio de Pesquisa da Microsoft [conexão](externalconnectors-externalconnection.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|type|microsoft.graph.externalConnectors.externalItemContentType|O tipo de conteúdo na propriedade value. Os valores possíveis são: `text`, `html`, `unknownFutureValue`. Esses são os tipos de conteúdo que o indexador suporta e não os tipos de extensão de arquivo permitidos.|
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

