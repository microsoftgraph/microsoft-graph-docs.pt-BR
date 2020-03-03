---
title: tipo de recurso userfeedback
description: O tipo userfeedback.
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0ab9c49563bb4715b1736618a939b681178ddae8
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394654"
---
# <a name="userfeedback-resource-type"></a><span data-ttu-id="12839-103">tipo de recurso userfeedback</span><span class="sxs-lookup"><span data-stu-id="12839-103">userFeedback resource type</span></span>

<span data-ttu-id="12839-104">Namespace: Microsoft. Graph. callRecords</span><span class="sxs-lookup"><span data-stu-id="12839-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12839-105">Representa os comentários fornecidos pelo usuário para um ponto de extremidade sobre a qualidade da sessão.</span><span class="sxs-lookup"><span data-stu-id="12839-105">Represents the feedback provided by the user an endpoint about the quality of the session.</span></span>

## <a name="properties"></a><span data-ttu-id="12839-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12839-106">Properties</span></span>

| <span data-ttu-id="12839-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12839-107">Property</span></span>     | <span data-ttu-id="12839-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="12839-108">Type</span></span>        | <span data-ttu-id="12839-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="12839-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="12839-110">classificação</span><span class="sxs-lookup"><span data-stu-id="12839-110">rating</span></span>|<span data-ttu-id="12839-111">String</span><span class="sxs-lookup"><span data-stu-id="12839-111">String</span></span>|<span data-ttu-id="12839-112">A classificação fornecida pelo usuário deste ponto de extremidade sobre a qualidade desta sessão.</span><span class="sxs-lookup"><span data-stu-id="12839-112">The rating provided by the user of this endpoint about the quality of this Session.</span></span> <span data-ttu-id="12839-113">Os valores possíveis são: `notRated`, `bad`, `poor`, `fair`, `good`, `excellent`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="12839-113">Possible values are: `notRated`, `bad`, `poor`, `fair`, `good`, `excellent`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="12839-114">texto</span><span class="sxs-lookup"><span data-stu-id="12839-114">text</span></span>|<span data-ttu-id="12839-115">String</span><span class="sxs-lookup"><span data-stu-id="12839-115">String</span></span>|<span data-ttu-id="12839-116">O texto de comentários fornecido pelo usuário deste ponto de extremidade para a sessão.</span><span class="sxs-lookup"><span data-stu-id="12839-116">The feedback text provided by the user of this endpoint for the session.</span></span>|
|<span data-ttu-id="12839-117">sinais</span><span class="sxs-lookup"><span data-stu-id="12839-117">tokens</span></span>|[<span data-ttu-id="12839-118">Microsoft. Graph. callRecords. feedbackTokenSet</span><span class="sxs-lookup"><span data-stu-id="12839-118">microsoft.graph.callRecords.feedbackTokenSet</span></span>](callrecords-feedbacktokenset.md)|<span data-ttu-id="12839-119">O conjunto de tokens de comentários fornecidos pelo usuário deste ponto de extremidade para a sessão.</span><span class="sxs-lookup"><span data-stu-id="12839-119">The set of feedback tokens provided by the user of this endpoint for the session.</span></span> <span data-ttu-id="12839-120">Este é um conjunto de propriedades booleanas.</span><span class="sxs-lookup"><span data-stu-id="12839-120">This is a set of Boolean properties.</span></span> <span data-ttu-id="12839-121">Os nomes de propriedade não devem ser dependentes, já que eles podem ser alterados, dependendo de quais tokens são oferecidos para o usuário.</span><span class="sxs-lookup"><span data-stu-id="12839-121">The property names should not be relied upon since they may change depending on what tokens are offered to the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12839-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12839-122">JSON representation</span></span>

<span data-ttu-id="12839-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12839-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.userFeedback",
  "baseType": null
}-->

```json
{
  "rating": "String",
  "text": "String",
  "tokens": {"@odata.type": "microsoft.graph.callRecords.feedbackTokenSet"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->