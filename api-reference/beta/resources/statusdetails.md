---
title: Tipo de recurso statusDetails
description: Descreve o status do evento de provisionamento e os erros associados.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d817c0aa46dde6b49debd849d8fd2ae61e06a672
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956814"
---
# <a name="statusdetails-resource-type"></a><span data-ttu-id="f4a0e-103">Tipo de recurso statusDetails</span><span class="sxs-lookup"><span data-stu-id="f4a0e-103">statusDetails resource type</span></span>

<span data-ttu-id="f4a0e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4a0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4a0e-105">Descreve o status do evento de provisionamento e os erros associados.</span><span class="sxs-lookup"><span data-stu-id="f4a0e-105">Describes the status of the provisioning event and the associated errors.</span></span> <span data-ttu-id="f4a0e-106">Ele é herdado do [statusBase](/graph/api/resources/statusbase) e usado somente quando o status é definido como `failure` .</span><span class="sxs-lookup"><span data-stu-id="f4a0e-106">It is inherited from [statusBase](/graph/api/resources/statusbase) and only used when status is set to `failure`.</span></span>  

## <a name="properties"></a><span data-ttu-id="f4a0e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4a0e-107">Properties</span></span>

| <span data-ttu-id="f4a0e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4a0e-108">Property</span></span>     | <span data-ttu-id="f4a0e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4a0e-109">Type</span></span>        | <span data-ttu-id="f4a0e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4a0e-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f4a0e-111">status</span><span class="sxs-lookup"><span data-stu-id="f4a0e-111">status</span></span>|<span data-ttu-id="f4a0e-112">statusBase</span><span class="sxs-lookup"><span data-stu-id="f4a0e-112">statusBase</span></span>|<span data-ttu-id="f4a0e-113">Os valores possíveis são: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f4a0e-113">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span> <span data-ttu-id="f4a0e-114">Herdado do statusBase.</span><span class="sxs-lookup"><span data-stu-id="f4a0e-114">Inherited from statusBase.</span></span>|
|<span data-ttu-id="f4a0e-115">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="f4a0e-115">additionalDetails</span></span>|<span data-ttu-id="f4a0e-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4a0e-116">String</span></span>|<span data-ttu-id="f4a0e-117">Detalhes adicionais em caso de erro.</span><span class="sxs-lookup"><span data-stu-id="f4a0e-117">Additional details in case of error.</span></span>|
|<span data-ttu-id="f4a0e-118">errorCategory</span><span class="sxs-lookup"><span data-stu-id="f4a0e-118">errorCategory</span></span>|<span data-ttu-id="f4a0e-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4a0e-119">String</span></span>|<span data-ttu-id="f4a0e-120">Categoriza o código de erro.</span><span class="sxs-lookup"><span data-stu-id="f4a0e-120">Categorizes the error code.</span></span> <span data-ttu-id="f4a0e-121">Os valores possíveis são `Failure`, `NonServiceFailure`, `Success`.</span><span class="sxs-lookup"><span data-stu-id="f4a0e-121">Possible values are `Failure`, `NonServiceFailure`, `Success`.</span></span>|
|<span data-ttu-id="f4a0e-122">errorCode</span><span class="sxs-lookup"><span data-stu-id="f4a0e-122">errorCode</span></span>|<span data-ttu-id="f4a0e-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4a0e-123">String</span></span>|<span data-ttu-id="f4a0e-124">Código de erro exclusivo se ocorrer algum.</span><span class="sxs-lookup"><span data-stu-id="f4a0e-124">Unique error code if any occurred.</span></span> [<span data-ttu-id="f4a0e-125">Saiba Mais</span><span class="sxs-lookup"><span data-stu-id="f4a0e-125">Learn more</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|<span data-ttu-id="f4a0e-126">motivo</span><span class="sxs-lookup"><span data-stu-id="f4a0e-126">reason</span></span>|<span data-ttu-id="f4a0e-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4a0e-127">String</span></span>|<span data-ttu-id="f4a0e-128">Resume o status e descreve por que o status aconteceu.</span><span class="sxs-lookup"><span data-stu-id="f4a0e-128">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="f4a0e-129">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="f4a0e-129">recommendedAction</span></span>|<span data-ttu-id="f4a0e-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4a0e-130">String</span></span>|<span data-ttu-id="f4a0e-131">Fornece a resolução do erro correspondente.</span><span class="sxs-lookup"><span data-stu-id="f4a0e-131">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4a0e-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4a0e-132">JSON representation</span></span>

<span data-ttu-id="f4a0e-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4a0e-133">The following is a JSON representation of the resource.</span></span>

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


