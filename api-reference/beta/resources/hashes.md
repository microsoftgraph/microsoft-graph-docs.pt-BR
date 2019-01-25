---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Hashes
localization_priority: Normal
ms.openlocfilehash: 551b09cee9fa662d357ee763b67ce78bea03425f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514842"
---
# <a name="hashes-resource-type"></a>Tipo de recurso de hashes

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
  "quickXorHash": "string (base64)"
}
```

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo   | Descrição                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| **sha1Hash**     | String | Hash SHA1 para o conteúdo do arquivo (se disponível). Somente leitura. |
| **crc32Hash**    | String | O valor de CRC32 do arquivo (se disponível). Somente leitura.            |
| **quickXorHash** | String | Um hash de proprietário do arquivo que pode ser usado para determinar se o conteúdo do arquivo foi alterado (se disponível). Somente leitura. |

**Observação:** Em alguns casos, os valores de hash podem não estar disponíveis. Nesse caso, os valores de hash em um item serão atualizados depois que o item for baixado.

## <a name="remarks"></a>Comentários

No OneDrive for Business e no SharePoint Server 2016, **sha1Hash** e **crc32Hash** não estão disponíveis.

No OneDrive Personal, o **quickXorHash** não está disponível.

Para calcular o **quickXorHash** de um arquivo, consulte o [trecho de código QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).


<!--
{
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes",
  "suppressions": [
    "Error: /api-reference/beta/resources/hashes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
