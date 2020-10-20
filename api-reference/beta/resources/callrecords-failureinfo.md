---
title: tipo de recurso failureInfo
description: O tipo failureInfo
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e67e0df2c3f98ea2c9c1b49d32cb6295559516dd
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601185"
---
# <a name="failureinfo-resource-type"></a><span data-ttu-id="c4ab4-103">tipo de recurso failureInfo</span><span class="sxs-lookup"><span data-stu-id="c4ab4-103">failureInfo resource type</span></span>

<span data-ttu-id="c4ab4-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="c4ab4-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4ab4-105">Representa informações sobre o motivo pelo qual uma chamada ou parte de uma chamada falhou.</span><span class="sxs-lookup"><span data-stu-id="c4ab4-105">Represents information about why a call or portion of a call failed.</span></span>

<span data-ttu-id="c4ab4-106">A falha pode ser de dois tipos:</span><span class="sxs-lookup"><span data-stu-id="c4ab4-106">The failure can be of two types:</span></span> 

- <span data-ttu-id="c4ab4-107">Falha de configuração de chamada</span><span class="sxs-lookup"><span data-stu-id="c4ab4-107">Call setup failure</span></span>
- <span data-ttu-id="c4ab4-108">Queda de chamada intermediário</span><span class="sxs-lookup"><span data-stu-id="c4ab4-108">Mid-call drop</span></span>

<span data-ttu-id="c4ab4-109">Se um ou mais fluxos de mídia tiverem qualquer uma dessas falhas, essa falha será propagada no nível do segmento.</span><span class="sxs-lookup"><span data-stu-id="c4ab4-109">If one or more media streams have any of these failures, that failure is propagated at the segment level.</span></span> <span data-ttu-id="c4ab4-110">Se um ou mais segmentos tiverem qualquer uma dessas falhas, essa falha será propagada no nível da sessão.</span><span class="sxs-lookup"><span data-stu-id="c4ab4-110">If one or more segments have any of these failures, that failure is propagated at the session level.</span></span>

## <a name="properties"></a><span data-ttu-id="c4ab4-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c4ab4-111">Properties</span></span>

| <span data-ttu-id="c4ab4-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4ab4-112">Property</span></span>     | <span data-ttu-id="c4ab4-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4ab4-113">Type</span></span>        | <span data-ttu-id="c4ab4-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4ab4-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c4ab4-115">motivo</span><span class="sxs-lookup"><span data-stu-id="c4ab4-115">reason</span></span>|<span data-ttu-id="c4ab4-116">String</span><span class="sxs-lookup"><span data-stu-id="c4ab4-116">String</span></span>|<span data-ttu-id="c4ab4-117">Classificação de por que uma chamada ou parte de uma chamada falhou.</span><span class="sxs-lookup"><span data-stu-id="c4ab4-117">Classification of why a call or portion of a call failed.</span></span>|
|<span data-ttu-id="c4ab4-118">estágio</span><span class="sxs-lookup"><span data-stu-id="c4ab4-118">stage</span></span>|<span data-ttu-id="c4ab4-119">Microsoft. Graph. callRecords. failureStage</span><span class="sxs-lookup"><span data-stu-id="c4ab4-119">microsoft.graph.callRecords.failureStage</span></span>|<span data-ttu-id="c4ab4-120">O estágio quando a falha ocorreu.</span><span class="sxs-lookup"><span data-stu-id="c4ab4-120">The stage when the failure occurred.</span></span> <span data-ttu-id="c4ab4-121">Os valores possíveis são: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c4ab4-121">Possible values are: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4ab4-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c4ab4-122">JSON representation</span></span>

<span data-ttu-id="c4ab4-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c4ab4-123">The following is a JSON representation of the resource.</span></span>

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


