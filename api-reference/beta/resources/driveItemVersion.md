---
author: JeremyKelley
description: O recurso DriveItemVersion representa uma versão específica de um DriveItem.
ms.date: 09/17/2017
title: DriveItemVersion
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: d6f2245fe02657d883d1e6646ac6ff6fce0187ea
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723159"
---
# <a name="driveitemversion-resource-type"></a>Tipo de recurso DriveItemVersion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **DriveItemVersion** representa uma versão específica de um [DriveItem](driveitem.md).

## <a name="tasks-on-driveitemversion-resources"></a>Tarefas em recursos DriveItemVersion

As tarefas a seguir estão disponíveis para recursos driveItemVersion.

| Tarefa comum                        | Método HTTP                                                        |
| :--------------------------------- | :----------------------------------------------------------------- |
| [Listar versões][version-list]      | `GET /drive/items/{item-id}/versions`                              |
| [Obter versão][version-get]         | `GET /drive/items/{item-id}/versions/{version-id}`                 |
| [Obter conteúdo][content-get]        | `GET /drive/items/{item-id}/versions/{version-id}/content`         |
| [Restaurar versão][version-restore] | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

Na tabela anterior, os exemplos usam `/drive`, mas há muitas solicitações válidas.

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource","keyProperty":"id", "@odata.type": "microsoft.graph.driveItemVersion", "@type.aka": "oneDrive.driveItemVersion" } -->

```json
{
  "content": {"@odata.type": "Edm.Stream"},
  "id": "string",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": {"@odata.type": "microsoft.graph.publicationFacet"},
  "size": 12356
}
```

## <a name="properties"></a>Propriedades

| Propriedade                 | Tipo                                                 | Descrição                                                             |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | A ID da versão. Somente leitura.                                       |
| **lastModifiedBy**       | [IdentitySet](../resources/identityset.md)           | Identidade do usuário que modificou a versão pela última vez. Somente leitura.        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | Data e hora em que a versão foi modificada pela última vez. Somente leitura.                 |
| **publication**          | [PublicationFacet](../resources/publicationfacet.md) | Indica o status de publicação desta versão específica. Somente leitura. |
| **size**                 | Int64                                                | Indica o tamanho do fluxo de conteúdo para esta versão do item.  |

## <a name="relationships"></a>Relações

A tabela a seguir define as relações que o recurso **driveItemVersion** tem com outros recursos.

| Relação | Tipo   | Descrição                        |
| :----------- | :----- | :--------------------------------- |
| **content**  | Fluxo | O fluxo de conteúdo da versão. |

<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": []
}
-->
