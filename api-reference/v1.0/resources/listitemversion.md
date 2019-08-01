---
title: Tipo de recurso ListItemVersion
description: O recurso **listItemVersion** representa uma versão anterior de um recurso ListItem.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: resourcePageType
ms.openlocfilehash: 8523e77fd308ab4863a0c3d90ccacad73cc766cc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036445"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="e249a-103">Tipo de recurso ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="e249a-103">ListItemVersion resource type</span></span>

<span data-ttu-id="e249a-104">O recurso **listItemVersion** representa uma versão anterior de um recurso [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="e249a-104">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="e249a-105">Tarefas em recursos ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="e249a-105">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="e249a-106">As seguintes tarefas estão disponíveis para os recursos listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="e249a-106">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="e249a-107">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="e249a-107">Common task</span></span>             |         <span data-ttu-id="e249a-108">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="e249a-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="e249a-109">[Listar versões][version-list]</span><span class="sxs-lookup"><span data-stu-id="e249a-109">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="e249a-110">[Obter versão][version-get]</span><span class="sxs-lookup"><span data-stu-id="e249a-110">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="e249a-111">[Restaurar versão][version-restore]</span><span class="sxs-lookup"><span data-stu-id="e249a-111">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="e249a-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e249a-112">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e249a-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e249a-113">Properties</span></span>

|      <span data-ttu-id="e249a-114">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e249a-114">Property name</span></span>       |                         <span data-ttu-id="e249a-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="e249a-115">Type</span></span>                         |                               <span data-ttu-id="e249a-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="e249a-116">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="e249a-117">**id**</span><span class="sxs-lookup"><span data-stu-id="e249a-117">**id**</span></span>                   | <span data-ttu-id="e249a-118">string</span><span class="sxs-lookup"><span data-stu-id="e249a-118">string</span></span>                                               | <span data-ttu-id="e249a-119">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="e249a-119">The ID of the version.</span></span> <span data-ttu-id="e249a-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e249a-120">Read-only.</span></span>                                       |
| <span data-ttu-id="e249a-121">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="e249a-121">**lastModifiedBy**</span></span>       | [<span data-ttu-id="e249a-122">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="e249a-122">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="e249a-123">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e249a-123">Identity of the user which last modified the version.</span></span> <span data-ttu-id="e249a-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e249a-124">Read-only.</span></span>        |
| <span data-ttu-id="e249a-125">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="e249a-125">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="e249a-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e249a-126">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="e249a-127">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e249a-127">Date and time the version was last modified.</span></span> <span data-ttu-id="e249a-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e249a-128">Read-only.</span></span>                 |
| <span data-ttu-id="e249a-129">**published**</span><span class="sxs-lookup"><span data-stu-id="e249a-129">**published**</span></span>            | [<span data-ttu-id="e249a-130">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="e249a-130">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="e249a-131">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="e249a-131">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="e249a-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e249a-132">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="e249a-133">Relações</span><span class="sxs-lookup"><span data-stu-id="e249a-133">Relationships</span></span>

<span data-ttu-id="e249a-134">A tabela a seguir define as relações que o recurso **driveItemVersion** tem com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="e249a-134">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="e249a-135">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="e249a-135">Relationship name</span></span> |                      <span data-ttu-id="e249a-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="e249a-136">Type</span></span>                      |                               <span data-ttu-id="e249a-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="e249a-137">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="e249a-138">**fields**</span><span class="sxs-lookup"><span data-stu-id="e249a-138">**fields**</span></span>        | [<span data-ttu-id="e249a-139">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="e249a-139">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="e249a-140">Uma coleção de campos e valores para esta versão do item da lista.</span><span class="sxs-lookup"><span data-stu-id="e249a-140">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
