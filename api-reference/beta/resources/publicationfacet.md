---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
ms.openlocfilehash: a95ec524b8e33ce65d9ecb7030a90a49305cdf6c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344051"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="5710c-102">Tipo de recurso PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="5710c-102">PublicationFacet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5710c-103">O recurso **publicationFacet** fornece detalhes sobre o status de publicado em um recurso [driveItemVersion](driveitemversion.md) ou [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="5710c-103">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5710c-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5710c-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="5710c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5710c-105">Properties</span></span>

|   <span data-ttu-id="5710c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5710c-106">Property</span></span>    |  <span data-ttu-id="5710c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5710c-107">Type</span></span>  | <span data-ttu-id="5710c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5710c-108">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="5710c-109">**level**</span><span class="sxs-lookup"><span data-stu-id="5710c-109">**level**</span></span>     | <span data-ttu-id="5710c-110">String</span><span class="sxs-lookup"><span data-stu-id="5710c-110">String</span></span> | <span data-ttu-id="5710c-111">O estado de publicação deste documento.</span><span class="sxs-lookup"><span data-stu-id="5710c-111">The state of publication for this document.</span></span> <span data-ttu-id="5710c-112">Pode ser `published` ou `checkout`.</span><span class="sxs-lookup"><span data-stu-id="5710c-112">Either `published` or `checkout`.</span></span> <span data-ttu-id="5710c-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5710c-113">Read-only.</span></span>  |
| <span data-ttu-id="5710c-114">**versionId**</span><span class="sxs-lookup"><span data-stu-id="5710c-114">**versionId**</span></span> | <span data-ttu-id="5710c-115">String</span><span class="sxs-lookup"><span data-stu-id="5710c-115">String</span></span> | <span data-ttu-id="5710c-116">O identificador exclusivo da versão fica visível para o chamador atual.</span><span class="sxs-lookup"><span data-stu-id="5710c-116">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="5710c-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5710c-117">Read-only.</span></span>  |


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
