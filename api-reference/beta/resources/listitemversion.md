---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: ListItemVersion
localization_priority: Normal
ms.openlocfilehash: 0ffdda98d941ef197bd956146ba796ace037cb8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849620"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="b5173-102">Tipo de recurso ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="b5173-102">ListItemVersion resource type</span></span>

> <span data-ttu-id="b5173-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b5173-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5173-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b5173-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b5173-105">O recurso **listItemVersion** representa uma versão anterior de um recurso [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="b5173-105">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="b5173-106">Tarefas em recursos ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="b5173-106">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="b5173-107">As seguintes tarefas estão disponíveis para os recursos listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="b5173-107">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="b5173-108">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="b5173-108">Common task</span></span>             |         <span data-ttu-id="b5173-109">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="b5173-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="b5173-110">[Versões de lista][version-list]</span><span class="sxs-lookup"><span data-stu-id="b5173-110">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="b5173-111">[Obter versão][version-get]</span><span class="sxs-lookup"><span data-stu-id="b5173-111">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="b5173-112">[Restaurar versão][version-restore]</span><span class="sxs-lookup"><span data-stu-id="b5173-112">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="b5173-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b5173-113">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b5173-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b5173-114">Properties</span></span>

|      <span data-ttu-id="b5173-115">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="b5173-115">Property name</span></span>       |                         <span data-ttu-id="b5173-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5173-116">Type</span></span>                         |                               <span data-ttu-id="b5173-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5173-117">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="b5173-118">**id**</span><span class="sxs-lookup"><span data-stu-id="b5173-118">**id**</span></span>                   | <span data-ttu-id="b5173-119">string</span><span class="sxs-lookup"><span data-stu-id="b5173-119">string</span></span>                                               | <span data-ttu-id="b5173-120">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="b5173-120">The ID of the version.</span></span> <span data-ttu-id="b5173-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5173-121">Read-only.</span></span>                                       |
| <span data-ttu-id="b5173-122">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="b5173-122">**lastModifiedBy**</span></span>       | [<span data-ttu-id="b5173-123">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="b5173-123">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="b5173-124">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b5173-124">Identity of the user which last modified the version.</span></span> <span data-ttu-id="b5173-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5173-125">Read-only.</span></span>        |
| <span data-ttu-id="b5173-126">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="b5173-126">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="b5173-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5173-127">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="b5173-128">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b5173-128">Date and time the version was last modified.</span></span> <span data-ttu-id="b5173-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5173-129">Read-only.</span></span>                 |
| <span data-ttu-id="b5173-130">**published**</span><span class="sxs-lookup"><span data-stu-id="b5173-130">**published**</span></span>            | [<span data-ttu-id="b5173-131">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="b5173-131">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="b5173-132">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="b5173-132">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="b5173-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5173-133">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="b5173-134">Relações</span><span class="sxs-lookup"><span data-stu-id="b5173-134">Relationships</span></span>

<span data-ttu-id="b5173-135">A tabela a seguir define as relações que o recurso **driveItemVersion** tem com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="b5173-135">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="b5173-136">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="b5173-136">Relationship name</span></span> |                      <span data-ttu-id="b5173-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5173-137">Type</span></span>                      |                               <span data-ttu-id="b5173-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5173-138">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="b5173-139">**fields**</span><span class="sxs-lookup"><span data-stu-id="b5173-139">**fields**</span></span>        | [<span data-ttu-id="b5173-140">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="b5173-140">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="b5173-141">Uma coleção de campos e valores para esta versão do item da lista.</span><span class="sxs-lookup"><span data-stu-id="b5173-141">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
