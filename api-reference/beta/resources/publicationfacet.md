---
author: JeremyKelley
description: O recurso publicationFacet fornece detalhes sobre o status de publicado em um recurso driveItemVersion ou driveItem.
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9c09f0863376e1569fb4af0acc0044fa1c7c8cfa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008856"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="527a6-103">Tipo de recurso PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="527a6-103">PublicationFacet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="527a6-104">O recurso **publicationFacet** fornece detalhes sobre o status de publicado em um recurso [driveItemVersion](driveitemversion.md) ou [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="527a6-104">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="527a6-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="527a6-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="527a6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="527a6-106">Properties</span></span>

|   <span data-ttu-id="527a6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="527a6-107">Property</span></span>    |  <span data-ttu-id="527a6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="527a6-108">Type</span></span>  | <span data-ttu-id="527a6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="527a6-109">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="527a6-110">**level**</span><span class="sxs-lookup"><span data-stu-id="527a6-110">**level**</span></span>     | <span data-ttu-id="527a6-111">String</span><span class="sxs-lookup"><span data-stu-id="527a6-111">String</span></span> | <span data-ttu-id="527a6-112">O estado de publicação deste documento.</span><span class="sxs-lookup"><span data-stu-id="527a6-112">The state of publication for this document.</span></span> <span data-ttu-id="527a6-113">Pode ser `published` ou `checkout`.</span><span class="sxs-lookup"><span data-stu-id="527a6-113">Either `published` or `checkout`.</span></span> <span data-ttu-id="527a6-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="527a6-114">Read-only.</span></span>  |
| <span data-ttu-id="527a6-115">**versionId**</span><span class="sxs-lookup"><span data-stu-id="527a6-115">**versionId**</span></span> | <span data-ttu-id="527a6-116">String</span><span class="sxs-lookup"><span data-stu-id="527a6-116">String</span></span> | <span data-ttu-id="527a6-117">O identificador exclusivo da versão fica visível para o chamador atual.</span><span class="sxs-lookup"><span data-stu-id="527a6-117">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="527a6-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="527a6-118">Read-only.</span></span>  |


<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": []
}
-->
