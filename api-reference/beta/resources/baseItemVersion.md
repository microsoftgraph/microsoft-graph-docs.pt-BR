---
author: JeremyKelley
description: O recurso baseItemVersion representa uma versão anterior de um item ou de uma entidade.
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 47865e388616763b60ce3cd45195bf9919c7acf2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508035"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="3cb06-103">Tipo de recurso BaseItemVersion</span><span class="sxs-lookup"><span data-stu-id="3cb06-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="3cb06-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3cb06-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cb06-105">O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="3cb06-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="3cb06-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3cb06-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.baseItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="3cb06-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3cb06-107">Properties</span></span>

|      <span data-ttu-id="3cb06-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="3cb06-108">Property name</span></span>       |                         <span data-ttu-id="3cb06-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cb06-109">Type</span></span>                         |                               <span data-ttu-id="3cb06-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cb06-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="3cb06-111">**id**</span><span class="sxs-lookup"><span data-stu-id="3cb06-111">**id**</span></span>                   | <span data-ttu-id="3cb06-112">string</span><span class="sxs-lookup"><span data-stu-id="3cb06-112">string</span></span>                                               | <span data-ttu-id="3cb06-113">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="3cb06-113">The ID of the version.</span></span> <span data-ttu-id="3cb06-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3cb06-114">Read-only.</span></span>                                       |
| <span data-ttu-id="3cb06-115">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="3cb06-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="3cb06-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="3cb06-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="3cb06-117">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3cb06-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="3cb06-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3cb06-118">Read-only.</span></span>        |
| <span data-ttu-id="3cb06-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="3cb06-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="3cb06-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cb06-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="3cb06-121">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3cb06-121">Date and time the version was last modified.</span></span> <span data-ttu-id="3cb06-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3cb06-122">Read-only.</span></span>                 |
| <span data-ttu-id="3cb06-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="3cb06-123">**publication**</span></span>          | [<span data-ttu-id="3cb06-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="3cb06-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="3cb06-125">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="3cb06-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="3cb06-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3cb06-126">Read-only.</span></span> |


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
