---
title: enumeração fileHashType
description: Enum para tipos de arquivo de hash.
localization_priority: Normal
ms.openlocfilehash: 082fdd9cdad6c3ec1ea4e07020983ac0bac7ed65
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518377"
---
# <a name="filehashtype-enum"></a>enumeração fileHashType

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Enum para tipos de arquivo de hash.

## <a name="members"></a>Membros

|Membro|Valor|Descrição|
|:---|:---|:---|
|unknown|.0|Tipo desconhecido.|
|SHA1|-1|Tipo de hash SHA1.|
|SHA256|-2| Tipo de hash SHA256.|
|MD5|-3| Tipo de hash MD5.|
|authenticodeHash256|4*| Tipo de hash AuthenticodeHash256.|
|lsHash|.5| Tipo de hash LsHash.|
|ctph|-6| Tipo de hash CTPH.|
|peSha1|-7| Tipo de hash PESHA1.|
|peSha256|8*| Tipo de hash PESHA256.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/filehashtypeenumtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
