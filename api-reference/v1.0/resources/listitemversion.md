---
title: Tipo de recurso ListItemVersion
description: O recurso **listItemVersion** representa uma versão anterior de um recurso ListItem.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 6e21be59b71a8f348931603c799ebbbe225e5d3f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951842"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="8082f-103">Tipo de recurso ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="8082f-103">ListItemVersion resource type</span></span>

<span data-ttu-id="8082f-104">O recurso **listItemVersion** representa uma versão anterior de um recurso [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="8082f-104">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="8082f-105">Tarefas em recursos ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="8082f-105">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="8082f-106">As seguintes tarefas estão disponíveis para os recursos listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="8082f-106">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="8082f-107">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="8082f-107">Common task</span></span>             |         <span data-ttu-id="8082f-108">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="8082f-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="8082f-109">[Versões de lista][version-list]</span><span class="sxs-lookup"><span data-stu-id="8082f-109">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="8082f-110">[Obter versão][version-get]</span><span class="sxs-lookup"><span data-stu-id="8082f-110">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="8082f-111">[Restaurar versão][version-restore]</span><span class="sxs-lookup"><span data-stu-id="8082f-111">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="8082f-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8082f-112">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.listItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
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

## <a name="properties"></a><span data-ttu-id="8082f-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8082f-113">Properties</span></span>

|      <span data-ttu-id="8082f-114">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="8082f-114">Property name</span></span>       |                         <span data-ttu-id="8082f-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="8082f-115">Type</span></span>                         |                               <span data-ttu-id="8082f-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="8082f-116">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="8082f-117">**id**</span><span class="sxs-lookup"><span data-stu-id="8082f-117">**id**</span></span>                   | <span data-ttu-id="8082f-118">string</span><span class="sxs-lookup"><span data-stu-id="8082f-118">string</span></span>                                               | <span data-ttu-id="8082f-119">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="8082f-119">The ID of the version.</span></span> <span data-ttu-id="8082f-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8082f-120">Read-only.</span></span>                                       |
| <span data-ttu-id="8082f-121">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="8082f-121">**lastModifiedBy**</span></span>       | [<span data-ttu-id="8082f-122">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="8082f-122">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="8082f-123">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8082f-123">Identity of the user which last modified the version.</span></span> <span data-ttu-id="8082f-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8082f-124">Read-only.</span></span>        |
| <span data-ttu-id="8082f-125">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="8082f-125">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="8082f-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8082f-126">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="8082f-127">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8082f-127">Date and time the version was last modified.</span></span> <span data-ttu-id="8082f-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8082f-128">Read-only.</span></span>                 |
| <span data-ttu-id="8082f-129">**published**</span><span class="sxs-lookup"><span data-stu-id="8082f-129">**published**</span></span>            | [<span data-ttu-id="8082f-130">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="8082f-130">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="8082f-131">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="8082f-131">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="8082f-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8082f-132">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="8082f-133">Relações</span><span class="sxs-lookup"><span data-stu-id="8082f-133">Relationships</span></span>

<span data-ttu-id="8082f-134">A tabela a seguir define as relações que o recurso **driveItemVersion** tem com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="8082f-134">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="8082f-135">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="8082f-135">Relationship name</span></span> |                      <span data-ttu-id="8082f-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="8082f-136">Type</span></span>                      |                               <span data-ttu-id="8082f-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="8082f-137">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="8082f-138">**fields**</span><span class="sxs-lookup"><span data-stu-id="8082f-138">**fields**</span></span>        | [<span data-ttu-id="8082f-139">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="8082f-139">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="8082f-140">Uma coleção de campos e valores para esta versão do item da lista.</span><span class="sxs-lookup"><span data-stu-id="8082f-140">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
