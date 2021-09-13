---
title: Tipo de recurso driveItemUploadableProperties
description: O recurso driveItemUploadableProperties representa um item sendo carregado ao criar uma sessão de carregamento.
ms.localizationpriority: medium
author: JeremyKelley
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: bedbdbd67010352c3bc69a743e355efaf0514409
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067462"
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

