---
author: JeremyKelley
ms.date: 09/10/2017
title: Tipo de recurso File
ms.localizationpriority: medium
description: O recurso File agrupa itens de dados relacionados a arquivos em uma única estrutura.
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f97f037916dabd91653b785add53cbb9cb38afdd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036505"
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

