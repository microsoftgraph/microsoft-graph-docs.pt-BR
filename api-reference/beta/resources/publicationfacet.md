---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
ms.openlocfilehash: 66e12c3240d1cade57d377e43403b33102fe166e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563235"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="6a025-102">Tipo de recurso PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="6a025-102">PublicationFacet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a025-103">O recurso **publicationFacet** fornece detalhes sobre o status de publicado em um recurso [driveItemVersion](driveitemversion.md) ou [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="6a025-103">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a025-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a025-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6a025-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a025-105">Properties</span></span>

|   <span data-ttu-id="6a025-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a025-106">Property</span></span>    |  <span data-ttu-id="6a025-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a025-107">Type</span></span>  | <span data-ttu-id="6a025-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a025-108">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="6a025-109">**level**</span><span class="sxs-lookup"><span data-stu-id="6a025-109">**level**</span></span>     | <span data-ttu-id="6a025-110">String</span><span class="sxs-lookup"><span data-stu-id="6a025-110">String</span></span> | <span data-ttu-id="6a025-111">O estado de publicação deste documento.</span><span class="sxs-lookup"><span data-stu-id="6a025-111">The state of publication for this document.</span></span> <span data-ttu-id="6a025-112">Pode ser `published` ou `checkout`.</span><span class="sxs-lookup"><span data-stu-id="6a025-112">Either `published` or `checkout`.</span></span> <span data-ttu-id="6a025-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a025-113">Read-only.</span></span>  |
| <span data-ttu-id="6a025-114">**versionId**</span><span class="sxs-lookup"><span data-stu-id="6a025-114">**versionId**</span></span> | <span data-ttu-id="6a025-115">String</span><span class="sxs-lookup"><span data-stu-id="6a025-115">String</span></span> | <span data-ttu-id="6a025-116">O identificador exclusivo da versão fica visível para o chamador atual.</span><span class="sxs-lookup"><span data-stu-id="6a025-116">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="6a025-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a025-117">Read-only.</span></span>  |


<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": [
    "Error: /api-reference/beta/resources/publicationfacet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
