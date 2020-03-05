---
author: JeremyKelley
description: O recurso publicationFacet fornece detalhes sobre o status de publicado em um recurso driveItemVersion ou driveItem.
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 46e5a8925e6f2521763bd1b1830e967a08df3abb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521310"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="0495d-103">Tipo de recurso PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="0495d-103">PublicationFacet resource type</span></span>

<span data-ttu-id="0495d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0495d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0495d-105">O recurso **publicationFacet** fornece detalhes sobre o status de publicado em um recurso [driveItemVersion](driveitemversion.md) ou [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0495d-105">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0495d-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0495d-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0495d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0495d-107">Properties</span></span>

|   <span data-ttu-id="0495d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0495d-108">Property</span></span>    |  <span data-ttu-id="0495d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0495d-109">Type</span></span>  | <span data-ttu-id="0495d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0495d-110">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="0495d-111">**level**</span><span class="sxs-lookup"><span data-stu-id="0495d-111">**level**</span></span>     | <span data-ttu-id="0495d-112">String</span><span class="sxs-lookup"><span data-stu-id="0495d-112">String</span></span> | <span data-ttu-id="0495d-113">O estado de publicação deste documento.</span><span class="sxs-lookup"><span data-stu-id="0495d-113">The state of publication for this document.</span></span> <span data-ttu-id="0495d-114">Pode ser `published` ou `checkout`.</span><span class="sxs-lookup"><span data-stu-id="0495d-114">Either `published` or `checkout`.</span></span> <span data-ttu-id="0495d-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0495d-115">Read-only.</span></span>  |
| <span data-ttu-id="0495d-116">**versionId**</span><span class="sxs-lookup"><span data-stu-id="0495d-116">**versionId**</span></span> | <span data-ttu-id="0495d-117">String</span><span class="sxs-lookup"><span data-stu-id="0495d-117">String</span></span> | <span data-ttu-id="0495d-118">O identificador exclusivo da versão fica visível para o chamador atual.</span><span class="sxs-lookup"><span data-stu-id="0495d-118">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="0495d-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0495d-119">Read-only.</span></span>  |


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
