---
title: tipo de recurso convertIdResult
description: O resultado de uma conversão de formato de ID executada pela função translateExchangeIds.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 405d663e4f1f7fb040e79cdd10669bc824e3edef
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036442"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="28e1e-103">tipo de recurso convertIdResult</span><span class="sxs-lookup"><span data-stu-id="28e1e-103">convertIdResult resource type</span></span>

<span data-ttu-id="28e1e-104">O resultado de uma conversão de formato de ID executada pela função [translateExchangeIds](../api/user-translateexchangeids.md) .</span><span class="sxs-lookup"><span data-stu-id="28e1e-104">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="28e1e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28e1e-105">Properties</span></span>

| <span data-ttu-id="28e1e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28e1e-106">Property</span></span> | <span data-ttu-id="28e1e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="28e1e-107">Type</span></span> | <span data-ttu-id="28e1e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="28e1e-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="28e1e-109">sourceId</span><span class="sxs-lookup"><span data-stu-id="28e1e-109">sourceId</span></span> | <span data-ttu-id="28e1e-110">String</span><span class="sxs-lookup"><span data-stu-id="28e1e-110">String</span></span> | <span data-ttu-id="28e1e-111">O identificador que foi convertido.</span><span class="sxs-lookup"><span data-stu-id="28e1e-111">The identifier that was converted.</span></span> <span data-ttu-id="28e1e-112">Esse valor é o identificador original não convertido.</span><span class="sxs-lookup"><span data-stu-id="28e1e-112">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="28e1e-113">targetId</span><span class="sxs-lookup"><span data-stu-id="28e1e-113">targetId</span></span> | <span data-ttu-id="28e1e-114">String</span><span class="sxs-lookup"><span data-stu-id="28e1e-114">String</span></span> | <span data-ttu-id="28e1e-115">O identificador convertido.</span><span class="sxs-lookup"><span data-stu-id="28e1e-115">The converted identifier.</span></span> <span data-ttu-id="28e1e-116">Esse valor não estará presente se a conversão tiver falhado.</span><span class="sxs-lookup"><span data-stu-id="28e1e-116">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="28e1e-117">errorDetails</span><span class="sxs-lookup"><span data-stu-id="28e1e-117">errorDetails</span></span> | [<span data-ttu-id="28e1e-118">genericError</span><span class="sxs-lookup"><span data-stu-id="28e1e-118">genericError</span></span>](genericerror.md) | <span data-ttu-id="28e1e-119">Um objeto Error que indica o motivo da falha de conversão.</span><span class="sxs-lookup"><span data-stu-id="28e1e-119">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="28e1e-120">Esse valor não estará presente se a conversão tiver sido bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="28e1e-120">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="28e1e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28e1e-121">JSON representation</span></span>

<span data-ttu-id="28e1e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="28e1e-122">Here is a JSON representation of the resource.</span></span>

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
