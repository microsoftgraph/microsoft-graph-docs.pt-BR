---
title: tipo de recurso convertIdResult
description: O resultado de uma conversão de formato de ID executada pela função translateExchangeIds.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: aa663420dd7b6e1c79e03af675b1f505c08cb875
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091849"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="a64a8-103">tipo de recurso convertIdResult</span><span class="sxs-lookup"><span data-stu-id="a64a8-103">convertIdResult resource type</span></span>

<span data-ttu-id="a64a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a64a8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a64a8-105">O resultado de uma conversão de formato de ID executada pela função [translateExchangeIds](../api/user-translateexchangeids.md) .</span><span class="sxs-lookup"><span data-stu-id="a64a8-105">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="a64a8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a64a8-106">Properties</span></span>

| <span data-ttu-id="a64a8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a64a8-107">Property</span></span> | <span data-ttu-id="a64a8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a64a8-108">Type</span></span> | <span data-ttu-id="a64a8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a64a8-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="a64a8-110">sourceId</span><span class="sxs-lookup"><span data-stu-id="a64a8-110">sourceId</span></span> | <span data-ttu-id="a64a8-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a64a8-111">String</span></span> | <span data-ttu-id="a64a8-112">O identificador que foi convertido.</span><span class="sxs-lookup"><span data-stu-id="a64a8-112">The identifier that was converted.</span></span> <span data-ttu-id="a64a8-113">Esse valor é o identificador original não convertido.</span><span class="sxs-lookup"><span data-stu-id="a64a8-113">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="a64a8-114">targetId</span><span class="sxs-lookup"><span data-stu-id="a64a8-114">targetId</span></span> | <span data-ttu-id="a64a8-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a64a8-115">String</span></span> | <span data-ttu-id="a64a8-116">O identificador convertido.</span><span class="sxs-lookup"><span data-stu-id="a64a8-116">The converted identifier.</span></span> <span data-ttu-id="a64a8-117">Esse valor não estará presente se a conversão tiver falhado.</span><span class="sxs-lookup"><span data-stu-id="a64a8-117">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="a64a8-118">errorDetails</span><span class="sxs-lookup"><span data-stu-id="a64a8-118">errorDetails</span></span> | [<span data-ttu-id="a64a8-119">genericError</span><span class="sxs-lookup"><span data-stu-id="a64a8-119">genericError</span></span>](genericerror.md) | <span data-ttu-id="a64a8-120">Um objeto Error que indica o motivo da falha de conversão.</span><span class="sxs-lookup"><span data-stu-id="a64a8-120">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="a64a8-121">Esse valor não estará presente se a conversão tiver sido bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="a64a8-121">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a64a8-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a64a8-122">JSON representation</span></span>

<span data-ttu-id="a64a8-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a64a8-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```

