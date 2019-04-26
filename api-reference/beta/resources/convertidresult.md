---
title: tipo de recurso convertIdResult
description: O resultado de uma conversão de formato de ID executada pela função translateExchangeIds.
localization_priority: Normal
ms.openlocfilehash: 5981f75ee071777f9119d0db2c0078153a160180
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341033"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="8358b-103">tipo de recurso convertIdResult</span><span class="sxs-lookup"><span data-stu-id="8358b-103">convertIdResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8358b-104">O resultado de uma conversão de formato de ID executada pela função [translateExchangeIds](../api/user-translateexchangeids.md) .</span><span class="sxs-lookup"><span data-stu-id="8358b-104">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="8358b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8358b-105">Properties</span></span>

| <span data-ttu-id="8358b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8358b-106">Property</span></span> | <span data-ttu-id="8358b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8358b-107">Type</span></span> | <span data-ttu-id="8358b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8358b-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="8358b-109">sourceId</span><span class="sxs-lookup"><span data-stu-id="8358b-109">sourceId</span></span> | <span data-ttu-id="8358b-110">String</span><span class="sxs-lookup"><span data-stu-id="8358b-110">String</span></span> | <span data-ttu-id="8358b-111">O identificador que foi convertido.</span><span class="sxs-lookup"><span data-stu-id="8358b-111">The identifier that was converted.</span></span> <span data-ttu-id="8358b-112">Esse valor é o identificador original não convertido.</span><span class="sxs-lookup"><span data-stu-id="8358b-112">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="8358b-113">targetId</span><span class="sxs-lookup"><span data-stu-id="8358b-113">targetId</span></span> | <span data-ttu-id="8358b-114">String</span><span class="sxs-lookup"><span data-stu-id="8358b-114">String</span></span> | <span data-ttu-id="8358b-115">O identificador convertido.</span><span class="sxs-lookup"><span data-stu-id="8358b-115">The converted identifier.</span></span> <span data-ttu-id="8358b-116">Esse valor não estará presente se a conversão tiver falhado.</span><span class="sxs-lookup"><span data-stu-id="8358b-116">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="8358b-117">errorDetails</span><span class="sxs-lookup"><span data-stu-id="8358b-117">errorDetails</span></span> | [<span data-ttu-id="8358b-118">genericError</span><span class="sxs-lookup"><span data-stu-id="8358b-118">genericError</span></span>](genericerror.md) | <span data-ttu-id="8358b-119">Um objeto Error que indica o motivo da falha de conversão.</span><span class="sxs-lookup"><span data-stu-id="8358b-119">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="8358b-120">Esse valor não estará presente se a conversão tiver sido bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="8358b-120">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8358b-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8358b-121">JSON representation</span></span>

<span data-ttu-id="8358b-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8358b-122">Here is a JSON representation of the resource.</span></span>

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
