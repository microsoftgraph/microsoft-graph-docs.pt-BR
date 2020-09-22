---
author: JeremyKelley
description: O recurso hash agrupa hashes disponíveis em uma estrutura única para um item.
ms.date: 09/10/2017
title: Hashes
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: df3629be679b714805ea6618b7aa963214f32793
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013605"
---
# <a name="hashes-resource-type"></a>tipo de recurso hashes

Namespace: Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Agrupa hashes disponíveis em uma estrutura única para um item.

> [!NOTE]
> Nem todos os serviços fornecem um valor para todas as propriedades de hash listadas. No OneDrive for Business e no SharePoint Server 2016, **sha1Hash**, **crc32Hash**e **sha256Hash** não estão disponíveis. No OneDrive Personal, o **quickXorHash** não está disponível.

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo   | Descrição                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| **sha1Hash**     | String | Hash SHA1 para o conteúdo do arquivo (se disponível). Somente leitura. |
| **sha256Hash**   | String | O hash SHA256 para o conteúdo do arquivo (se disponível). Somente leitura. |
| **crc32Hash**    | String | O valor de CRC32 do arquivo (se disponível). Somente leitura.            |
| **quickXorHash** | String | Um hash de proprietário do arquivo que pode ser usado para determinar se o conteúdo do arquivo foi alterado (se disponível). Somente leitura. |

> **Observação:** Nos casos em que os valores de hash não estiverem disponíveis, os valores de hash em um item serão atualizados após o download do item.

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

## <a name="see-also"></a>Confira também

- Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).
- Para calcular o **quickXorHash** de um arquivo, confira o [trecho de código QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).


<!--
{
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes",
  "suppressions": []
}
-->


