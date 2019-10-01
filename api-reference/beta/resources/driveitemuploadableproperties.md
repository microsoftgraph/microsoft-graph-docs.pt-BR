---
title: tipo de recurso driveItemUploadableProperties
description: O recurso driveItemUploadableProperties representa um item sendo carregado durante a criação de uma sessão de carregamento.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f8511bba850c1d165fe9b7082b7df51900b17962
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333386"
---
# <a name="driveitemuploadableproperties-resource-type"></a>tipo de recurso driveItemUploadableProperties

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **driveItemUploadableProperties** representa um item sendo carregado durante [a criação de uma sessão de carregamento](../api/driveitem-createuploadsession.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo                              | Descrição                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|description   |String                             | Fornece uma descrição do item visível para o usuário. Leitura e gravação. Somente no OneDrive Personal.             |
|Tamanho      |Int64                              | Fornece um tamanho de arquivo esperado para executar uma verificação de cota antes do carregamento. Somente no OneDrive Personal. |
|fileSystemInfo|[fileSystemInfo](filesysteminfo.md)| Informações do sistema de arquivos no cliente. Leitura e gravação.                                                      |
|name          |String                             | O nome do item (nome do arquivo e extensão). Leitura e gravação.                                          |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.driveItemUploadableProperties",
  "baseType": null
}-->

```json
{
  "description": "String",
  "fileSize": 1024,
  "fileSystemInfo": {"@odata.type": "microsoft.graph.fileSystemInfo"},
  "name": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "driveItemUploadableProperties resource",
  "keywords": "driveItemUploadableProperties,createUploadSession",
  "section": "documentation",
  "tocPath": ""
}-->