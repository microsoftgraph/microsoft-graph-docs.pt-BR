---
title: Tipo de recurso activateService
description: Representa um serviço a ser ativado.
author: dkershaw10
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a1ab2112406d0049df002327be784c46b7e879e6
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109052"
---
# <a name="activateservice-resource-type"></a><span data-ttu-id="863e4-103">Tipo de recurso activateService</span><span class="sxs-lookup"><span data-stu-id="863e4-103">activateService resource type</span></span>

<span data-ttu-id="863e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="863e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="863e4-105">Representa um serviço a ser ativado.</span><span class="sxs-lookup"><span data-stu-id="863e4-105">Represents a service to be activated.</span></span>

## <a name="properties"></a><span data-ttu-id="863e4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="863e4-106">Properties</span></span>

| <span data-ttu-id="863e4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="863e4-107">Property</span></span>         | <span data-ttu-id="863e4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="863e4-108">Type</span></span>         | <span data-ttu-id="863e4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="863e4-109">Description</span></span>                           |
| ----------------- | ------------ | ------------------------------------- |
| <span data-ttu-id="863e4-110">service</span><span class="sxs-lookup"><span data-stu-id="863e4-110">service</span></span>| <span data-ttu-id="863e4-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="863e4-111">String</span></span> | <span data-ttu-id="863e4-112">O nome do serviço a ser ativado.</span><span class="sxs-lookup"><span data-stu-id="863e4-112">The name of the service to activate.</span></span> |
| <span data-ttu-id="863e4-113">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="863e4-113">servicePlanId</span></span> | <span data-ttu-id="863e4-114">GUID</span><span class="sxs-lookup"><span data-stu-id="863e4-114">GUID</span></span> | <span data-ttu-id="863e4-115">O identificador de plano do plano de serviço a ser ativado.</span><span class="sxs-lookup"><span data-stu-id="863e4-115">The plan identifier of the service plan to activate.</span></span> |
| <span data-ttu-id="863e4-116">skuId</span><span class="sxs-lookup"><span data-stu-id="863e4-116">skuId</span></span> | <span data-ttu-id="863e4-117">GUID</span><span class="sxs-lookup"><span data-stu-id="863e4-117">GUID</span></span> | <span data-ttu-id="863e4-118">O identificador SKU do plano de serviço.</span><span class="sxs-lookup"><span data-stu-id="863e4-118">The SKU identifier of the service plan.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="863e4-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="863e4-119">JSON representation</span></span>

<span data-ttu-id="863e4-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="863e4-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activateService"
}-->

```json
{
    "service": "string",
    "skuId": "guid",
    "servicePlanId": "guid"
}

```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "activateService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
