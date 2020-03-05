---
title: Tipo de recurso PublicationFacet
description: O recurso **publicationFacet** fornece detalhes sobre o status de publicado em um recurso driveItemVersion ou driveItem.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: defd2c9b06a0d866ce43bbd4a9e8b36bdad770fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447035"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="9cd13-103">Tipo de recurso PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="9cd13-103">PublicationFacet resource type</span></span>

<span data-ttu-id="9cd13-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9cd13-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9cd13-105">O recurso **publicationFacet** fornece detalhes sobre o status de publicado em um recurso [driveItemVersion](driveitemversion.md) ou [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="9cd13-105">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9cd13-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9cd13-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="9cd13-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9cd13-107">Properties</span></span>

|   <span data-ttu-id="9cd13-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9cd13-108">Property</span></span>    |  <span data-ttu-id="9cd13-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cd13-109">Type</span></span>  | <span data-ttu-id="9cd13-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cd13-110">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="9cd13-111">**level**</span><span class="sxs-lookup"><span data-stu-id="9cd13-111">**level**</span></span>     | <span data-ttu-id="9cd13-112">String</span><span class="sxs-lookup"><span data-stu-id="9cd13-112">String</span></span> | <span data-ttu-id="9cd13-113">O estado de publicação deste documento.</span><span class="sxs-lookup"><span data-stu-id="9cd13-113">The state of publication for this document.</span></span> <span data-ttu-id="9cd13-114">Pode ser `published` ou `checkout`.</span><span class="sxs-lookup"><span data-stu-id="9cd13-114">Either `published` or `checkout`.</span></span> <span data-ttu-id="9cd13-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9cd13-115">Read-only.</span></span>  |
| <span data-ttu-id="9cd13-116">**versionId**</span><span class="sxs-lookup"><span data-stu-id="9cd13-116">**versionId**</span></span> | <span data-ttu-id="9cd13-117">String</span><span class="sxs-lookup"><span data-stu-id="9cd13-117">String</span></span> | <span data-ttu-id="9cd13-118">O identificador exclusivo da versão fica visível para o chamador atual.</span><span class="sxs-lookup"><span data-stu-id="9cd13-118">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="9cd13-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9cd13-119">Read-only.</span></span>  |


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
