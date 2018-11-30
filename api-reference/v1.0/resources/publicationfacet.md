---
title: Tipo de recurso PublicationFacet
description: O recurso **publicationFacet** fornece detalhes sobre o status de publicado em um recurso driveItemVersion ou driveItem.
ms.openlocfilehash: 429ec649dc9f511a4012e6790842fdd774bead8b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003999"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="46b5f-103">Tipo de recurso PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="46b5f-103">PublicationFacet resource type</span></span>

<span data-ttu-id="46b5f-104">O recurso **publicationFacet** fornece detalhes sobre o status de publicado em um recurso [driveItemVersion](driveitemversion.md) ou [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="46b5f-104">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="46b5f-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46b5f-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="46b5f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46b5f-106">Properties</span></span>

|   <span data-ttu-id="46b5f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46b5f-107">Property</span></span>    |  <span data-ttu-id="46b5f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="46b5f-108">Type</span></span>  | <span data-ttu-id="46b5f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="46b5f-109">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="46b5f-110">**level**</span><span class="sxs-lookup"><span data-stu-id="46b5f-110">**level**</span></span>     | <span data-ttu-id="46b5f-111">String</span><span class="sxs-lookup"><span data-stu-id="46b5f-111">String</span></span> | <span data-ttu-id="46b5f-112">O estado de publicação deste documento.</span><span class="sxs-lookup"><span data-stu-id="46b5f-112">The state of publication for this document.</span></span> <span data-ttu-id="46b5f-113">Pode ser `published` ou `checkout`.</span><span class="sxs-lookup"><span data-stu-id="46b5f-113">Either `published` or `checkout`.</span></span> <span data-ttu-id="46b5f-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46b5f-114">Read-only.</span></span>  |
| <span data-ttu-id="46b5f-115">**versionId**</span><span class="sxs-lookup"><span data-stu-id="46b5f-115">**versionId**</span></span> | <span data-ttu-id="46b5f-116">String</span><span class="sxs-lookup"><span data-stu-id="46b5f-116">String</span></span> | <span data-ttu-id="46b5f-117">O identificador exclusivo da versão fica visível para o chamador atual.</span><span class="sxs-lookup"><span data-stu-id="46b5f-117">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="46b5f-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46b5f-118">Read-only.</span></span>  |


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
