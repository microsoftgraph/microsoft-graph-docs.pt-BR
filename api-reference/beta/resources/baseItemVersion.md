---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
ms.openlocfilehash: fcf427300007277f7ea6382579ad3a0929ca97d1
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643021"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="14282-102">Tipo de recurso BaseItemVersion</span><span class="sxs-lookup"><span data-stu-id="14282-102">BaseItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14282-103">O recurso **baseItemVersion** representa uma versão anterior de um item ou de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="14282-103">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="14282-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14282-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="14282-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14282-105">Properties</span></span>

|      <span data-ttu-id="14282-106">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="14282-106">Property name</span></span>       |                         <span data-ttu-id="14282-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="14282-107">Type</span></span>                         |                               <span data-ttu-id="14282-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="14282-108">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="14282-109">**id**</span><span class="sxs-lookup"><span data-stu-id="14282-109">**id**</span></span>                   | <span data-ttu-id="14282-110">string</span><span class="sxs-lookup"><span data-stu-id="14282-110">string</span></span>                                               | <span data-ttu-id="14282-111">A ID da versão.</span><span class="sxs-lookup"><span data-stu-id="14282-111">The ID of the version.</span></span> <span data-ttu-id="14282-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="14282-112">Read-only.</span></span>                                       |
| <span data-ttu-id="14282-113">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="14282-113">**lastModifiedBy**</span></span>       | [<span data-ttu-id="14282-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="14282-114">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="14282-115">Identidade do usuário que modificou a versão pela última vez.</span><span class="sxs-lookup"><span data-stu-id="14282-115">Identity of the user which last modified the version.</span></span> <span data-ttu-id="14282-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="14282-116">Read-only.</span></span>        |
| <span data-ttu-id="14282-117">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="14282-117">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="14282-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14282-118">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="14282-119">Data e hora em que a versão foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="14282-119">Date and time the version was last modified.</span></span> <span data-ttu-id="14282-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="14282-120">Read-only.</span></span>                 |
| <span data-ttu-id="14282-121">**publication**</span><span class="sxs-lookup"><span data-stu-id="14282-121">**publication**</span></span>          | [<span data-ttu-id="14282-122">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="14282-122">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="14282-123">Indica o status de publicação desta versão específica.</span><span class="sxs-lookup"><span data-stu-id="14282-123">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="14282-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="14282-124">Read-only.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/baseItemVersion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
