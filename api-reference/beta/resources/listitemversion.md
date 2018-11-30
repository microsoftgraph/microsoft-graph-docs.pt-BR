---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: ListItemVersion
ms.openlocfilehash: 7cda16159c6e5e58a0f60aef3c60198c7615f9e0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033224"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="fcb0f-102">Tipo de recurso ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="fcb0f-102">ListItemVersion resource type</span></span>

> <span data-ttu-id="fcb0f-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fcb0f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fcb0f-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fcb0f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fcb0f-105">O recurso **listItemVersion** representa uma versão anterior de um recurso [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="fcb0f-105">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="fcb0f-106">Tarefas em recursos ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="fcb0f-106">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="fcb0f-107">As seguintes tarefas estão disponíveis para os recursos listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="fcb0f-107">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="fcb0f-108">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="fcb0f-108">Common task</span></span>             |         <span data-ttu-id="fcb0f-109">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="fcb0f-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="fcb0f-110">[Versões de lista][version-list]</span><span class="sxs-lookup"><span data-stu-id="fcb0f-110">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="fcb0f-111">[Obter versão][version-get]</span><span class="sxs-lookup"><span data-stu-id="fcb0f-111">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="fcb0f-112">[Restaurar versão][version-restore]</span><span class="sxs-lookup"><span data-stu-id="fcb0f-112">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="fcb0f-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fcb0f-113">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="fcb0f-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fcb0f-114">Properties</span></span>

|      <span data-ttu-id="fcb0f-115">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="fcb0f-115">Property name</span></span>       |                         <span data-ttu-id="fcb0f-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcb0f-116">Type</span></span>                         |                               <span data-ttu-id="fcb0f-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcb0f-117">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="fcb0f-118">**id**</span><span class="sxs-lookup"><span data-stu-id="fcb0f-118">**id**</span></span>                   | <span data-ttu-id="fcb0f-119">string</span><span class="sxs-lookup"><span data-stu-id="fcb0f-119">string</span></span>                                               | <span data-ttu-id="fcb0f-120">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="fcb0f-120">The ID of the version.</span></span> <span data-ttu-id="fcb0f-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fcb0f-121">Read-only.</span></span>                                       |
| <span data-ttu-id="fcb0f-122">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="fcb0f-122">**lastModifiedBy**</span></span>       | [<span data-ttu-id="fcb0f-123">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="fcb0f-123">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="fcb0f-124">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fcb0f-124">Identity of the user which last modified the version.</span></span> <span data-ttu-id="fcb0f-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fcb0f-125">Read-only.</span></span>        |
| <span data-ttu-id="fcb0f-126">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="fcb0f-126">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="fcb0f-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcb0f-127">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="fcb0f-128">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fcb0f-128">Date and time the version was last modified.</span></span> <span data-ttu-id="fcb0f-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fcb0f-129">Read-only.</span></span>                 |
| <span data-ttu-id="fcb0f-130">**published**</span><span class="sxs-lookup"><span data-stu-id="fcb0f-130">**published**</span></span>            | [<span data-ttu-id="fcb0f-131">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="fcb0f-131">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="fcb0f-132">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="fcb0f-132">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="fcb0f-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fcb0f-133">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="fcb0f-134">Relações</span><span class="sxs-lookup"><span data-stu-id="fcb0f-134">Relationships</span></span>

<span data-ttu-id="fcb0f-135">A tabela a seguir define as relações que o recurso **driveItemVersion** tem com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="fcb0f-135">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="fcb0f-136">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="fcb0f-136">Relationship name</span></span> |                      <span data-ttu-id="fcb0f-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcb0f-137">Type</span></span>                      |                               <span data-ttu-id="fcb0f-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcb0f-138">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="fcb0f-139">**fields**</span><span class="sxs-lookup"><span data-stu-id="fcb0f-139">**fields**</span></span>        | [<span data-ttu-id="fcb0f-140">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="fcb0f-140">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="fcb0f-141">Uma coleção de campos e valores para esta versão do item da lista.</span><span class="sxs-lookup"><span data-stu-id="fcb0f-141">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->