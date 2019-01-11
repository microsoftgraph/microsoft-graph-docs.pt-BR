---
title: tipo de recurso de convertIdResult
description: O resultado de uma conversão de formato de ID realizada pela função translateExchangeIds.
localization_priority: Normal
ms.openlocfilehash: 7e1878de3d3b7ddee36d799c928d6a130b578200
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821452"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="39c8c-103">tipo de recurso de convertIdResult</span><span class="sxs-lookup"><span data-stu-id="39c8c-103">convertIdResult resource type</span></span>

> <span data-ttu-id="39c8c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="39c8c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39c8c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="39c8c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="39c8c-106">O resultado de uma conversão de formato de ID realizada pela função [translateExchangeIds](../api/user-translateexchangeids.md) .</span><span class="sxs-lookup"><span data-stu-id="39c8c-106">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="39c8c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="39c8c-107">Properties</span></span>

| <span data-ttu-id="39c8c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39c8c-108">Property</span></span> | <span data-ttu-id="39c8c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="39c8c-109">Type</span></span> | <span data-ttu-id="39c8c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="39c8c-110">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="39c8c-111">sourceId</span><span class="sxs-lookup"><span data-stu-id="39c8c-111">sourceId</span></span> | <span data-ttu-id="39c8c-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39c8c-112">String</span></span> | <span data-ttu-id="39c8c-113">O identificador que foi convertido.</span><span class="sxs-lookup"><span data-stu-id="39c8c-113">The identifier that was converted.</span></span> <span data-ttu-id="39c8c-114">Esse valor é o identificador original, não convertido.</span><span class="sxs-lookup"><span data-stu-id="39c8c-114">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="39c8c-115">Alvo</span><span class="sxs-lookup"><span data-stu-id="39c8c-115">targetId</span></span> | <span data-ttu-id="39c8c-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39c8c-116">String</span></span> | <span data-ttu-id="39c8c-117">O identificador convertido.</span><span class="sxs-lookup"><span data-stu-id="39c8c-117">The converted identifier.</span></span> <span data-ttu-id="39c8c-118">Este valor não estiver presente, se a conversão falhou.</span><span class="sxs-lookup"><span data-stu-id="39c8c-118">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="39c8c-119">errorDetails</span><span class="sxs-lookup"><span data-stu-id="39c8c-119">errorDetails</span></span> | [<span data-ttu-id="39c8c-120">Erro genérico</span><span class="sxs-lookup"><span data-stu-id="39c8c-120">genericError</span></span>](genericerror.md) | <span data-ttu-id="39c8c-121">Um objeto de erro que indica o motivo da falha de conversão.</span><span class="sxs-lookup"><span data-stu-id="39c8c-121">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="39c8c-122">Este valor não estiver presente, se a conversão foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="39c8c-122">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="39c8c-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="39c8c-123">JSON representation</span></span>

<span data-ttu-id="39c8c-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="39c8c-124">Here is a JSON representation of the resource.</span></span>

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
