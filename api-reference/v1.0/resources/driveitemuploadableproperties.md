---
title: tipo de recurso driveItemUploadableProperties
description: O recurso driveItemUploadableProperties representa um item sendo carregado durante a criação de uma sessão de carregamento.
localization_priority: Normal
author: JeremyKelley
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 1f3ef83f36af70aa2efd3cce8d0215d705114e50
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863870"
---
# <a name="driveitemuploadableproperties-resource-type"></a>tipo de recurso driveItemUploadableProperties

Namespace: microsoft.graph

Representa um item que está sendo carregado ao [criar uma sessão de carregamento](../api/driveitem-createuploadsession.md).

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
|**description**   |String                             | Fornece uma descrição do item visível para o usuário. Leitura e gravação. Somente no OneDrive Personal.             |
|**Tamanho**      |Int64                              | Fornece um tamanho de arquivo esperado para executar uma verificação de cota antes do carregamento. Somente no OneDrive Personal. |
|**fileSystemInfo**|[fileSystemInfo](filesysteminfo.md)| File system information on client. Read-write.                                                      |
|**name**          |String                             | The name of the item (filename and extension). Read-write.                                          |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "driveItemUploadableProperties resource",
  "keywords": "driveItemUploadableProperties,createUploadSession",
  "section": "documentation",
  "tocPath": ""
}-->
