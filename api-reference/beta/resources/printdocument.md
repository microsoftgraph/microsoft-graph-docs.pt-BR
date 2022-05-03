---
title: Tipo de recurso printDocument
description: Representa um documento que está sendo impresso.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 55eaea78c960596beab18682209acad9522c00d1
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176904"
---
# <a name="printdocument-resource-type"></a>Tipo de recurso printDocument

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um documento que está sendo impresso.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar sessão de upload](../api/printdocument-createuploadsession.md) | [uploadSession](uploadsession.md) | Crie uma sessão de upload para carregar iterativamente intervalos de arquivo binário do **printDocument**. |
| [Baixar arquivo binário](../api/printdocument-get-file.md) | Download Url | Baixe o arquivo binário associado ao **printDocument**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|O identificador do documento. Somente leitura.|
|displayName|Cadeia de caracteres|O nome do documento. Somente leitura.|
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


