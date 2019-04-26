---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/17/2017
title: ListItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 56413ad243e5c6c2c2a7ae3a81dab50586f42db8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345229"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="9dab6-102">Tipo de recurso ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="9dab6-102">ListItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dab6-103">O recurso **listItemVersion** representa uma versão anterior de um recurso [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="9dab6-103">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="9dab6-104">Tarefas em recursos ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="9dab6-104">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="9dab6-105">As seguintes tarefas estão disponíveis para os recursos listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="9dab6-105">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="9dab6-106">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="9dab6-106">Common task</span></span>             |         <span data-ttu-id="9dab6-107">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="9dab6-107">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="9dab6-108">[Versões de lista][version-list]</span><span class="sxs-lookup"><span data-stu-id="9dab6-108">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="9dab6-109">[Obter versão][version-get]</span><span class="sxs-lookup"><span data-stu-id="9dab6-109">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="9dab6-110">[Restaurar versão][version-restore]</span><span class="sxs-lookup"><span data-stu-id="9dab6-110">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="9dab6-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9dab6-111">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="9dab6-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9dab6-112">Properties</span></span>

|      <span data-ttu-id="9dab6-113">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="9dab6-113">Property name</span></span>       |                         <span data-ttu-id="9dab6-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="9dab6-114">Type</span></span>                         |                               <span data-ttu-id="9dab6-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="9dab6-115">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="9dab6-116">**id**</span><span class="sxs-lookup"><span data-stu-id="9dab6-116">**id**</span></span>                   | <span data-ttu-id="9dab6-117">string</span><span class="sxs-lookup"><span data-stu-id="9dab6-117">string</span></span>                                               | <span data-ttu-id="9dab6-118">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="9dab6-118">The ID of the version.</span></span> <span data-ttu-id="9dab6-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9dab6-119">Read-only.</span></span>                                       |
| <span data-ttu-id="9dab6-120">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="9dab6-120">**lastModifiedBy**</span></span>       | [<span data-ttu-id="9dab6-121">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="9dab6-121">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="9dab6-122">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9dab6-122">Identity of the user which last modified the version.</span></span> <span data-ttu-id="9dab6-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9dab6-123">Read-only.</span></span>        |
| <span data-ttu-id="9dab6-124">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="9dab6-124">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="9dab6-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dab6-125">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="9dab6-126">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9dab6-126">Date and time the version was last modified.</span></span> <span data-ttu-id="9dab6-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9dab6-127">Read-only.</span></span>                 |
| <span data-ttu-id="9dab6-128">**published**</span><span class="sxs-lookup"><span data-stu-id="9dab6-128">**published**</span></span>            | [<span data-ttu-id="9dab6-129">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="9dab6-129">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="9dab6-130">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="9dab6-130">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="9dab6-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9dab6-131">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="9dab6-132">Relações</span><span class="sxs-lookup"><span data-stu-id="9dab6-132">Relationships</span></span>

<span data-ttu-id="9dab6-133">A tabela a seguir define as relações que o recurso **driveItemVersion** tem com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="9dab6-133">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="9dab6-134">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="9dab6-134">Relationship name</span></span> |                      <span data-ttu-id="9dab6-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="9dab6-135">Type</span></span>                      |                               <span data-ttu-id="9dab6-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="9dab6-136">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="9dab6-137">**fields**</span><span class="sxs-lookup"><span data-stu-id="9dab6-137">**fields**</span></span>        | [<span data-ttu-id="9dab6-138">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="9dab6-138">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="9dab6-139">Uma coleção de campos e valores para esta versão do item da lista.</span><span class="sxs-lookup"><span data-stu-id="9dab6-139">A collection of the fields and values for this version of the list item.</span></span> |


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
