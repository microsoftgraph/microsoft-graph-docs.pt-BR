---
title: Tipo de recurso DriveItemVersion
description: O **recurso DriveItemVersion** representa uma versão específica de um DriveItem.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: resourcePageType
ms.openlocfilehash: d015175df3f4fb91d6a91dce7cf5b10714f6d1988044e9c98c81fcd5c3dd5369
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54135257"
---
# <a name="driveitemversion-resource-type"></a>Tipo de recurso DriveItemVersion

Namespace: microsoft.graph

O recurso **DriveItemVersion** representa uma versão específica de um [DriveItem](driveitem.md).


## <a name="tasks-on-driveitemversion-resources"></a>Tarefas em recursos DriveItemVersion

As tarefas a seguir estão disponíveis para recursos driveItemVersion.

|            Tarefa comum             |         Método HTTP         |
| :--------------------------------- | :-------------------------- |
| [Listar versões][version-list]      | `GET /drive/items/{item-id}/versions`  |
| [Obter versão][version-get]         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| [Obter conteúdo][content-get]        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| [Restaurar versão][version-restore] | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

Na tabela anterior, os exemplos usam `/drive`, mas há muitas solicitações válidas.

## <a name="json-representation"></a>Representação JSON

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.driveItemVersion",
  "@type.aka&quot;: &quot;oneDrive.driveItemVersion"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" },
  "size": 12356
}
```

## <a name="properties"></a>Propriedades

|      Nome da propriedade       |                         Tipo                         |                               Descrição                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | A ID da versão. Somente leitura.                                       |
| **lastModifiedBy**       | [IdentitySet](../resources/identityset.md)           | Identidade do usuário que modificou a versão pela última vez. Somente leitura.        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | Data e hora em que a versão foi modificada pela última vez. Somente leitura.                 |
| **publication**          | [PublicationFacet](../resources/publicationfacet.md) | Indica o status de publicação desta versão específica. Somente leitura. |
| **size**                 | Int64                                                | Indica o tamanho do fluxo de conteúdo para esta versão do item.  |
| **content**              | Fluxo                                               | O fluxo de conteúdo para esta versão do item.                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->

