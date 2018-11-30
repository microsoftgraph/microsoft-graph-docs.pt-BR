---
title: tipo de recurso de callRoute
description: O tipo de callRoute.
ms.openlocfilehash: d2a85d34fe755c6e725abc9a1308a3837f0acf3e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035371"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="13527-103">tipo de recurso de callRoute</span><span class="sxs-lookup"><span data-stu-id="13527-103">callRoute resource type</span></span>

> <span data-ttu-id="13527-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="13527-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13527-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="13527-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13527-106">O tipo de callRoute.</span><span class="sxs-lookup"><span data-stu-id="13527-106">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="13527-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13527-107">Properties</span></span>

| <span data-ttu-id="13527-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13527-108">Property</span></span>            | <span data-ttu-id="13527-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="13527-109">Type</span></span>                          | <span data-ttu-id="13527-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="13527-110">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="13527-111">final</span><span class="sxs-lookup"><span data-stu-id="13527-111">final</span></span>               | [<span data-ttu-id="13527-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="13527-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="13527-113">A identidade que foi resolvida na chamada.</span><span class="sxs-lookup"><span data-stu-id="13527-113">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="13527-114">Original</span><span class="sxs-lookup"><span data-stu-id="13527-114">original</span></span>            | [<span data-ttu-id="13527-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="13527-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="13527-116">A identidade que originalmente utilizada na chamada.</span><span class="sxs-lookup"><span data-stu-id="13527-116">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="13527-117">routingType</span><span class="sxs-lookup"><span data-stu-id="13527-117">routingType</span></span>         | <span data-ttu-id="13527-118">String</span><span class="sxs-lookup"><span data-stu-id="13527-118">String</span></span>                        | <span data-ttu-id="13527-119">Os valores possíveis são: `forwarded`, `lookup`, `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="13527-119">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="13527-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13527-120">JSON representation</span></span>

<span data-ttu-id="13527-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13527-121">The following is a JSON representation of the resource.</span></span>

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
