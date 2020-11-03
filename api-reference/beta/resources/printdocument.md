---
title: tipo de recurso de documento de documentos
description: Representa um documento que está sendo impresso.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c0bc886b618e061bee51ad82d7032737015f58ab
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849207"
---
# <a name="printdocument-resource-type"></a>tipo de recurso de documento de documentos

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um documento que está sendo impresso.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar sessão de upload](../api/printdocument-createuploadsession.md) | [uploadSession](uploadsession.md) | Criar uma sessão de carregamento para carregar com interseção intervalos de arquivos binários do **documento**. |
| [Baixar arquivo binário](../api/printdocument-get-file.md) | URL de download | Baixe o arquivo binário associado ao **documento**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O identificador do documento. Somente leitura.|
|displayName|String|O nome do documento. Somente leitura.|
|contentType|String|O tipo de conteúdo do documento (MIME). Somente leitura.|
|size|Int64|O tamanho do documento em bytes. Somente leitura.|

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
  "displayName": "String",
  "contentType": "String",
  "size": 12345
}

```


