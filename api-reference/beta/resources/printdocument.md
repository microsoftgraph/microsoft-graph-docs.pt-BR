---
title: tipo de recurso de documento de documentos
description: Representa um documento que está sendo impresso.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bfe1badffdd675c68678e1f8463d09aee2af1217
ms.sourcegitcommit: 3c0fa2d13ede0fdfa66d966d4ec32cb468c3befa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48273680"
---
# <a name="printdocument-resource-type"></a>tipo de recurso de documento de documentos

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um documento que está sendo impresso.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [uploadData](../api/printdocument-uploaddata.md) | Nenhum | Carregar um único segmento binário do **documento**. |
| [Baixar arquivo binário](../api/printdocument-get-file.md) | URL de download | Baixe o arquivo binário associado ao **documento**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O identificador do documento. Somente leitura.|
|displayName|String|O nome do documento. Somente leitura.|
|contentType|String|O tipo de conteúdo do documento (MIME). Somente leitura.|
|size|Int64|O tamanho do documento em bytes. Somente leitura.|
|configuration|[printerDocumentConfiguration](printerdocumentconfiguration.md) |Um grupo de configurações que uma impressora deve usar para imprimir um documento. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printDocument"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "mimeType": "String",
  "sizeInBytes": 12345,
  "documentConfiguration": {
    "pageRanges": [ {"@odata.type": "microsoft.graph.printPageRange"} ],
    "printQuality": "String",
    "printResolutionInDpi": 123456,
    "feedDirection": "String",
    "orientation": "String",
    "duplexConfiguration": "String",
    "copies": 123456,
    "colorConfiguration": "String",
  }
}

```


