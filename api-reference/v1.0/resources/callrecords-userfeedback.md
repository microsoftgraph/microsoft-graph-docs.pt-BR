---
title: tipo de recurso userfeedback
description: O tipo userfeedback.
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 468f6a58d3e70a37b15c1b18663958ea5193d59a
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491938"
---
# <a name="userfeedback-resource-type"></a><span data-ttu-id="554dd-103">tipo de recurso userfeedback</span><span class="sxs-lookup"><span data-stu-id="554dd-103">userFeedback resource type</span></span>

<span data-ttu-id="554dd-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="554dd-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="554dd-105">Representa os comentários fornecidos pelo usuário para um ponto de extremidade sobre a qualidade da sessão.</span><span class="sxs-lookup"><span data-stu-id="554dd-105">Represents the feedback provided by the user an endpoint about the quality of the session.</span></span>

## <a name="properties"></a><span data-ttu-id="554dd-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="554dd-106">Properties</span></span>

| <span data-ttu-id="554dd-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="554dd-107">Property</span></span>     | <span data-ttu-id="554dd-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="554dd-108">Type</span></span>        | <span data-ttu-id="554dd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="554dd-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="554dd-110">classificação</span><span class="sxs-lookup"><span data-stu-id="554dd-110">rating</span></span>|<span data-ttu-id="554dd-111">Microsoft. Graph. callRecords. userFeedbackRating</span><span class="sxs-lookup"><span data-stu-id="554dd-111">microsoft.graph.callRecords.userFeedbackRating</span></span>|<span data-ttu-id="554dd-112">A classificação fornecida pelo usuário deste ponto de extremidade sobre a qualidade desta sessão.</span><span class="sxs-lookup"><span data-stu-id="554dd-112">The rating provided by the user of this endpoint about the quality of this Session.</span></span> <span data-ttu-id="554dd-113">Os valores possíveis são: `notRated`, `bad`, `poor`, `fair`, `good`, `excellent`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="554dd-113">Possible values are: `notRated`, `bad`, `poor`, `fair`, `good`, `excellent`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="554dd-114">texto</span><span class="sxs-lookup"><span data-stu-id="554dd-114">text</span></span>|<span data-ttu-id="554dd-115">String</span><span class="sxs-lookup"><span data-stu-id="554dd-115">String</span></span>|<span data-ttu-id="554dd-116">O texto de comentários fornecido pelo usuário deste ponto de extremidade para a sessão.</span><span class="sxs-lookup"><span data-stu-id="554dd-116">The feedback text provided by the user of this endpoint for the session.</span></span>|
|<span data-ttu-id="554dd-117">sinais</span><span class="sxs-lookup"><span data-stu-id="554dd-117">tokens</span></span>|[<span data-ttu-id="554dd-118">Microsoft. Graph. callRecords. feedbackTokenSet</span><span class="sxs-lookup"><span data-stu-id="554dd-118">microsoft.graph.callRecords.feedbackTokenSet</span></span>](callrecords-feedbacktokenset.md)|<span data-ttu-id="554dd-119">O conjunto de tokens de comentários fornecidos pelo usuário deste ponto de extremidade para a sessão.</span><span class="sxs-lookup"><span data-stu-id="554dd-119">The set of feedback tokens provided by the user of this endpoint for the session.</span></span> <span data-ttu-id="554dd-120">Este é um conjunto de propriedades booleanas.</span><span class="sxs-lookup"><span data-stu-id="554dd-120">This is a set of Boolean properties.</span></span> <span data-ttu-id="554dd-121">Os nomes de propriedade não devem ser dependentes, já que eles podem ser alterados, dependendo de quais tokens são oferecidos para o usuário.</span><span class="sxs-lookup"><span data-stu-id="554dd-121">The property names should not be relied upon since they may change depending on what tokens are offered to the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="554dd-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="554dd-122">JSON representation</span></span>

<span data-ttu-id="554dd-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="554dd-123">The following is a JSON representation of the resource.</span></span>

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