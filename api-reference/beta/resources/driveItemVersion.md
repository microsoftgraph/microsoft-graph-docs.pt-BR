---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: DriveItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3f33c59da4a748c176c6044e4db3bac70eac71cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923611"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="51a48-102">Tipo de recurso DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="51a48-102">DriveItemVersion resource type</span></span>

> <span data-ttu-id="51a48-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="51a48-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51a48-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="51a48-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51a48-105">O recurso **DriveItemVersion** representa uma versão específica de um [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="51a48-105">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="51a48-106">Tarefas em recursos DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="51a48-106">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="51a48-107">As tarefas a seguir estão disponíveis para recursos driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="51a48-107">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="51a48-108">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="51a48-108">Common task</span></span>             |         <span data-ttu-id="51a48-109">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="51a48-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="51a48-110">[Versões de lista][version-list]</span><span class="sxs-lookup"><span data-stu-id="51a48-110">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="51a48-111">[Obter versão][version-get]</span><span class="sxs-lookup"><span data-stu-id="51a48-111">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="51a48-112">[Obter conteúdo][content-get]</span><span class="sxs-lookup"><span data-stu-id="51a48-112">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="51a48-113">[Restaurar versão][version-restore]</span><span class="sxs-lookup"><span data-stu-id="51a48-113">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="51a48-114">Na tabela anterior, os exemplos usam `/drive`, mas há muitas solicitações válidas.</span><span class="sxs-lookup"><span data-stu-id="51a48-114">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="51a48-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51a48-115">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="51a48-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51a48-116">Properties</span></span>

|      <span data-ttu-id="51a48-117">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="51a48-117">Property name</span></span>       |                         <span data-ttu-id="51a48-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="51a48-118">Type</span></span>                         |                               <span data-ttu-id="51a48-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="51a48-119">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="51a48-120">**id**</span><span class="sxs-lookup"><span data-stu-id="51a48-120">**id**</span></span>                   | <span data-ttu-id="51a48-121">string</span><span class="sxs-lookup"><span data-stu-id="51a48-121">string</span></span>                                               | <span data-ttu-id="51a48-122">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="51a48-122">The ID of the version.</span></span> <span data-ttu-id="51a48-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51a48-123">Read-only.</span></span>                                       |
| <span data-ttu-id="51a48-124">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="51a48-124">**lastModifiedBy**</span></span>       | [<span data-ttu-id="51a48-125">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="51a48-125">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="51a48-126">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="51a48-126">Identity of the user which last modified the version.</span></span> <span data-ttu-id="51a48-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51a48-127">Read-only.</span></span>        |
| <span data-ttu-id="51a48-128">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="51a48-128">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="51a48-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51a48-129">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="51a48-130">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="51a48-130">Date and time the version was last modified.</span></span> <span data-ttu-id="51a48-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51a48-131">Read-only.</span></span>                 |
| <span data-ttu-id="51a48-132">**publication**</span><span class="sxs-lookup"><span data-stu-id="51a48-132">**publication**</span></span>          | [<span data-ttu-id="51a48-133">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="51a48-133">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="51a48-134">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="51a48-134">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="51a48-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51a48-135">Read-only.</span></span> |
| <span data-ttu-id="51a48-136">**size**</span><span class="sxs-lookup"><span data-stu-id="51a48-136">**size**</span></span>                 | <span data-ttu-id="51a48-137">Int64</span><span class="sxs-lookup"><span data-stu-id="51a48-137">Int64</span></span>                                                | <span data-ttu-id="51a48-138">Indica o tamanho do fluxo de conteúdo para esta versão do item.</span><span class="sxs-lookup"><span data-stu-id="51a48-138">Indicates the size of the content stream for this version of the item.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="51a48-139">Relações</span><span class="sxs-lookup"><span data-stu-id="51a48-139">Relationships</span></span>

<span data-ttu-id="51a48-140">A tabela a seguir define as relações que o recurso **driveItemVersion** tem com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="51a48-140">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="51a48-141">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="51a48-141">Relationship name</span></span> |  <span data-ttu-id="51a48-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="51a48-142">Type</span></span>  |            <span data-ttu-id="51a48-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="51a48-143">Description</span></span>             |
| :---------------- | :----- | :--------------------------------- |
| <span data-ttu-id="51a48-144">**content**</span><span class="sxs-lookup"><span data-stu-id="51a48-144">**content**</span></span>       | <span data-ttu-id="51a48-145">Fluxo</span><span class="sxs-lookup"><span data-stu-id="51a48-145">Stream</span></span> | <span data-ttu-id="51a48-146">O fluxo de conteúdo da versão.</span><span class="sxs-lookup"><span data-stu-id="51a48-146">The content stream of the version.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
