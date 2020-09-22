---
title: Tipo de recurso DriveItemVersion
description: O recurso **DriveItemVersion** representa uma versão específica de um DriveItem.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: resourcePageType
ms.openlocfilehash: 1f7c45ecc82a209094748410614d6b25993e2aa7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018575"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="38587-103">Tipo de recurso DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="38587-103">DriveItemVersion resource type</span></span>

<span data-ttu-id="38587-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38587-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="38587-105">O recurso **DriveItemVersion** representa uma versão específica de um [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="38587-105">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="38587-106">Tarefas em recursos DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="38587-106">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="38587-107">As tarefas a seguir estão disponíveis para recursos driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="38587-107">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="38587-108">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="38587-108">Common task</span></span>             |         <span data-ttu-id="38587-109">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="38587-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="38587-110">[Listar versões][version-list]</span><span class="sxs-lookup"><span data-stu-id="38587-110">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="38587-111">[Obter versão][version-get]</span><span class="sxs-lookup"><span data-stu-id="38587-111">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="38587-112">[Obter conteúdo][content-get]</span><span class="sxs-lookup"><span data-stu-id="38587-112">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="38587-113">[Restaurar versão][version-restore]</span><span class="sxs-lookup"><span data-stu-id="38587-113">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="38587-114">Na tabela anterior, os exemplos usam `/drive`, mas há muitas solicitações válidas.</span><span class="sxs-lookup"><span data-stu-id="38587-114">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="38587-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38587-115">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="38587-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38587-116">Properties</span></span>

|      <span data-ttu-id="38587-117">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="38587-117">Property name</span></span>       |                         <span data-ttu-id="38587-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="38587-118">Type</span></span>                         |                               <span data-ttu-id="38587-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="38587-119">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="38587-120">**id**</span><span class="sxs-lookup"><span data-stu-id="38587-120">**id**</span></span>                   | <span data-ttu-id="38587-121">string</span><span class="sxs-lookup"><span data-stu-id="38587-121">string</span></span>                                               | <span data-ttu-id="38587-122">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="38587-122">The ID of the version.</span></span> <span data-ttu-id="38587-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38587-123">Read-only.</span></span>                                       |
| <span data-ttu-id="38587-124">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="38587-124">**lastModifiedBy**</span></span>       | [<span data-ttu-id="38587-125">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="38587-125">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="38587-126">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="38587-126">Identity of the user which last modified the version.</span></span> <span data-ttu-id="38587-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38587-127">Read-only.</span></span>        |
| <span data-ttu-id="38587-128">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="38587-128">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="38587-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38587-129">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="38587-130">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="38587-130">Date and time the version was last modified.</span></span> <span data-ttu-id="38587-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38587-131">Read-only.</span></span>                 |
| <span data-ttu-id="38587-132">**publication**</span><span class="sxs-lookup"><span data-stu-id="38587-132">**publication**</span></span>          | [<span data-ttu-id="38587-133">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="38587-133">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="38587-134">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="38587-134">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="38587-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38587-135">Read-only.</span></span> |
| <span data-ttu-id="38587-136">**size**</span><span class="sxs-lookup"><span data-stu-id="38587-136">**size**</span></span>                 | <span data-ttu-id="38587-137">Int64</span><span class="sxs-lookup"><span data-stu-id="38587-137">Int64</span></span>                                                | <span data-ttu-id="38587-138">Indica o tamanho do fluxo de conteúdo para esta versão do item.</span><span class="sxs-lookup"><span data-stu-id="38587-138">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="38587-139">**content**</span><span class="sxs-lookup"><span data-stu-id="38587-139">**content**</span></span>              | <span data-ttu-id="38587-140">Fluxo</span><span class="sxs-lookup"><span data-stu-id="38587-140">Stream</span></span>                                               | <span data-ttu-id="38587-141">O fluxo de conteúdo para esta versão do item.</span><span class="sxs-lookup"><span data-stu-id="38587-141">The content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->

