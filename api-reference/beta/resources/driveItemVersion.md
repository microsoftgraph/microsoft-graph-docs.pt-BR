---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: DriveItemVersion
ms.openlocfilehash: 6abe10a14a4995231b12cf0c828325259775ffd8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033868"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="c3982-102">Tipo de recurso DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="c3982-102">DriveItemVersion resource type</span></span>

> <span data-ttu-id="c3982-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c3982-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3982-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c3982-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3982-105">O recurso **DriveItemVersion** representa uma versão específica de um [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c3982-105">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="c3982-106">Tarefas em recursos DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="c3982-106">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="c3982-107">As tarefas a seguir estão disponíveis para recursos driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="c3982-107">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="c3982-108">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="c3982-108">Common task</span></span>             |         <span data-ttu-id="c3982-109">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="c3982-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="c3982-110">[Versões de lista][version-list]</span><span class="sxs-lookup"><span data-stu-id="c3982-110">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="c3982-111">[Obter versão][version-get]</span><span class="sxs-lookup"><span data-stu-id="c3982-111">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="c3982-112">[Obter conteúdo][content-get]</span><span class="sxs-lookup"><span data-stu-id="c3982-112">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="c3982-113">[Restaurar versão][version-restore]</span><span class="sxs-lookup"><span data-stu-id="c3982-113">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="c3982-114">Na tabela anterior, os exemplos usam `/drive`, mas há muitas solicitações válidas.</span><span class="sxs-lookup"><span data-stu-id="c3982-114">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3982-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3982-115">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c3982-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3982-116">Properties</span></span>

|      <span data-ttu-id="c3982-117">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="c3982-117">Property name</span></span>       |                         <span data-ttu-id="c3982-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3982-118">Type</span></span>                         |                               <span data-ttu-id="c3982-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3982-119">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="c3982-120">**id**</span><span class="sxs-lookup"><span data-stu-id="c3982-120">**id**</span></span>                   | <span data-ttu-id="c3982-121">string</span><span class="sxs-lookup"><span data-stu-id="c3982-121">string</span></span>                                               | <span data-ttu-id="c3982-122">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="c3982-122">The ID of the version.</span></span> <span data-ttu-id="c3982-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3982-123">Read-only.</span></span>                                       |
| <span data-ttu-id="c3982-124">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="c3982-124">**lastModifiedBy**</span></span>       | [<span data-ttu-id="c3982-125">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="c3982-125">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="c3982-126">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c3982-126">Identity of the user which last modified the version.</span></span> <span data-ttu-id="c3982-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3982-127">Read-only.</span></span>        |
| <span data-ttu-id="c3982-128">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="c3982-128">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="c3982-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3982-129">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="c3982-130">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c3982-130">Date and time the version was last modified.</span></span> <span data-ttu-id="c3982-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3982-131">Read-only.</span></span>                 |
| <span data-ttu-id="c3982-132">**publication**</span><span class="sxs-lookup"><span data-stu-id="c3982-132">**publication**</span></span>          | [<span data-ttu-id="c3982-133">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="c3982-133">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="c3982-134">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="c3982-134">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="c3982-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c3982-135">Read-only.</span></span> |
| <span data-ttu-id="c3982-136">**size**</span><span class="sxs-lookup"><span data-stu-id="c3982-136">**size**</span></span>                 | <span data-ttu-id="c3982-137">Int64</span><span class="sxs-lookup"><span data-stu-id="c3982-137">Int64</span></span>                                                | <span data-ttu-id="c3982-138">Indica o tamanho do fluxo de conteúdo para esta versão do item.</span><span class="sxs-lookup"><span data-stu-id="c3982-138">Indicates the size of the content stream for this version of the item.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="c3982-139">Relações</span><span class="sxs-lookup"><span data-stu-id="c3982-139">Relationships</span></span>

<span data-ttu-id="c3982-140">A tabela a seguir define as relações que o recurso **driveItemVersion** tem com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="c3982-140">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="c3982-141">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="c3982-141">Relationship name</span></span> |  <span data-ttu-id="c3982-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3982-142">Type</span></span>  |            <span data-ttu-id="c3982-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3982-143">Description</span></span>             |
| :---------------- | :----- | :--------------------------------- |
| <span data-ttu-id="c3982-144">**content**</span><span class="sxs-lookup"><span data-stu-id="c3982-144">**content**</span></span>       | <span data-ttu-id="c3982-145">Fluxo</span><span class="sxs-lookup"><span data-stu-id="c3982-145">Stream</span></span> | <span data-ttu-id="c3982-146">O fluxo de conteúdo da versão.</span><span class="sxs-lookup"><span data-stu-id="c3982-146">The content stream of the version.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->