---
author: JeremyKelley
description: O recurso listItemVersion representa uma versão anterior de um recurso ListItem.
ms.date: 09/17/2017
title: ListItemVersion
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 3daffc15f394139301d205c08b02b7a1a57f9d5a
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722914"
---
# <a name="listitemversion-resource-type"></a>Tipo de recurso ListItemVersion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **listItemVersion** representa uma versão anterior de um recurso [ListItem](listitem.md).

## <a name="tasks-on-listitemversion-resources"></a>Tarefas em recursos ListItemVersion

As seguintes tarefas estão disponíveis para os recursos listItemVersion.

| Tarefa comum                        | Método HTTP                                                 |
| :--------------------------------- | :---------------------------------------------------------- |
| [Listar versões][version-list]      | `GET /sites/{site-id}/items/{item-id}/versions`             |
| [Obter versão][version-get]         | `GET /sites/{site-id}/items/versions/{version-id}`          |
| [Restaurar versão][version-restore] | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource","keyProperty":"id", "@odata.type": "microsoft.graph.listItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "published": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a>Propriedades

| Propriedade                 | Tipo                                                 | Descrição                                                             |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | A ID da versão. Somente leitura.                                       |
| **lastModifiedBy**       | [IdentitySet](../resources/identityset.md)           | Identidade do usuário que modificou a versão pela última vez. Somente leitura.        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | Data e hora em que a versão foi modificada pela última vez. Somente leitura.                 |
| **published**            | [PublicationFacet](../resources/publicationfacet.md) | Indica o status de publicação desta versão específica. Somente leitura. |

## <a name="relationships"></a>Relações

A tabela a seguir define as relações que o recurso **driveItemVersion** tem com outros recursos.

| Relação | Tipo                                           | Descrição                                                              |
| :----------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| **fields**   | [FieldValueSet](../resources/fieldvalueset.md) | Uma coleção de campos e valores para esta versão do item da lista. |

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
