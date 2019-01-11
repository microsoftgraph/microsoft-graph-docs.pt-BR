---
title: tipo de recurso de callRoute
description: O tipo de callRoute.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: e417a7e814b5a2a80da1fa9cd7a551f82e0c37db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815082"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="650e7-103">tipo de recurso de callRoute</span><span class="sxs-lookup"><span data-stu-id="650e7-103">callRoute resource type</span></span>

> <span data-ttu-id="650e7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="650e7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="650e7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="650e7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="650e7-106">O tipo de callRoute.</span><span class="sxs-lookup"><span data-stu-id="650e7-106">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="650e7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="650e7-107">Properties</span></span>

| <span data-ttu-id="650e7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="650e7-108">Property</span></span>            | <span data-ttu-id="650e7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="650e7-109">Type</span></span>                          | <span data-ttu-id="650e7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="650e7-110">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="650e7-111">final</span><span class="sxs-lookup"><span data-stu-id="650e7-111">final</span></span>               | [<span data-ttu-id="650e7-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="650e7-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="650e7-113">A identidade que foi resolvida na chamada.</span><span class="sxs-lookup"><span data-stu-id="650e7-113">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="650e7-114">Original</span><span class="sxs-lookup"><span data-stu-id="650e7-114">original</span></span>            | [<span data-ttu-id="650e7-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="650e7-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="650e7-116">A identidade que originalmente utilizada na chamada.</span><span class="sxs-lookup"><span data-stu-id="650e7-116">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="650e7-117">routingType</span><span class="sxs-lookup"><span data-stu-id="650e7-117">routingType</span></span>         | <span data-ttu-id="650e7-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="650e7-118">String</span></span>                        | <span data-ttu-id="650e7-119">Os valores possíveis são: `forwarded`, `lookup`, `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="650e7-119">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="650e7-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="650e7-120">JSON representation</span></span>

<span data-ttu-id="650e7-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="650e7-121">The following is a JSON representation of the resource.</span></span>

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
