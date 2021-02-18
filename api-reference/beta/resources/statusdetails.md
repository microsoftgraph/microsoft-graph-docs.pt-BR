---
title: Tipo de recurso statusDetails
description: Descreve o status do evento de provisionamento e os erros associados.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 81ea4a75970e37a360c402aced66f01ccb9e7c47
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292606"
---
# <a name="statusdetails-resource-type"></a><span data-ttu-id="0f7bc-103">Tipo de recurso statusDetails</span><span class="sxs-lookup"><span data-stu-id="0f7bc-103">statusDetails resource type</span></span>

<span data-ttu-id="0f7bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f7bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f7bc-105">Descreve o status do evento de provisionamento e os erros associados.</span><span class="sxs-lookup"><span data-stu-id="0f7bc-105">Describes the status of the provisioning event and the associated errors.</span></span> <span data-ttu-id="0f7bc-106">Ele é herdado de [statusBase](/graph/api/resources/statusbase) e usado somente quando o status é definido como `failure` .</span><span class="sxs-lookup"><span data-stu-id="0f7bc-106">It is inherited from [statusBase](/graph/api/resources/statusbase) and only used when status is set to `failure`.</span></span>  

## <a name="properties"></a><span data-ttu-id="0f7bc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f7bc-107">Properties</span></span>

| <span data-ttu-id="0f7bc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f7bc-108">Property</span></span>     | <span data-ttu-id="0f7bc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f7bc-109">Type</span></span>        | <span data-ttu-id="0f7bc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f7bc-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0f7bc-111">status</span><span class="sxs-lookup"><span data-stu-id="0f7bc-111">status</span></span>|<span data-ttu-id="0f7bc-112">String</span><span class="sxs-lookup"><span data-stu-id="0f7bc-112">String</span></span>|<span data-ttu-id="0f7bc-113">Os valores possíveis são: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0f7bc-113">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span> <span data-ttu-id="0f7bc-114">Herdado do statusBase.</span><span class="sxs-lookup"><span data-stu-id="0f7bc-114">Inherited from statusBase.</span></span>|
|<span data-ttu-id="0f7bc-115">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="0f7bc-115">additionalDetails</span></span>|<span data-ttu-id="0f7bc-116">String</span><span class="sxs-lookup"><span data-stu-id="0f7bc-116">String</span></span>|<span data-ttu-id="0f7bc-117">Detalhes adicionais em caso de erro.</span><span class="sxs-lookup"><span data-stu-id="0f7bc-117">Additional details in case of error.</span></span>|
|<span data-ttu-id="0f7bc-118">errorCategory</span><span class="sxs-lookup"><span data-stu-id="0f7bc-118">errorCategory</span></span>|<span data-ttu-id="0f7bc-119">String</span><span class="sxs-lookup"><span data-stu-id="0f7bc-119">String</span></span>|<span data-ttu-id="0f7bc-120">Categoriza o código de erro.</span><span class="sxs-lookup"><span data-stu-id="0f7bc-120">Categorizes the error code.</span></span> <span data-ttu-id="0f7bc-121">Os valores possíveis são `Failure`, `NonServiceFailure`, `Success`.</span><span class="sxs-lookup"><span data-stu-id="0f7bc-121">Possible values are `Failure`, `NonServiceFailure`, `Success`.</span></span>|
|<span data-ttu-id="0f7bc-122">errorCode</span><span class="sxs-lookup"><span data-stu-id="0f7bc-122">errorCode</span></span>|<span data-ttu-id="0f7bc-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f7bc-123">String</span></span>|<span data-ttu-id="0f7bc-124">Código de erro exclusivo se ocorreu.</span><span class="sxs-lookup"><span data-stu-id="0f7bc-124">Unique error code if any occurred.</span></span> [<span data-ttu-id="0f7bc-125">Saiba Mais</span><span class="sxs-lookup"><span data-stu-id="0f7bc-125">Learn more</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|<span data-ttu-id="0f7bc-126">motivo</span><span class="sxs-lookup"><span data-stu-id="0f7bc-126">reason</span></span>|<span data-ttu-id="0f7bc-127">String</span><span class="sxs-lookup"><span data-stu-id="0f7bc-127">String</span></span>|<span data-ttu-id="0f7bc-128">Resume o status e descreve por que o status aconteceu.</span><span class="sxs-lookup"><span data-stu-id="0f7bc-128">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="0f7bc-129">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="0f7bc-129">recommendedAction</span></span>|<span data-ttu-id="0f7bc-130">String</span><span class="sxs-lookup"><span data-stu-id="0f7bc-130">String</span></span>|<span data-ttu-id="0f7bc-131">Fornece a resolução do erro correspondente.</span><span class="sxs-lookup"><span data-stu-id="0f7bc-131">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f7bc-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f7bc-132">JSON representation</span></span>

<span data-ttu-id="0f7bc-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f7bc-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.statusDetails",
  "baseType": "microsoft.graph.statusBase"
}-->

```json
{
  "status": "failure",
  "additionalDetails": "String",
  "errorCategory": "String",
  "errorCode": "String",
  "reason": "String",
  "recommendedAction": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "statusDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


