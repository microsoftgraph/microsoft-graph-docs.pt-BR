---
title: Tipo de recurso PublicationFacet
description: O recurso **publicationFacet** fornece detalhes sobre o status de publicado em um recurso driveItemVersion ou driveItem.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5189b578d0a996ceb27014d2c5400e508e1e8a56
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034948"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="5f7a4-103">Tipo de recurso PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="5f7a4-103">PublicationFacet resource type</span></span>

<span data-ttu-id="5f7a4-104">O recurso **publicationFacet** fornece detalhes sobre o status de publicado em um recurso [driveItemVersion](driveitemversion.md) ou [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="5f7a4-104">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f7a4-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f7a4-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.publicationFacet"
}-->

```json
{
  "level": "published | checkout",
  "versionId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="5f7a4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f7a4-106">Properties</span></span>

|   <span data-ttu-id="5f7a4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f7a4-107">Property</span></span>    |  <span data-ttu-id="5f7a4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f7a4-108">Type</span></span>  | <span data-ttu-id="5f7a4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f7a4-109">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="5f7a4-110">**level**</span><span class="sxs-lookup"><span data-stu-id="5f7a4-110">**level**</span></span>     | <span data-ttu-id="5f7a4-111">String</span><span class="sxs-lookup"><span data-stu-id="5f7a4-111">String</span></span> | <span data-ttu-id="5f7a4-112">O estado de publicação deste documento.</span><span class="sxs-lookup"><span data-stu-id="5f7a4-112">The state of publication for this document.</span></span> <span data-ttu-id="5f7a4-113">Pode ser `published` ou `checkout`.</span><span class="sxs-lookup"><span data-stu-id="5f7a4-113">Either `published` or `checkout`.</span></span> <span data-ttu-id="5f7a4-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f7a4-114">Read-only.</span></span>  |
| <span data-ttu-id="5f7a4-115">**versionId**</span><span class="sxs-lookup"><span data-stu-id="5f7a4-115">**versionId**</span></span> | <span data-ttu-id="5f7a4-116">String</span><span class="sxs-lookup"><span data-stu-id="5f7a4-116">String</span></span> | <span data-ttu-id="5f7a4-117">O identificador exclusivo da versão fica visível para o chamador atual.</span><span class="sxs-lookup"><span data-stu-id="5f7a4-117">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="5f7a4-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f7a4-118">Read-only.</span></span>  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "suppressions": [
    " Warning: /api-reference/v1.0/resources/publicationfacet.md:
      Found potential enums in resource example that weren't defined in a table:(published,checkout) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Photo"
} -->
