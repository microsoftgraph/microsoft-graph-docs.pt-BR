---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: PublicationFacet
ms.openlocfilehash: 60dff1e0dd97073ccb7eccd7be0f51b6b77fc273
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037235"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="bf163-102">Tipo de recurso PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="bf163-102">PublicationFacet resource type</span></span>

> <span data-ttu-id="bf163-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bf163-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf163-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bf163-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf163-105">O recurso **publicationFacet** fornece detalhes sobre o status de publicado em um recurso [driveItemVersion](driveitemversion.md) ou [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="bf163-105">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf163-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bf163-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="bf163-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bf163-107">Properties</span></span>

|   <span data-ttu-id="bf163-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf163-108">Property</span></span>    |  <span data-ttu-id="bf163-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf163-109">Type</span></span>  | <span data-ttu-id="bf163-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf163-110">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="bf163-111">**level**</span><span class="sxs-lookup"><span data-stu-id="bf163-111">**level**</span></span>     | <span data-ttu-id="bf163-112">String</span><span class="sxs-lookup"><span data-stu-id="bf163-112">String</span></span> | <span data-ttu-id="bf163-113">O estado de publicação deste documento.</span><span class="sxs-lookup"><span data-stu-id="bf163-113">The state of publication for this document.</span></span> <span data-ttu-id="bf163-114">Pode ser `published` ou `checkout`.</span><span class="sxs-lookup"><span data-stu-id="bf163-114">Either `published` or `checkout`.</span></span> <span data-ttu-id="bf163-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bf163-115">Read-only.</span></span>  |
| <span data-ttu-id="bf163-116">**versionId**</span><span class="sxs-lookup"><span data-stu-id="bf163-116">**versionId**</span></span> | <span data-ttu-id="bf163-117">String</span><span class="sxs-lookup"><span data-stu-id="bf163-117">String</span></span> | <span data-ttu-id="bf163-118">O identificador exclusivo da versão fica visível para o chamador atual.</span><span class="sxs-lookup"><span data-stu-id="bf163-118">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="bf163-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bf163-119">Read-only.</span></span>  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
