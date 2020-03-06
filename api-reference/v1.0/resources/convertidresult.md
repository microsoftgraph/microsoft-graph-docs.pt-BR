---
title: tipo de recurso convertIdResult
description: O resultado de uma conversão de formato de ID executada pela função translateExchangeIds.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 6eb66033ef1b0e345c3929982b9f08d6e4ce2573
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531747"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="75d78-103">tipo de recurso convertIdResult</span><span class="sxs-lookup"><span data-stu-id="75d78-103">convertIdResult resource type</span></span>

<span data-ttu-id="75d78-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75d78-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75d78-105">O resultado de uma conversão de formato de ID executada pela função [translateExchangeIds](../api/user-translateexchangeids.md) .</span><span class="sxs-lookup"><span data-stu-id="75d78-105">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="75d78-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75d78-106">Properties</span></span>

| <span data-ttu-id="75d78-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75d78-107">Property</span></span> | <span data-ttu-id="75d78-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="75d78-108">Type</span></span> | <span data-ttu-id="75d78-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="75d78-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="75d78-110">sourceId</span><span class="sxs-lookup"><span data-stu-id="75d78-110">sourceId</span></span> | <span data-ttu-id="75d78-111">String</span><span class="sxs-lookup"><span data-stu-id="75d78-111">String</span></span> | <span data-ttu-id="75d78-112">O identificador que foi convertido.</span><span class="sxs-lookup"><span data-stu-id="75d78-112">The identifier that was converted.</span></span> <span data-ttu-id="75d78-113">Esse valor é o identificador original não convertido.</span><span class="sxs-lookup"><span data-stu-id="75d78-113">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="75d78-114">targetId</span><span class="sxs-lookup"><span data-stu-id="75d78-114">targetId</span></span> | <span data-ttu-id="75d78-115">String</span><span class="sxs-lookup"><span data-stu-id="75d78-115">String</span></span> | <span data-ttu-id="75d78-116">O identificador convertido.</span><span class="sxs-lookup"><span data-stu-id="75d78-116">The converted identifier.</span></span> <span data-ttu-id="75d78-117">Esse valor não estará presente se a conversão tiver falhado.</span><span class="sxs-lookup"><span data-stu-id="75d78-117">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="75d78-118">errorDetails</span><span class="sxs-lookup"><span data-stu-id="75d78-118">errorDetails</span></span> | [<span data-ttu-id="75d78-119">genericError</span><span class="sxs-lookup"><span data-stu-id="75d78-119">genericError</span></span>](genericerror.md) | <span data-ttu-id="75d78-120">Um objeto Error que indica o motivo da falha de conversão.</span><span class="sxs-lookup"><span data-stu-id="75d78-120">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="75d78-121">Esse valor não estará presente se a conversão tiver sido bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="75d78-121">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="75d78-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75d78-122">JSON representation</span></span>

<span data-ttu-id="75d78-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75d78-123">Here is a JSON representation of the resource.</span></span>

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
