---
title: Tipo de recurso driveItemUploadableProperties
description: O recurso driveItemUploadableProperties representa um item sendo carregado ao criar uma sessão de carregamento.
localization_priority: Normal
author: JeremyKelley
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 39a1b68f4584e6c583213a08b203f1e3d5a7a5453b8eb1ad8708c06ef953c0c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182557"
---
# <a name="driveitemuploadableproperties-resource-type"></a>Tipo de recurso driveItemUploadableProperties

Namespace: microsoft.graph

Representa um item que está sendo carregado ao [criar uma sessão de carregamento.](../api/driveitem-createuploadsession.md)

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

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo                              | Descrição                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|**description**   |String                             | Fornece uma descrição do item visível para o usuário. Leitura e gravação. Somente no OneDrive Pessoal.             |
|**fileSize**      |Int64                              | Fornece um tamanho de arquivo esperado para executar uma verificação de cota antes de carregar. Somente no OneDrive Pessoal. |
|**fileSystemInfo**|[fileSystemInfo](filesysteminfo.md)| Informações do sistema de arquivos no cliente. Leitura e gravação.                                                      |
|**name**          |String                             | O nome do item (nome do arquivo e extensão). Leitura e gravação.                                          |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "driveItemUploadableProperties resource",
  "keywords": "driveItemUploadableProperties,createUploadSession",
  "section": "documentation",
  "tocPath": ""
}-->

