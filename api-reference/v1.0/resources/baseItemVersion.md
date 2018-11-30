---
title: Tipo de recurso BaseItemVersion
description: O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.
ms.openlocfilehash: c4fc95fd419bf8b2f20ab202874ca31a2b1d63f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004920"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="f31e9-103">Tipo de recurso BaseItemVersion</span><span class="sxs-lookup"><span data-stu-id="f31e9-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="f31e9-104">O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="f31e9-104">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f31e9-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f31e9-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f31e9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f31e9-106">Properties</span></span>

|      <span data-ttu-id="f31e9-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="f31e9-107">Property name</span></span>       |                         <span data-ttu-id="f31e9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f31e9-108">Type</span></span>                         |                               <span data-ttu-id="f31e9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f31e9-109">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="f31e9-110">**id**</span><span class="sxs-lookup"><span data-stu-id="f31e9-110">**id**</span></span>                   | <span data-ttu-id="f31e9-111">string</span><span class="sxs-lookup"><span data-stu-id="f31e9-111">string</span></span>                                               | <span data-ttu-id="f31e9-112">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="f31e9-112">The ID of the version.</span></span> <span data-ttu-id="f31e9-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f31e9-113">Read-only.</span></span>                                       |
| <span data-ttu-id="f31e9-114">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="f31e9-114">**lastModifiedBy**</span></span>       | [<span data-ttu-id="f31e9-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="f31e9-115">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="f31e9-116">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f31e9-116">Identity of the user which last modified the version.</span></span> <span data-ttu-id="f31e9-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f31e9-117">Read-only.</span></span>        |
| <span data-ttu-id="f31e9-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="f31e9-118">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="f31e9-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f31e9-119">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="f31e9-120">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f31e9-120">Date and time the version was last modified.</span></span> <span data-ttu-id="f31e9-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f31e9-121">Read-only.</span></span>                 |
| <span data-ttu-id="f31e9-122">**publication**</span><span class="sxs-lookup"><span data-stu-id="f31e9-122">**publication**</span></span>          | [<span data-ttu-id="f31e9-123">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="f31e9-123">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="f31e9-124">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="f31e9-124">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="f31e9-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f31e9-125">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
