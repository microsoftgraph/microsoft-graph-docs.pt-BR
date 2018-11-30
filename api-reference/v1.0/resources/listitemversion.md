---
title: Tipo de recurso ListItemVersion
description: O recurso **listItemVersion** representa uma versão anterior de um recurso ListItem.
ms.openlocfilehash: f036ea217abe766806e7f3c6b24bee4394f54889
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003536"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="fc864-103">Tipo de recurso ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="fc864-103">ListItemVersion resource type</span></span>

<span data-ttu-id="fc864-104">O recurso **listItemVersion** representa uma versão anterior de um recurso [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="fc864-104">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="fc864-105">Tarefas em recursos ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="fc864-105">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="fc864-106">As seguintes tarefas estão disponíveis para os recursos listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="fc864-106">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="fc864-107">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="fc864-107">Common task</span></span>             |         <span data-ttu-id="fc864-108">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="fc864-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="fc864-109">[Versões de lista][version-list]</span><span class="sxs-lookup"><span data-stu-id="fc864-109">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="fc864-110">[Obter versão][version-get]</span><span class="sxs-lookup"><span data-stu-id="fc864-110">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="fc864-111">[Restaurar versão][version-restore]</span><span class="sxs-lookup"><span data-stu-id="fc864-111">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="fc864-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc864-112">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="fc864-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc864-113">Properties</span></span>

|      <span data-ttu-id="fc864-114">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="fc864-114">Property name</span></span>       |                         <span data-ttu-id="fc864-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc864-115">Type</span></span>                         |                               <span data-ttu-id="fc864-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc864-116">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="fc864-117">**id**</span><span class="sxs-lookup"><span data-stu-id="fc864-117">**id**</span></span>                   | <span data-ttu-id="fc864-118">string</span><span class="sxs-lookup"><span data-stu-id="fc864-118">string</span></span>                                               | <span data-ttu-id="fc864-119">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="fc864-119">The ID of the version.</span></span> <span data-ttu-id="fc864-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fc864-120">Read-only.</span></span>                                       |
| <span data-ttu-id="fc864-121">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="fc864-121">**lastModifiedBy**</span></span>       | [<span data-ttu-id="fc864-122">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="fc864-122">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="fc864-123">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fc864-123">Identity of the user which last modified the version.</span></span> <span data-ttu-id="fc864-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fc864-124">Read-only.</span></span>        |
| <span data-ttu-id="fc864-125">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="fc864-125">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="fc864-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc864-126">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="fc864-127">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fc864-127">Date and time the version was last modified.</span></span> <span data-ttu-id="fc864-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fc864-128">Read-only.</span></span>                 |
| <span data-ttu-id="fc864-129">**published**</span><span class="sxs-lookup"><span data-stu-id="fc864-129">**published**</span></span>            | [<span data-ttu-id="fc864-130">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="fc864-130">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="fc864-131">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="fc864-131">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="fc864-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fc864-132">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="fc864-133">Relações</span><span class="sxs-lookup"><span data-stu-id="fc864-133">Relationships</span></span>

<span data-ttu-id="fc864-134">A tabela a seguir define as relações que o recurso **driveItemVersion** tem com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="fc864-134">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="fc864-135">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="fc864-135">Relationship name</span></span> |                      <span data-ttu-id="fc864-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc864-136">Type</span></span>                      |                               <span data-ttu-id="fc864-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc864-137">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="fc864-138">**fields**</span><span class="sxs-lookup"><span data-stu-id="fc864-138">**fields**</span></span>        | [<span data-ttu-id="fc864-139">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="fc864-139">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="fc864-140">Uma coleção de campos e valores para esta versão do item da lista.</span><span class="sxs-lookup"><span data-stu-id="fc864-140">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
