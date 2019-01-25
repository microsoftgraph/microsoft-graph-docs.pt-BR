---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: driveItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 25b480a22b93ce454927177d2d842390496f54de
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528967"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="78071-102">Tipo de recurso DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="78071-102">DriveItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78071-103">O recurso **DriveItemVersion** representa uma versão específica de um [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="78071-103">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="78071-104">Tarefas em recursos DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="78071-104">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="78071-105">As tarefas a seguir estão disponíveis para recursos driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="78071-105">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="78071-106">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="78071-106">Common task</span></span>             |         <span data-ttu-id="78071-107">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="78071-107">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="78071-108">[Versões de lista][version-list]</span><span class="sxs-lookup"><span data-stu-id="78071-108">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="78071-109">[Obter versão][version-get]</span><span class="sxs-lookup"><span data-stu-id="78071-109">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="78071-110">[Obter conteúdo][content-get]</span><span class="sxs-lookup"><span data-stu-id="78071-110">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="78071-111">[Restaurar versão][version-restore]</span><span class="sxs-lookup"><span data-stu-id="78071-111">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="78071-112">Na tabela anterior, os exemplos usam `/drive`, mas há muitas solicitações válidas.</span><span class="sxs-lookup"><span data-stu-id="78071-112">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="78071-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78071-113">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemVersion", "@type.aka": "oneDrive.driveItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="78071-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78071-114">Properties</span></span>

|      <span data-ttu-id="78071-115">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="78071-115">Property name</span></span>       |                         <span data-ttu-id="78071-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="78071-116">Type</span></span>                         |                               <span data-ttu-id="78071-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="78071-117">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="78071-118">**id**</span><span class="sxs-lookup"><span data-stu-id="78071-118">**id**</span></span>                   | <span data-ttu-id="78071-119">string</span><span class="sxs-lookup"><span data-stu-id="78071-119">string</span></span>                                               | <span data-ttu-id="78071-120">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="78071-120">The ID of the version.</span></span> <span data-ttu-id="78071-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78071-121">Read-only.</span></span>                                       |
| <span data-ttu-id="78071-122">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="78071-122">**lastModifiedBy**</span></span>       | [<span data-ttu-id="78071-123">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="78071-123">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="78071-124">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="78071-124">Identity of the user which last modified the version.</span></span> <span data-ttu-id="78071-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78071-125">Read-only.</span></span>        |
| <span data-ttu-id="78071-126">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="78071-126">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="78071-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78071-127">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="78071-128">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="78071-128">Date and time the version was last modified.</span></span> <span data-ttu-id="78071-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78071-129">Read-only.</span></span>                 |
| <span data-ttu-id="78071-130">publication</span><span class="sxs-lookup"><span data-stu-id="78071-130">**publication**</span></span>          | [<span data-ttu-id="78071-131">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="78071-131">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="78071-132">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="78071-132">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="78071-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78071-133">Read-only.</span></span> |
| <span data-ttu-id="78071-134">**size**</span><span class="sxs-lookup"><span data-stu-id="78071-134">**size**</span></span>                 | <span data-ttu-id="78071-135">Int64</span><span class="sxs-lookup"><span data-stu-id="78071-135">Int64</span></span>                                                | <span data-ttu-id="78071-136">Indica o tamanho do fluxo de conteúdo para esta versão do item.</span><span class="sxs-lookup"><span data-stu-id="78071-136">Indicates the size of the content stream for this version of the item.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="78071-137">Relações</span><span class="sxs-lookup"><span data-stu-id="78071-137">Relationships</span></span>

<span data-ttu-id="78071-138">A tabela a seguir define as relações que o recurso **driveItemVersion** tem com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="78071-138">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="78071-139">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="78071-139">Relationship name</span></span> |  <span data-ttu-id="78071-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="78071-140">Type</span></span>  |            <span data-ttu-id="78071-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="78071-141">Description</span></span>             |
| :---------------- | :----- | :--------------------------------- |
| <span data-ttu-id="78071-142">**content**</span><span class="sxs-lookup"><span data-stu-id="78071-142">**content**</span></span>       | <span data-ttu-id="78071-143">Fluxo</span><span class="sxs-lookup"><span data-stu-id="78071-143">Stream</span></span> | <span data-ttu-id="78071-144">O fluxo de conteúdo da versão.</span><span class="sxs-lookup"><span data-stu-id="78071-144">The content stream of the version.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/driveItemVersion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
