---
title: Tipo de recurso DriveItemVersion
description: O recurso **DriveItemVersion** representa uma versão específica de um DriveItem.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: resourcePageType
ms.openlocfilehash: e9521eb549bf84b900e6c49c4dedc5f2199de317
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029397"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="a9adf-103">Tipo de recurso DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="a9adf-103">DriveItemVersion resource type</span></span>

<span data-ttu-id="a9adf-104">O recurso **DriveItemVersion** representa uma versão específica de um [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="a9adf-104">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="a9adf-105">Tarefas em recursos DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="a9adf-105">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="a9adf-106">As tarefas a seguir estão disponíveis para recursos driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="a9adf-106">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="a9adf-107">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="a9adf-107">Common task</span></span>             |         <span data-ttu-id="a9adf-108">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="a9adf-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="a9adf-109">[Listar versões][version-list]</span><span class="sxs-lookup"><span data-stu-id="a9adf-109">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="a9adf-110">[Obter versão][version-get]</span><span class="sxs-lookup"><span data-stu-id="a9adf-110">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="a9adf-111">[Obter conteúdo][content-get]</span><span class="sxs-lookup"><span data-stu-id="a9adf-111">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="a9adf-112">[Restaurar versão][version-restore]</span><span class="sxs-lookup"><span data-stu-id="a9adf-112">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="a9adf-113">Na tabela anterior, os exemplos usam `/drive`, mas há muitas solicitações válidas.</span><span class="sxs-lookup"><span data-stu-id="a9adf-113">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9adf-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9adf-114">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.driveItemVersion",
  "@type.aka": "oneDrive.driveItemVersion"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" },
  "size": 12356
}
```

## <a name="properties"></a><span data-ttu-id="a9adf-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9adf-115">Properties</span></span>

|      <span data-ttu-id="a9adf-116">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="a9adf-116">Property name</span></span>       |                         <span data-ttu-id="a9adf-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9adf-117">Type</span></span>                         |                               <span data-ttu-id="a9adf-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9adf-118">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="a9adf-119">**id**</span><span class="sxs-lookup"><span data-stu-id="a9adf-119">**id**</span></span>                   | <span data-ttu-id="a9adf-120">string</span><span class="sxs-lookup"><span data-stu-id="a9adf-120">string</span></span>                                               | <span data-ttu-id="a9adf-121">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="a9adf-121">The ID of the version.</span></span> <span data-ttu-id="a9adf-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a9adf-122">Read-only.</span></span>                                       |
| <span data-ttu-id="a9adf-123">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="a9adf-123">**lastModifiedBy**</span></span>       | [<span data-ttu-id="a9adf-124">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="a9adf-124">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="a9adf-125">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a9adf-125">Identity of the user which last modified the version.</span></span> <span data-ttu-id="a9adf-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a9adf-126">Read-only.</span></span>        |
| <span data-ttu-id="a9adf-127">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="a9adf-127">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="a9adf-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9adf-128">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="a9adf-129">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a9adf-129">Date and time the version was last modified.</span></span> <span data-ttu-id="a9adf-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a9adf-130">Read-only.</span></span>                 |
| <span data-ttu-id="a9adf-131">**publication**</span><span class="sxs-lookup"><span data-stu-id="a9adf-131">**publication**</span></span>          | [<span data-ttu-id="a9adf-132">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="a9adf-132">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="a9adf-133">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="a9adf-133">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="a9adf-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a9adf-134">Read-only.</span></span> |
| <span data-ttu-id="a9adf-135">**size**</span><span class="sxs-lookup"><span data-stu-id="a9adf-135">**size**</span></span>                 | <span data-ttu-id="a9adf-136">Int64</span><span class="sxs-lookup"><span data-stu-id="a9adf-136">Int64</span></span>                                                | <span data-ttu-id="a9adf-137">Indica o tamanho do fluxo de conteúdo para esta versão do item.</span><span class="sxs-lookup"><span data-stu-id="a9adf-137">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="a9adf-138">**content**</span><span class="sxs-lookup"><span data-stu-id="a9adf-138">**content**</span></span>              | <span data-ttu-id="a9adf-139">Fluxo</span><span class="sxs-lookup"><span data-stu-id="a9adf-139">Stream</span></span>                                               | <span data-ttu-id="a9adf-140">O fluxo de conteúdo para esta versão do item.</span><span class="sxs-lookup"><span data-stu-id="a9adf-140">The content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
