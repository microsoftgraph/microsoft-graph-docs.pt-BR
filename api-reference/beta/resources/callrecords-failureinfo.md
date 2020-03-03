---
title: tipo de recurso failureInfo
description: O tipo failureInfo
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3160fe3b2d0c1fd59ddd86621667b67ee5759dd5
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394672"
---
# <a name="failureinfo-resource-type"></a><span data-ttu-id="c6c44-103">tipo de recurso failureInfo</span><span class="sxs-lookup"><span data-stu-id="c6c44-103">failureInfo resource type</span></span>

<span data-ttu-id="c6c44-104">Namespace: Microsoft. Graph. callRecords</span><span class="sxs-lookup"><span data-stu-id="c6c44-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6c44-105">Representa informações sobre o motivo pelo qual uma chamada ou parte de uma chamada falhou.</span><span class="sxs-lookup"><span data-stu-id="c6c44-105">Represents information about why a call or portion of a call failed.</span></span>

## <a name="properties"></a><span data-ttu-id="c6c44-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6c44-106">Properties</span></span>

| <span data-ttu-id="c6c44-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6c44-107">Property</span></span>     | <span data-ttu-id="c6c44-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6c44-108">Type</span></span>        | <span data-ttu-id="c6c44-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6c44-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c6c44-110">motivo</span><span class="sxs-lookup"><span data-stu-id="c6c44-110">reason</span></span>|<span data-ttu-id="c6c44-111">String</span><span class="sxs-lookup"><span data-stu-id="c6c44-111">String</span></span>|<span data-ttu-id="c6c44-112">Classificação de por que uma chamada ou parte de uma chamada falhou.</span><span class="sxs-lookup"><span data-stu-id="c6c44-112">Classification of why a call or portion of a call failed.</span></span>|
|<span data-ttu-id="c6c44-113">estágio</span><span class="sxs-lookup"><span data-stu-id="c6c44-113">stage</span></span>|<span data-ttu-id="c6c44-114">String</span><span class="sxs-lookup"><span data-stu-id="c6c44-114">String</span></span>|<span data-ttu-id="c6c44-115">O estágio quando a falha ocorreu.</span><span class="sxs-lookup"><span data-stu-id="c6c44-115">The stage when the failure occurred.</span></span> <span data-ttu-id="c6c44-116">Os valores possíveis são: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c6c44-116">Possible values are: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6c44-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6c44-117">JSON representation</span></span>

<span data-ttu-id="c6c44-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c6c44-118">The following is a JSON representation of the resource.</span></span>

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