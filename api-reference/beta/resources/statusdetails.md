---
title: Tipo de recurso statusDetails
description: Descreve o status do evento de provisionamento e os erros associados.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: e3333ac030ec08722ad6bcaa58a153fc961469cf
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546901"
---
# <a name="statusdetails-resource-type-deprecated"></a><span data-ttu-id="23dbd-103">Tipo de recurso statusDetails (preterido)</span><span class="sxs-lookup"><span data-stu-id="23dbd-103">statusDetails resource type (deprecated)</span></span>

<span data-ttu-id="23dbd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23dbd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
>[!CAUTION] 
> <span data-ttu-id="23dbd-105">A API statusDetails está preterida e interromperá o retorno de dados em 31 de dezembro de 2021.</span><span class="sxs-lookup"><span data-stu-id="23dbd-105">The statusDetails API is deprecated and will stop returning data om December 31, 2021.</span></span> <span data-ttu-id="23dbd-106">Use o novo tipo [provisioningStatusInfo.](provisioningstatusinfo.md)</span><span class="sxs-lookup"><span data-stu-id="23dbd-106">Please use the new [provisioningStatusInfo](provisioningstatusinfo.md) type.</span></span>

<span data-ttu-id="23dbd-107">Descreve o status do evento de provisionamento e os erros associados.</span><span class="sxs-lookup"><span data-stu-id="23dbd-107">Describes the status of the provisioning event and the associated errors.</span></span> <span data-ttu-id="23dbd-108">Ele é herdado do [statusBase](/graph/api/resources/statusbase) e usado somente quando o status é definido como `failure` .</span><span class="sxs-lookup"><span data-stu-id="23dbd-108">It is inherited from [statusBase](/graph/api/resources/statusbase) and only used when status is set to `failure`.</span></span>  

## <a name="properties"></a><span data-ttu-id="23dbd-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23dbd-109">Properties</span></span>

| <span data-ttu-id="23dbd-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23dbd-110">Property</span></span>     | <span data-ttu-id="23dbd-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="23dbd-111">Type</span></span>        | <span data-ttu-id="23dbd-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="23dbd-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="23dbd-113">status</span><span class="sxs-lookup"><span data-stu-id="23dbd-113">status</span></span>|<span data-ttu-id="23dbd-114">statusBase</span><span class="sxs-lookup"><span data-stu-id="23dbd-114">statusBase</span></span>|<span data-ttu-id="23dbd-115">Os valores possíveis são: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="23dbd-115">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span> <span data-ttu-id="23dbd-116">Herdado do statusBase.</span><span class="sxs-lookup"><span data-stu-id="23dbd-116">Inherited from statusBase.</span></span>|
|<span data-ttu-id="23dbd-117">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="23dbd-117">additionalDetails</span></span>|<span data-ttu-id="23dbd-118">String</span><span class="sxs-lookup"><span data-stu-id="23dbd-118">String</span></span>|<span data-ttu-id="23dbd-119">Detalhes adicionais em caso de erro.</span><span class="sxs-lookup"><span data-stu-id="23dbd-119">Additional details in case of error.</span></span>|
|<span data-ttu-id="23dbd-120">errorCategory</span><span class="sxs-lookup"><span data-stu-id="23dbd-120">errorCategory</span></span>|<span data-ttu-id="23dbd-121">String</span><span class="sxs-lookup"><span data-stu-id="23dbd-121">String</span></span>|<span data-ttu-id="23dbd-122">Categoriza o código de erro.</span><span class="sxs-lookup"><span data-stu-id="23dbd-122">Categorizes the error code.</span></span> <span data-ttu-id="23dbd-123">Os valores possíveis são `Failure`, `NonServiceFailure`, `Success`.</span><span class="sxs-lookup"><span data-stu-id="23dbd-123">Possible values are `Failure`, `NonServiceFailure`, `Success`.</span></span>|
|<span data-ttu-id="23dbd-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="23dbd-124">errorCode</span></span>|<span data-ttu-id="23dbd-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23dbd-125">String</span></span>|<span data-ttu-id="23dbd-126">Código de erro exclusivo se ocorrer algum.</span><span class="sxs-lookup"><span data-stu-id="23dbd-126">Unique error code if any occurred.</span></span> [<span data-ttu-id="23dbd-127">Saiba mais</span><span class="sxs-lookup"><span data-stu-id="23dbd-127">Learn more</span></span>](/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|<span data-ttu-id="23dbd-128">motivo</span><span class="sxs-lookup"><span data-stu-id="23dbd-128">reason</span></span>|<span data-ttu-id="23dbd-129">String</span><span class="sxs-lookup"><span data-stu-id="23dbd-129">String</span></span>|<span data-ttu-id="23dbd-130">Resume o status e descreve por que o status aconteceu.</span><span class="sxs-lookup"><span data-stu-id="23dbd-130">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="23dbd-131">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="23dbd-131">recommendedAction</span></span>|<span data-ttu-id="23dbd-132">String</span><span class="sxs-lookup"><span data-stu-id="23dbd-132">String</span></span>|<span data-ttu-id="23dbd-133">Fornece a resolução do erro correspondente.</span><span class="sxs-lookup"><span data-stu-id="23dbd-133">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="23dbd-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23dbd-134">JSON representation</span></span>

<span data-ttu-id="23dbd-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23dbd-135">The following is a JSON representation of the resource.</span></span>

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


