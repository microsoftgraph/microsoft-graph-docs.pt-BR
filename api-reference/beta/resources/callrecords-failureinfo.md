---
title: tipo de recurso failureInfo
description: O tipo failureInfo
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5edd2a501b3e1a5633f0bd01ac36815201eb927d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064371"
---
# <a name="failureinfo-resource-type"></a><span data-ttu-id="fe8d7-103">tipo de recurso failureInfo</span><span class="sxs-lookup"><span data-stu-id="fe8d7-103">failureInfo resource type</span></span>

<span data-ttu-id="fe8d7-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="fe8d7-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe8d7-105">Representa informações sobre o motivo pelo qual uma chamada ou parte de uma chamada falhou.</span><span class="sxs-lookup"><span data-stu-id="fe8d7-105">Represents information about why a call or portion of a call failed.</span></span>

<span data-ttu-id="fe8d7-106">A falha pode ser de dois tipos:</span><span class="sxs-lookup"><span data-stu-id="fe8d7-106">The failure can be of two types:</span></span> 

- <span data-ttu-id="fe8d7-107">Falha de configuração de chamada</span><span class="sxs-lookup"><span data-stu-id="fe8d7-107">Call setup failure</span></span>
- <span data-ttu-id="fe8d7-108">Queda de chamada intermediário</span><span class="sxs-lookup"><span data-stu-id="fe8d7-108">Mid-call drop</span></span>

<span data-ttu-id="fe8d7-109">Se um ou mais fluxos de mídia tiverem qualquer uma dessas falhas, essa falha será propagada no nível do segmento.</span><span class="sxs-lookup"><span data-stu-id="fe8d7-109">If one or more media streams have any of these failures, that failure is propagated at the segment level.</span></span> <span data-ttu-id="fe8d7-110">Se um ou mais segmentos tiverem qualquer uma dessas falhas, essa falha será propagada no nível da sessão.</span><span class="sxs-lookup"><span data-stu-id="fe8d7-110">If one or more segments have any of these failures, that failure is propagated at the session level.</span></span>

## <a name="properties"></a><span data-ttu-id="fe8d7-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe8d7-111">Properties</span></span>

| <span data-ttu-id="fe8d7-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe8d7-112">Property</span></span>     | <span data-ttu-id="fe8d7-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe8d7-113">Type</span></span>        | <span data-ttu-id="fe8d7-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe8d7-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fe8d7-115">motivo</span><span class="sxs-lookup"><span data-stu-id="fe8d7-115">reason</span></span>|<span data-ttu-id="fe8d7-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe8d7-116">String</span></span>|<span data-ttu-id="fe8d7-117">Classificação de por que uma chamada ou parte de uma chamada falhou.</span><span class="sxs-lookup"><span data-stu-id="fe8d7-117">Classification of why a call or portion of a call failed.</span></span>|
|<span data-ttu-id="fe8d7-118">estágio</span><span class="sxs-lookup"><span data-stu-id="fe8d7-118">stage</span></span>|<span data-ttu-id="fe8d7-119">Microsoft. Graph. callRecords. failureStage</span><span class="sxs-lookup"><span data-stu-id="fe8d7-119">microsoft.graph.callRecords.failureStage</span></span>|<span data-ttu-id="fe8d7-120">O estágio quando a falha ocorreu.</span><span class="sxs-lookup"><span data-stu-id="fe8d7-120">The stage when the failure occurred.</span></span> <span data-ttu-id="fe8d7-121">Os valores possíveis são: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="fe8d7-121">Possible values are: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe8d7-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe8d7-122">JSON representation</span></span>

<span data-ttu-id="fe8d7-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe8d7-123">The following is a JSON representation of the resource.</span></span>

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


