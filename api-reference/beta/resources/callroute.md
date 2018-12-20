---
title: tipo de recurso de callRoute
description: O tipo de callRoute.
author: VinodRavichandran
ms.openlocfilehash: 9538fb8f27f60e869c19edc7bd19d7f6b29e8fff
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380153"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="2983e-103">tipo de recurso de callRoute</span><span class="sxs-lookup"><span data-stu-id="2983e-103">callRoute resource type</span></span>

> <span data-ttu-id="2983e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2983e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2983e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2983e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2983e-106">O tipo de callRoute.</span><span class="sxs-lookup"><span data-stu-id="2983e-106">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="2983e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2983e-107">Properties</span></span>

| <span data-ttu-id="2983e-108">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="2983e-108">Property</span></span>            | <span data-ttu-id="2983e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2983e-109">Type</span></span>                          | <span data-ttu-id="2983e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2983e-110">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="2983e-111">final</span><span class="sxs-lookup"><span data-stu-id="2983e-111">final</span></span>               | [<span data-ttu-id="2983e-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="2983e-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="2983e-113">A identidade que foi resolvida na chamada.</span><span class="sxs-lookup"><span data-stu-id="2983e-113">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="2983e-114">Original</span><span class="sxs-lookup"><span data-stu-id="2983e-114">original</span></span>            | [<span data-ttu-id="2983e-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="2983e-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="2983e-116">A identidade que originalmente utilizada na chamada.</span><span class="sxs-lookup"><span data-stu-id="2983e-116">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="2983e-117">routingType</span><span class="sxs-lookup"><span data-stu-id="2983e-117">routingType</span></span>         | <span data-ttu-id="2983e-118">String</span><span class="sxs-lookup"><span data-stu-id="2983e-118">String</span></span>                        | <span data-ttu-id="2983e-119">Os valores possíveis são: `forwarded`, `lookup`, `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="2983e-119">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="2983e-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2983e-120">JSON representation</span></span>

<span data-ttu-id="2983e-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2983e-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
