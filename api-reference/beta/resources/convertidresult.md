---
title: Tipo de recurso convertIdResult
description: O resultado de uma conversão de formato de ID executada pela função translateExchangeIds.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: eafc37f017c7f074c971d12b3b8e16d8da24b850
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136768"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="b6072-103">Tipo de recurso convertIdResult</span><span class="sxs-lookup"><span data-stu-id="b6072-103">convertIdResult resource type</span></span>

<span data-ttu-id="b6072-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6072-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6072-105">O resultado de uma conversão de formato de ID executada pela [função translateExchangeIds.](../api/user-translateexchangeids.md)</span><span class="sxs-lookup"><span data-stu-id="b6072-105">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="b6072-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6072-106">Properties</span></span>

| <span data-ttu-id="b6072-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6072-107">Property</span></span> | <span data-ttu-id="b6072-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6072-108">Type</span></span> | <span data-ttu-id="b6072-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6072-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="b6072-110">sourceId</span><span class="sxs-lookup"><span data-stu-id="b6072-110">sourceId</span></span> | <span data-ttu-id="b6072-111">String</span><span class="sxs-lookup"><span data-stu-id="b6072-111">String</span></span> | <span data-ttu-id="b6072-112">O identificador que foi convertido.</span><span class="sxs-lookup"><span data-stu-id="b6072-112">The identifier that was converted.</span></span> <span data-ttu-id="b6072-113">Esse valor é o identificador original não convertido.</span><span class="sxs-lookup"><span data-stu-id="b6072-113">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="b6072-114">targetId</span><span class="sxs-lookup"><span data-stu-id="b6072-114">targetId</span></span> | <span data-ttu-id="b6072-115">String</span><span class="sxs-lookup"><span data-stu-id="b6072-115">String</span></span> | <span data-ttu-id="b6072-116">O identificador convertido.</span><span class="sxs-lookup"><span data-stu-id="b6072-116">The converted identifier.</span></span> <span data-ttu-id="b6072-117">Esse valor não estará presente se a conversão falhar.</span><span class="sxs-lookup"><span data-stu-id="b6072-117">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="b6072-118">errorDetails</span><span class="sxs-lookup"><span data-stu-id="b6072-118">errorDetails</span></span> | [<span data-ttu-id="b6072-119">genericError</span><span class="sxs-lookup"><span data-stu-id="b6072-119">genericError</span></span>](genericerror.md) | <span data-ttu-id="b6072-120">Um objeto de erro indicando o motivo da falha de conversão.</span><span class="sxs-lookup"><span data-stu-id="b6072-120">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="b6072-121">Esse valor não estará presente se a conversão tiver êxito.</span><span class="sxs-lookup"><span data-stu-id="b6072-121">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b6072-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6072-122">JSON representation</span></span>

<span data-ttu-id="b6072-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6072-123">Here is a JSON representation of the resource.</span></span>

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


