---
title: Tipo de recurso convertIdResult
description: O resultado de uma conversão de formato de ID executada pela função translateExchangeIds.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 1710c437421426b4bd072e3c654df7d076d0f9f7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135151"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="feab3-103">Tipo de recurso convertIdResult</span><span class="sxs-lookup"><span data-stu-id="feab3-103">convertIdResult resource type</span></span>

<span data-ttu-id="feab3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="feab3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="feab3-105">O resultado de uma conversão de formato de ID executada pela [função translateExchangeIds.](../api/user-translateexchangeids.md)</span><span class="sxs-lookup"><span data-stu-id="feab3-105">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="feab3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="feab3-106">Properties</span></span>

| <span data-ttu-id="feab3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="feab3-107">Property</span></span> | <span data-ttu-id="feab3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="feab3-108">Type</span></span> | <span data-ttu-id="feab3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="feab3-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="feab3-110">sourceId</span><span class="sxs-lookup"><span data-stu-id="feab3-110">sourceId</span></span> | <span data-ttu-id="feab3-111">String</span><span class="sxs-lookup"><span data-stu-id="feab3-111">String</span></span> | <span data-ttu-id="feab3-112">O identificador que foi convertido.</span><span class="sxs-lookup"><span data-stu-id="feab3-112">The identifier that was converted.</span></span> <span data-ttu-id="feab3-113">Esse valor é o identificador original não convertido.</span><span class="sxs-lookup"><span data-stu-id="feab3-113">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="feab3-114">targetId</span><span class="sxs-lookup"><span data-stu-id="feab3-114">targetId</span></span> | <span data-ttu-id="feab3-115">String</span><span class="sxs-lookup"><span data-stu-id="feab3-115">String</span></span> | <span data-ttu-id="feab3-116">O identificador convertido.</span><span class="sxs-lookup"><span data-stu-id="feab3-116">The converted identifier.</span></span> <span data-ttu-id="feab3-117">Esse valor não estará presente se a conversão falhar.</span><span class="sxs-lookup"><span data-stu-id="feab3-117">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="feab3-118">errorDetails</span><span class="sxs-lookup"><span data-stu-id="feab3-118">errorDetails</span></span> | [<span data-ttu-id="feab3-119">genericError</span><span class="sxs-lookup"><span data-stu-id="feab3-119">genericError</span></span>](genericerror.md) | <span data-ttu-id="feab3-120">Um objeto de erro indicando o motivo da falha de conversão.</span><span class="sxs-lookup"><span data-stu-id="feab3-120">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="feab3-121">Esse valor não estará presente se a conversão tiver êxito.</span><span class="sxs-lookup"><span data-stu-id="feab3-121">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="feab3-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="feab3-122">JSON representation</span></span>

<span data-ttu-id="feab3-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="feab3-123">Here is a JSON representation of the resource.</span></span>

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

