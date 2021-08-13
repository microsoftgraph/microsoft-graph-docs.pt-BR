---
title: Tipo de recurso printDocument
description: Representa um documento que está sendo impresso.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 4e2c8359b49e2154e3f107c97edf93fc64bd394837d5cf8ca8b1daa14446b857
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54169365"
---
# <a name="printdocument-resource-type"></a>Tipo de recurso printDocument

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

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
|displayName|String|O nome do documento. Somente leitura.|
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