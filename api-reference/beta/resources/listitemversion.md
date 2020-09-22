---
author: JeremyKelley
description: O recurso listItemVersion representa uma versão anterior de um recurso ListItem.
ms.date: 09/17/2017
title: ListItemVersion
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: de11928d2ac6f0f78e2dabbd34ebb25d927c5aa9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055236"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="a38f5-103">Tipo de recurso ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="a38f5-103">ListItemVersion resource type</span></span>

<span data-ttu-id="a38f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a38f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a38f5-105">O recurso **listItemVersion** representa uma versão anterior de um recurso [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="a38f5-105">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="a38f5-106">Tarefas em recursos ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="a38f5-106">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="a38f5-107">As seguintes tarefas estão disponíveis para os recursos listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="a38f5-107">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="a38f5-108">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="a38f5-108">Common task</span></span>             |         <span data-ttu-id="a38f5-109">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="a38f5-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="a38f5-110">[Listar versões][version-list]</span><span class="sxs-lookup"><span data-stu-id="a38f5-110">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="a38f5-111">[Obter versão][version-get]</span><span class="sxs-lookup"><span data-stu-id="a38f5-111">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="a38f5-112">[Restaurar versão][version-restore]</span><span class="sxs-lookup"><span data-stu-id="a38f5-112">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="a38f5-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a38f5-113">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="a38f5-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a38f5-114">Properties</span></span>

|      <span data-ttu-id="a38f5-115">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="a38f5-115">Property name</span></span>       |                         <span data-ttu-id="a38f5-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="a38f5-116">Type</span></span>                         |                               <span data-ttu-id="a38f5-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="a38f5-117">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="a38f5-118">**id**</span><span class="sxs-lookup"><span data-stu-id="a38f5-118">**id**</span></span>                   | <span data-ttu-id="a38f5-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a38f5-119">string</span></span>                                               | <span data-ttu-id="a38f5-120">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="a38f5-120">The ID of the version.</span></span> <span data-ttu-id="a38f5-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a38f5-121">Read-only.</span></span>                                       |
| <span data-ttu-id="a38f5-122">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="a38f5-122">**lastModifiedBy**</span></span>       | [<span data-ttu-id="a38f5-123">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="a38f5-123">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="a38f5-124">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a38f5-124">Identity of the user which last modified the version.</span></span> <span data-ttu-id="a38f5-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a38f5-125">Read-only.</span></span>        |
| <span data-ttu-id="a38f5-126">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="a38f5-126">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="a38f5-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a38f5-127">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="a38f5-128">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a38f5-128">Date and time the version was last modified.</span></span> <span data-ttu-id="a38f5-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a38f5-129">Read-only.</span></span>                 |
| <span data-ttu-id="a38f5-130">**published**</span><span class="sxs-lookup"><span data-stu-id="a38f5-130">**published**</span></span>            | [<span data-ttu-id="a38f5-131">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="a38f5-131">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="a38f5-132">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="a38f5-132">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="a38f5-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a38f5-133">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="a38f5-134">Relações</span><span class="sxs-lookup"><span data-stu-id="a38f5-134">Relationships</span></span>

<span data-ttu-id="a38f5-135">A tabela a seguir define as relações que o recurso **driveItemVersion** tem com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="a38f5-135">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="a38f5-136">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="a38f5-136">Relationship name</span></span> |                      <span data-ttu-id="a38f5-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="a38f5-137">Type</span></span>                      |                               <span data-ttu-id="a38f5-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="a38f5-138">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="a38f5-139">**fields**</span><span class="sxs-lookup"><span data-stu-id="a38f5-139">**fields**</span></span>        | [<span data-ttu-id="a38f5-140">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="a38f5-140">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="a38f5-141">Uma coleção de campos e valores para esta versão do item da lista.</span><span class="sxs-lookup"><span data-stu-id="a38f5-141">A collection of the fields and values for this version of the list item.</span></span> |


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


