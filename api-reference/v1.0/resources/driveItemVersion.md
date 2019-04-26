---
title: Tipo de recurso DriveItemVersion
description: O recurso **DriveItemVersion** representa uma versão específica de um DriveItem.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fd6052464d40fcce86b83d93601282dda252c69b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562682"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="87e98-103">Tipo de recurso DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="87e98-103">DriveItemVersion resource type</span></span>

<span data-ttu-id="87e98-104">O recurso **DriveItemVersion** representa uma versão específica de um [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="87e98-104">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="87e98-105">Tarefas em recursos DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="87e98-105">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="87e98-106">As tarefas a seguir estão disponíveis para recursos driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="87e98-106">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="87e98-107">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="87e98-107">Common task</span></span>             |         <span data-ttu-id="87e98-108">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="87e98-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="87e98-109">[Versões de lista][version-list]</span><span class="sxs-lookup"><span data-stu-id="87e98-109">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="87e98-110">[Obter versão][version-get]</span><span class="sxs-lookup"><span data-stu-id="87e98-110">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="87e98-111">[Obter conteúdo][content-get]</span><span class="sxs-lookup"><span data-stu-id="87e98-111">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="87e98-112">[Restaurar versão][version-restore]</span><span class="sxs-lookup"><span data-stu-id="87e98-112">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="87e98-113">Na tabela anterior, os exemplos usam `/drive`, mas há muitas solicitações válidas.</span><span class="sxs-lookup"><span data-stu-id="87e98-113">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="87e98-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87e98-114">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="87e98-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87e98-115">Properties</span></span>

|      <span data-ttu-id="87e98-116">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="87e98-116">Property name</span></span>       |                         <span data-ttu-id="87e98-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="87e98-117">Type</span></span>                         |                               <span data-ttu-id="87e98-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="87e98-118">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="87e98-119">**id**</span><span class="sxs-lookup"><span data-stu-id="87e98-119">**id**</span></span>                   | <span data-ttu-id="87e98-120">string</span><span class="sxs-lookup"><span data-stu-id="87e98-120">string</span></span>                                               | <span data-ttu-id="87e98-121">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="87e98-121">The ID of the version.</span></span> <span data-ttu-id="87e98-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87e98-122">Read-only.</span></span>                                       |
| <span data-ttu-id="87e98-123">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="87e98-123">**lastModifiedBy**</span></span>       | [<span data-ttu-id="87e98-124">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="87e98-124">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="87e98-125">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="87e98-125">Identity of the user which last modified the version.</span></span> <span data-ttu-id="87e98-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87e98-126">Read-only.</span></span>        |
| <span data-ttu-id="87e98-127">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="87e98-127">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="87e98-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87e98-128">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="87e98-129">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="87e98-129">Date and time the version was last modified.</span></span> <span data-ttu-id="87e98-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87e98-130">Read-only.</span></span>                 |
| <span data-ttu-id="87e98-131">**publication**</span><span class="sxs-lookup"><span data-stu-id="87e98-131">**publication**</span></span>          | [<span data-ttu-id="87e98-132">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="87e98-132">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="87e98-133">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="87e98-133">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="87e98-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87e98-134">Read-only.</span></span> |
| <span data-ttu-id="87e98-135">**size**</span><span class="sxs-lookup"><span data-stu-id="87e98-135">**size**</span></span>                 | <span data-ttu-id="87e98-136">Int64</span><span class="sxs-lookup"><span data-stu-id="87e98-136">Int64</span></span>                                                | <span data-ttu-id="87e98-137">Indica o tamanho do fluxo de conteúdo para esta versão do item.</span><span class="sxs-lookup"><span data-stu-id="87e98-137">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="87e98-138">**content**</span><span class="sxs-lookup"><span data-stu-id="87e98-138">**content**</span></span>              | <span data-ttu-id="87e98-139">Fluxo</span><span class="sxs-lookup"><span data-stu-id="87e98-139">Stream</span></span>                                               | <span data-ttu-id="87e98-140">O fluxo de conteúdo para esta versão do item.</span><span class="sxs-lookup"><span data-stu-id="87e98-140">The content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
