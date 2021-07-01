---
title: Tipo de recurso driveItemUploadableProperties
description: O recurso driveItemUploadableProperties representa um item sendo carregado ao criar uma sessão de carregamento.
localization_priority: Normal
author: JeremyKelley
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 6c00270f1e86e2bb8f44af36c6c514c9b80a647d
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236205"
---
# <a name="driveitemuploadableproperties-resource-type"></a>Tipo de recurso driveItemUploadableProperties

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **recurso driveItemUploadableProperties** representa um item que está sendo carregado ao [criar uma sessão de carregamento.](../api/driveitem-createuploadsession.md)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo                              | Descrição                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|description   |String                             | Fornece uma descrição do item visível para o usuário. Leitura e gravação. Somente no OneDrive Pessoal.             |
|driveItemSource| [driveItemSource](driveItemSource.md)              | Informações sobre a fonte do item da unidade. Leitura e gravação. Somente em OneDrive for Business e SharePoint.  |
|fileSize      |Int64                              | Fornece um tamanho de arquivo esperado para executar uma verificação de cota antes de carregar. Somente no OneDrive Pessoal. |
|fileSystemInfo|[fileSystemInfo](filesysteminfo.md)| Informações do sistema de arquivos no cliente. Leitura e gravação.                                                      |
|mediaSource  | [mediaSource](mediaSource.md)                    | Informações de origem de mídia. Leitura e gravação. Somente em OneDrive for Business e SharePoint.                 |
|nome          |String                             | O nome do item (nome do arquivo e extensão). Leitura e gravação.                                          |

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

