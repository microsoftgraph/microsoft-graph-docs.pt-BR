---
title: Tipo de recurso BaseItemVersion
description: O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6d74356e20bcc634f2ce9c5e943aa8a53e5f4242
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532012"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="f43d8-103">Tipo de recurso BaseItemVersion</span><span class="sxs-lookup"><span data-stu-id="f43d8-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="f43d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f43d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f43d8-105">O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="f43d8-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f43d8-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f43d8-106">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="f43d8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f43d8-107">Properties</span></span>

|      <span data-ttu-id="f43d8-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="f43d8-108">Property name</span></span>       |                         <span data-ttu-id="f43d8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f43d8-109">Type</span></span>                         |                               <span data-ttu-id="f43d8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f43d8-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="f43d8-111">**id**</span><span class="sxs-lookup"><span data-stu-id="f43d8-111">**id**</span></span>                   | <span data-ttu-id="f43d8-112">string</span><span class="sxs-lookup"><span data-stu-id="f43d8-112">string</span></span>                                               | <span data-ttu-id="f43d8-113">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="f43d8-113">The ID of the version.</span></span> <span data-ttu-id="f43d8-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f43d8-114">Read-only.</span></span>                                       |
| <span data-ttu-id="f43d8-115">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="f43d8-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="f43d8-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="f43d8-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="f43d8-117">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f43d8-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="f43d8-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f43d8-118">Read-only.</span></span>        |
| <span data-ttu-id="f43d8-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="f43d8-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="f43d8-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f43d8-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="f43d8-121">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f43d8-121">Date and time the version was last modified.</span></span> <span data-ttu-id="f43d8-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f43d8-122">Read-only.</span></span>                 |
| <span data-ttu-id="f43d8-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="f43d8-123">**publication**</span></span>          | [<span data-ttu-id="f43d8-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="f43d8-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="f43d8-125">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="f43d8-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="f43d8-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f43d8-126">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
