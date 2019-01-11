---
title: Tipo de recurso BaseItemVersion
description: O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.
localization_priority: Normal
ms.openlocfilehash: bd28f9c8dc5be2bc6422aca2eb756aba78b8e393
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876962"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="90ae0-103">Tipo de recurso BaseItemVersion</span><span class="sxs-lookup"><span data-stu-id="90ae0-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="90ae0-104">O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="90ae0-104">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="90ae0-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90ae0-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="90ae0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90ae0-106">Properties</span></span>

|      <span data-ttu-id="90ae0-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="90ae0-107">Property name</span></span>       |                         <span data-ttu-id="90ae0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="90ae0-108">Type</span></span>                         |                               <span data-ttu-id="90ae0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="90ae0-109">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="90ae0-110">**id**</span><span class="sxs-lookup"><span data-stu-id="90ae0-110">**id**</span></span>                   | <span data-ttu-id="90ae0-111">string</span><span class="sxs-lookup"><span data-stu-id="90ae0-111">string</span></span>                                               | <span data-ttu-id="90ae0-112">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="90ae0-112">The ID of the version.</span></span> <span data-ttu-id="90ae0-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90ae0-113">Read-only.</span></span>                                       |
| <span data-ttu-id="90ae0-114">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="90ae0-114">**lastModifiedBy**</span></span>       | [<span data-ttu-id="90ae0-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="90ae0-115">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="90ae0-116">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="90ae0-116">Identity of the user which last modified the version.</span></span> <span data-ttu-id="90ae0-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90ae0-117">Read-only.</span></span>        |
| <span data-ttu-id="90ae0-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="90ae0-118">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="90ae0-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90ae0-119">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="90ae0-120">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="90ae0-120">Date and time the version was last modified.</span></span> <span data-ttu-id="90ae0-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90ae0-121">Read-only.</span></span>                 |
| <span data-ttu-id="90ae0-122">**publication**</span><span class="sxs-lookup"><span data-stu-id="90ae0-122">**publication**</span></span>          | [<span data-ttu-id="90ae0-123">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="90ae0-123">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="90ae0-124">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="90ae0-124">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="90ae0-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90ae0-125">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
