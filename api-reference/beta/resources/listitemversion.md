---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: listItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1d153a8ae8291e0299d1a470db6c8c7e0c8bd3e4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524748"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="91b23-102">Tipo de recurso ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="91b23-102">ListItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91b23-103">O recurso **listItemVersion** representa uma versão anterior de um recurso [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="91b23-103">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="91b23-104">Tarefas em recursos ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="91b23-104">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="91b23-105">As seguintes tarefas estão disponíveis para os recursos listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="91b23-105">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="91b23-106">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="91b23-106">Common task</span></span>             |         <span data-ttu-id="91b23-107">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="91b23-107">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="91b23-108">[Versões de lista][version-list]</span><span class="sxs-lookup"><span data-stu-id="91b23-108">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="91b23-109">[Obter versão][version-get]</span><span class="sxs-lookup"><span data-stu-id="91b23-109">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="91b23-110">[Restaurar versão][version-restore]</span><span class="sxs-lookup"><span data-stu-id="91b23-110">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="91b23-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91b23-111">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.listItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

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

## <a name="properties"></a><span data-ttu-id="91b23-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91b23-112">Properties</span></span>

|      <span data-ttu-id="91b23-113">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="91b23-113">Property name</span></span>       |                         <span data-ttu-id="91b23-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="91b23-114">Type</span></span>                         |                               <span data-ttu-id="91b23-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="91b23-115">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="91b23-116">**id**</span><span class="sxs-lookup"><span data-stu-id="91b23-116">**id**</span></span>                   | <span data-ttu-id="91b23-117">string</span><span class="sxs-lookup"><span data-stu-id="91b23-117">string</span></span>                                               | <span data-ttu-id="91b23-118">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="91b23-118">The ID of the version.</span></span> <span data-ttu-id="91b23-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="91b23-119">Read-only.</span></span>                                       |
| <span data-ttu-id="91b23-120">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="91b23-120">**lastModifiedBy**</span></span>       | [<span data-ttu-id="91b23-121">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="91b23-121">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="91b23-122">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="91b23-122">Identity of the user which last modified the version.</span></span> <span data-ttu-id="91b23-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="91b23-123">Read-only.</span></span>        |
| <span data-ttu-id="91b23-124">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="91b23-124">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="91b23-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91b23-125">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="91b23-126">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="91b23-126">Date and time the version was last modified.</span></span> <span data-ttu-id="91b23-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="91b23-127">Read-only.</span></span>                 |
| <span data-ttu-id="91b23-128">**published**</span><span class="sxs-lookup"><span data-stu-id="91b23-128">**published**</span></span>            | [<span data-ttu-id="91b23-129">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="91b23-129">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="91b23-130">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="91b23-130">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="91b23-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="91b23-131">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="91b23-132">Relações</span><span class="sxs-lookup"><span data-stu-id="91b23-132">Relationships</span></span>

<span data-ttu-id="91b23-133">A tabela a seguir define as relações que o recurso **driveItemVersion** tem com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="91b23-133">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="91b23-134">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="91b23-134">Relationship name</span></span> |                      <span data-ttu-id="91b23-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="91b23-135">Type</span></span>                      |                               <span data-ttu-id="91b23-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="91b23-136">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="91b23-137">**fields**</span><span class="sxs-lookup"><span data-stu-id="91b23-137">**fields**</span></span>        | [<span data-ttu-id="91b23-138">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="91b23-138">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="91b23-139">Uma coleção de campos e valores para esta versão do item da lista.</span><span class="sxs-lookup"><span data-stu-id="91b23-139">A collection of the fields and values for this version of the list item.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/listitemversion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
