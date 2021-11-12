---
title: Tipo de recurso printDocument
description: Representa um documento que está sendo impresso.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 86af8835c4452f379aadd4bfd23e87a9029045d4
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60945002"
---
# <a name="printdocument-resource-type"></a>Tipo de recurso printDocument

Namespace: microsoft.graph

Representa um documento que está sendo impresso.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [Criar sessão de carregamento](../api/printdocument-createuploadsession.md) | [uploadSession](uploadsession.md) | Criar uma sessão de carregamento para carregar iterativamente intervalos de arquivo binário do **printDocument**. |
| [Baixar arquivo binário](../api/printdocument-get-file.md) | Baixar Url | Baixe o arquivo binário associado ao **printDocument**. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador do documento. Somente leitura.|
|displayName|Cadeia de caracteres|O nome do documento. Somente leitura.|
|contentType|String|Tipo de conteúdo do documento (MIME). Somente leitura.|
|size|Int64|O tamanho do documento em bytes. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printDocument",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printDocument",
  "id": "String (identifier)",
  "displayName": "String",
  "contentType": "String",
  "size": "Integer"
}
```
