---
author: JeremyKelley
description: O recurso File agrupa itens de dados relacionados a arquivos em uma única estrutura.
ms.date: 09/10/2017
title: Arquivo
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: aaf662575552a37d28e9a429297f8f58f825b6e6
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291157"
---
# <a name="file-resource-type"></a>Tipo de recurso File

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **File** agrupa itens de dados relacionados a arquivos em uma única estrutura.

Se um [**DriveItem**](driveitem.md) tiver uma faceta **file** não nula, o item representa um arquivo. Além de outras propriedades, os arquivos têm um relacionamento **content**, que contém o fluxo de bytes do arquivo.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.file"
}-->

```json
{
  "hashes": {"@odata.type": "microsoft.graph.hashes"},
  "mimeType": "string"
}
```

## <a name="properties"></a>Propriedades

| Propriedade | Tipo                    | Descrição                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| hashes   | [hashes](hashes.md) | Hash do conteúdo binário do arquivo, se houver. Somente leitura.                                                                                    |
| mimeType | cadeia de caracteres                  | O tipo MIME para o arquivo. Determinado pela lógica no servidor e pode não ser o valor fornecido quando o arquivo foi carregado. Somente leitura. |

## <a name="remarks"></a>Comentários 

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).

<!--
{
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File",
  "suppressions": []
}
-->
