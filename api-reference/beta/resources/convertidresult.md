---
title: tipo de recurso convertIdResult
description: O resultado de uma conversão de formato de ID executada pela função translateExchangeIds.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 3579385fa4c42da3d14914d134dd817c4de08ba5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016748"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="3974c-103">tipo de recurso convertIdResult</span><span class="sxs-lookup"><span data-stu-id="3974c-103">convertIdResult resource type</span></span>

<span data-ttu-id="3974c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3974c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3974c-105">O resultado de uma conversão de formato de ID executada pela função [translateExchangeIds](../api/user-translateexchangeids.md) .</span><span class="sxs-lookup"><span data-stu-id="3974c-105">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="3974c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3974c-106">Properties</span></span>

| <span data-ttu-id="3974c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3974c-107">Property</span></span> | <span data-ttu-id="3974c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3974c-108">Type</span></span> | <span data-ttu-id="3974c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3974c-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="3974c-110">sourceId</span><span class="sxs-lookup"><span data-stu-id="3974c-110">sourceId</span></span> | <span data-ttu-id="3974c-111">String</span><span class="sxs-lookup"><span data-stu-id="3974c-111">String</span></span> | <span data-ttu-id="3974c-112">O identificador que foi convertido.</span><span class="sxs-lookup"><span data-stu-id="3974c-112">The identifier that was converted.</span></span> <span data-ttu-id="3974c-113">Esse valor é o identificador original não convertido.</span><span class="sxs-lookup"><span data-stu-id="3974c-113">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="3974c-114">targetId</span><span class="sxs-lookup"><span data-stu-id="3974c-114">targetId</span></span> | <span data-ttu-id="3974c-115">String</span><span class="sxs-lookup"><span data-stu-id="3974c-115">String</span></span> | <span data-ttu-id="3974c-116">O identificador convertido.</span><span class="sxs-lookup"><span data-stu-id="3974c-116">The converted identifier.</span></span> <span data-ttu-id="3974c-117">Esse valor não estará presente se a conversão tiver falhado.</span><span class="sxs-lookup"><span data-stu-id="3974c-117">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="3974c-118">errorDetails</span><span class="sxs-lookup"><span data-stu-id="3974c-118">errorDetails</span></span> | [<span data-ttu-id="3974c-119">genericError</span><span class="sxs-lookup"><span data-stu-id="3974c-119">genericError</span></span>](genericerror.md) | <span data-ttu-id="3974c-120">Um objeto Error que indica o motivo da falha de conversão.</span><span class="sxs-lookup"><span data-stu-id="3974c-120">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="3974c-121">Esse valor não estará presente se a conversão tiver sido bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="3974c-121">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3974c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3974c-122">JSON representation</span></span>

<span data-ttu-id="3974c-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3974c-123">Here is a JSON representation of the resource.</span></span>

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


