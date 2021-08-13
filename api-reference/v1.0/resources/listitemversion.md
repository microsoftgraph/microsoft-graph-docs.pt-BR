---
title: Tipo de recurso ListItemVersion
description: O recurso **listItemVersion** representa uma versão anterior de um recurso ListItem.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: resourcePageType
ms.openlocfilehash: 59f7672c0569c3965bf7b473ca1584f77fc4694bd0a06dfc46374d4f7c8826ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163716"
---
# <a name="listitemversion-resource-type"></a>Tipo de recurso ListItemVersion

Namespace: microsoft.graph

O recurso **listItemVersion** representa uma versão anterior de um recurso [ListItem](listitem.md).

## <a name="tasks-on-listitemversion-resources"></a>Tarefas em recursos ListItemVersion

As seguintes tarefas estão disponíveis para os recursos listItemVersion.

|            Tarefa comum             |         Método HTTP         |
| :--------------------------------- | :-------------------------- |
| [Listar versões][version-list]      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| [Obter versão][version-get]         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| [Restaurar versão][version-restore] | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a>Representação JSON

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.listItemVersion",
  "@type.aka&quot;: &quot;oneDrive.baseItemVersion"
}-->

```json
{
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "published": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a>Propriedades

|      Nome da propriedade       |                         Tipo                         |                               Descrição                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | A ID da versão. Somente leitura.                                       |
| **lastModifiedBy**       | [IdentitySet](../resources/identityset.md)           | Identidade do usuário que modificou a versão pela última vez. Somente leitura.        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | Data e hora em que a versão foi modificada pela última vez. Somente leitura.                 |
| **published**            | [PublicationFacet](../resources/publicationfacet.md) | Indica o status de publicação desta versão específica. Somente leitura. |


## <a name="relationships"></a>Relações

A tabela a seguir define as relações que o recurso **driveItemVersion** tem com outros recursos.

| Nome da relação |                      Tipo                      |                               Descrição                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| **fields**        | [FieldValueSet](../resources/fieldvalueset.md) | Uma coleção de campos e valores para esta versão do item da lista. |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->

