---
author: JeremyKelley
ms.date: 09/10/2017
title: Tipo de recurso File
localization_priority: Normal
description: O recurso File agrupa itens de dados relacionados a arquivos em uma única estrutura.
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 57266222e9cbc2778673172b3b96a40ca4d51df466a8c90ae784d170b7e25175
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146885"
---
# <a name="file-resource-type"></a>Tipo de recurso File

Namespace: microsoft.graph

O recurso **File** agrupa itens de dados relacionados a arquivos em uma única estrutura.

Se um [**DriveItem**](driveitem.md) tiver uma **faceta** de arquivo não nulo, o item representará um arquivo.
Além de outras propriedades, os arquivos têm um relacionamento **content**, que contém o fluxo de bytes do arquivo.

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
| hashes   | [Hashes](hashes.md) | Hash do conteúdo binário do arquivo, se houver. Somente leitura.                                                                                    |
| mimeType | cadeia de caracteres                  | O tipo MIME para o arquivo. Determinado pela lógica no servidor e pode não ser o valor fornecido quando o arquivo foi carregado. Somente leitura. |

## <a name="remarks"></a>Comentários 

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->

