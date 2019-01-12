---
title: tipo de recurso de callRoute
description: O tipo de callRoute.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fd131afcdb5581a719107d9fd3a9a597979d6f21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933068"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="5f6a3-103">tipo de recurso de callRoute</span><span class="sxs-lookup"><span data-stu-id="5f6a3-103">callRoute resource type</span></span>

> <span data-ttu-id="5f6a3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5f6a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f6a3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5f6a3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f6a3-106">O tipo de callRoute.</span><span class="sxs-lookup"><span data-stu-id="5f6a3-106">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="5f6a3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f6a3-107">Properties</span></span>

| <span data-ttu-id="5f6a3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f6a3-108">Property</span></span>            | <span data-ttu-id="5f6a3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f6a3-109">Type</span></span>                          | <span data-ttu-id="5f6a3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f6a3-110">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="5f6a3-111">final</span><span class="sxs-lookup"><span data-stu-id="5f6a3-111">final</span></span>               | [<span data-ttu-id="5f6a3-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="5f6a3-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="5f6a3-113">A identidade que foi resolvida na chamada.</span><span class="sxs-lookup"><span data-stu-id="5f6a3-113">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="5f6a3-114">Original</span><span class="sxs-lookup"><span data-stu-id="5f6a3-114">original</span></span>            | [<span data-ttu-id="5f6a3-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="5f6a3-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="5f6a3-116">A identidade que originalmente utilizada na chamada.</span><span class="sxs-lookup"><span data-stu-id="5f6a3-116">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="5f6a3-117">routingType</span><span class="sxs-lookup"><span data-stu-id="5f6a3-117">routingType</span></span>         | <span data-ttu-id="5f6a3-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f6a3-118">String</span></span>                        | <span data-ttu-id="5f6a3-119">Os valores possíveis são: `forwarded`, `lookup`, `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="5f6a3-119">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="5f6a3-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f6a3-120">JSON representation</span></span>

<span data-ttu-id="5f6a3-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5f6a3-121">The following is a JSON representation of the resource.</span></span>

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
