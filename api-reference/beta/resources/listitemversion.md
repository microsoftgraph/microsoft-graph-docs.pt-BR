---
author: JeremyKelley
description: O recurso listItemVersion representa uma versão anterior de um recurso ListItem.
ms.date: 09/17/2017
title: ListItemVersion
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ff3fbd3144a62939f9d4f6077c556c9d5884c687
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966952"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="88c88-103">Tipo de recurso ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="88c88-103">ListItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88c88-104">O recurso **listItemVersion** representa uma versão anterior de um recurso [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="88c88-104">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="88c88-105">Tarefas em recursos ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="88c88-105">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="88c88-106">As seguintes tarefas estão disponíveis para os recursos listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="88c88-106">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="88c88-107">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="88c88-107">Common task</span></span>             |         <span data-ttu-id="88c88-108">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="88c88-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="88c88-109">[Listar versões][version-list]</span><span class="sxs-lookup"><span data-stu-id="88c88-109">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="88c88-110">[Obter versão][version-get]</span><span class="sxs-lookup"><span data-stu-id="88c88-110">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="88c88-111">[Restaurar versão][version-restore]</span><span class="sxs-lookup"><span data-stu-id="88c88-111">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="88c88-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88c88-112">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="88c88-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88c88-113">Properties</span></span>

|      <span data-ttu-id="88c88-114">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="88c88-114">Property name</span></span>       |                         <span data-ttu-id="88c88-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="88c88-115">Type</span></span>                         |                               <span data-ttu-id="88c88-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="88c88-116">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="88c88-117">**id**</span><span class="sxs-lookup"><span data-stu-id="88c88-117">**id**</span></span>                   | <span data-ttu-id="88c88-118">string</span><span class="sxs-lookup"><span data-stu-id="88c88-118">string</span></span>                                               | <span data-ttu-id="88c88-119">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="88c88-119">The ID of the version.</span></span> <span data-ttu-id="88c88-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="88c88-120">Read-only.</span></span>                                       |
| <span data-ttu-id="88c88-121">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="88c88-121">**lastModifiedBy**</span></span>       | [<span data-ttu-id="88c88-122">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="88c88-122">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="88c88-123">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="88c88-123">Identity of the user which last modified the version.</span></span> <span data-ttu-id="88c88-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="88c88-124">Read-only.</span></span>        |
| <span data-ttu-id="88c88-125">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="88c88-125">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="88c88-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88c88-126">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="88c88-127">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="88c88-127">Date and time the version was last modified.</span></span> <span data-ttu-id="88c88-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="88c88-128">Read-only.</span></span>                 |
| <span data-ttu-id="88c88-129">**published**</span><span class="sxs-lookup"><span data-stu-id="88c88-129">**published**</span></span>            | [<span data-ttu-id="88c88-130">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="88c88-130">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="88c88-131">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="88c88-131">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="88c88-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="88c88-132">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="88c88-133">Relações</span><span class="sxs-lookup"><span data-stu-id="88c88-133">Relationships</span></span>

<span data-ttu-id="88c88-134">A tabela a seguir define as relações que o recurso **driveItemVersion** tem com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="88c88-134">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="88c88-135">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="88c88-135">Relationship name</span></span> |                      <span data-ttu-id="88c88-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="88c88-136">Type</span></span>                      |                               <span data-ttu-id="88c88-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="88c88-137">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="88c88-138">**fields**</span><span class="sxs-lookup"><span data-stu-id="88c88-138">**fields**</span></span>        | [<span data-ttu-id="88c88-139">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="88c88-139">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="88c88-140">Uma coleção de campos e valores para esta versão do item da lista.</span><span class="sxs-lookup"><span data-stu-id="88c88-140">A collection of the fields and values for this version of the list item.</span></span> |


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
