---
author: JeremyKelley
ms.date: 09/10/2017
localization_priority: Normal
title: Tipo de recurso de hashes
description: O recurso hash agrupa hashes disponíveis em uma estrutura simples para um item.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bd04ff57aff3d276655a173d123f228520a77b7d548afb9f8d75d30fd6ba4e6f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243550"
---
# <a name="hashes-resource-type"></a>Tipo de recurso de hashes

Namespace: microsoft.graph

O recurso **hash** agrupa hashes disponíveis em uma estrutura simples para um item.

**Observação:** Nem todos os serviços fornecem um valor para todas as propriedades de hash listadas.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string (hex)",
  "sha1Hash": "string (hex)",
  "sha256Hash": "string (hex)",
  "quickXorHash": "string (base64)"
}
```

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo   | Descrição                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| **sha1Hash**     | String | Hash SHA1 para o conteúdo do arquivo (se disponível). Somente leitura. |
| **sha256Hash**   | Cadeia de caracteres | Hash SHA256 para o conteúdo do arquivo (se disponível). Somente leitura. |
| **crc32Hash**    | String | O valor CRC32 do arquivo em pouco endian (se disponível). Somente leitura.            |
| **quickXorHash** | String | Um hash de proprietário do arquivo que pode ser usado para determinar se o conteúdo do arquivo foi alterado (se disponível). Somente leitura. |

**Observação:** Em alguns casos, os valores de hash podem não estar disponíveis. Nesse caso, os valores de hash em um item serão atualizados depois que o item for baixado.

## <a name="remarks"></a>Comentários

No OneDrive for Business e SharePoint Server 2016, **sha1Hash** e **crc32Hash**, **e sha256Hash** não estão disponíveis.

No OneDrive Personal, o **quickXorHash** não está disponível.

Para calcular o **quickXorHash** de um arquivo, consulte o [trecho de código QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).
Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->

