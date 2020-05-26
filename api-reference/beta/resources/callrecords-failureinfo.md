---
title: tipo de recurso failureInfo
description: O tipo failureInfo
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 38ccc3094521283c6c496b1d0e35b97a6cf37199
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353613"
---
# <a name="failureinfo-resource-type"></a><span data-ttu-id="3627d-103">tipo de recurso failureInfo</span><span class="sxs-lookup"><span data-stu-id="3627d-103">failureInfo resource type</span></span>

<span data-ttu-id="3627d-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="3627d-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3627d-105">Representa informações sobre o motivo pelo qual uma chamada ou parte de uma chamada falhou.</span><span class="sxs-lookup"><span data-stu-id="3627d-105">Represents information about why a call or portion of a call failed.</span></span>

## <a name="properties"></a><span data-ttu-id="3627d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3627d-106">Properties</span></span>

| <span data-ttu-id="3627d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3627d-107">Property</span></span>     | <span data-ttu-id="3627d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3627d-108">Type</span></span>        | <span data-ttu-id="3627d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3627d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3627d-110">motivo</span><span class="sxs-lookup"><span data-stu-id="3627d-110">reason</span></span>|<span data-ttu-id="3627d-111">String</span><span class="sxs-lookup"><span data-stu-id="3627d-111">String</span></span>|<span data-ttu-id="3627d-112">Classificação de por que uma chamada ou parte de uma chamada falhou.</span><span class="sxs-lookup"><span data-stu-id="3627d-112">Classification of why a call or portion of a call failed.</span></span>|
|<span data-ttu-id="3627d-113">estágio</span><span class="sxs-lookup"><span data-stu-id="3627d-113">stage</span></span>|<span data-ttu-id="3627d-114">Microsoft. Graph. callRecords. failureStage</span><span class="sxs-lookup"><span data-stu-id="3627d-114">microsoft.graph.callRecords.failureStage</span></span>|<span data-ttu-id="3627d-115">O estágio quando a falha ocorreu.</span><span class="sxs-lookup"><span data-stu-id="3627d-115">The stage when the failure occurred.</span></span> <span data-ttu-id="3627d-116">Os valores possíveis são: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3627d-116">Possible values are: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3627d-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3627d-117">JSON representation</span></span>

<span data-ttu-id="3627d-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3627d-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.failureInfo",
  "baseType": null
}-->

```json
{
  "reason": "String",
  "stage": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "failureInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->