---
title: Tipo de recurso provisioningErrorInfo
description: Descreve o status do evento de provisionamento e os erros associados.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: dddddfa793cf9aac7436fc85e0ce911df7b4ec3e
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546963"
---
# <a name="provisioningerrorinfo-resource-type"></a><span data-ttu-id="c65b5-103">Tipo de recurso provisioningErrorInfo</span><span class="sxs-lookup"><span data-stu-id="c65b5-103">provisioningErrorInfo resource type</span></span>

<span data-ttu-id="c65b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c65b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c65b5-105">Descreve o status do evento de provisionamento e os erros associados.</span><span class="sxs-lookup"><span data-stu-id="c65b5-105">Describes the status of the provisioning event and the associated errors.</span></span> 

## <a name="properties"></a><span data-ttu-id="c65b5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c65b5-106">Properties</span></span>

| <span data-ttu-id="c65b5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c65b5-107">Property</span></span>     | <span data-ttu-id="c65b5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c65b5-108">Type</span></span>        | <span data-ttu-id="c65b5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c65b5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c65b5-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="c65b5-110">additionalDetails</span></span>|<span data-ttu-id="c65b5-111">String</span><span class="sxs-lookup"><span data-stu-id="c65b5-111">String</span></span>|<span data-ttu-id="c65b5-112">Detalhes adicionais em caso de erro.</span><span class="sxs-lookup"><span data-stu-id="c65b5-112">Additional details in case of error.</span></span>|
|<span data-ttu-id="c65b5-113">errorCategory</span><span class="sxs-lookup"><span data-stu-id="c65b5-113">errorCategory</span></span>|<span data-ttu-id="c65b5-114">String</span><span class="sxs-lookup"><span data-stu-id="c65b5-114">String</span></span>|<span data-ttu-id="c65b5-115">Categoriza o código de erro.</span><span class="sxs-lookup"><span data-stu-id="c65b5-115">Categorizes the error code.</span></span> <span data-ttu-id="c65b5-116">Os valores possíveis `failure` são `nonServiceFailure` , , `success` , `unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="c65b5-116">Possible values are `failure`, `nonServiceFailure`, `success`, `unknownFutureValue`</span></span>|
|<span data-ttu-id="c65b5-117">errorCode</span><span class="sxs-lookup"><span data-stu-id="c65b5-117">errorCode</span></span>|<span data-ttu-id="c65b5-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c65b5-118">String</span></span>|<span data-ttu-id="c65b5-119">Código de erro exclusivo se ocorrer algum.</span><span class="sxs-lookup"><span data-stu-id="c65b5-119">Unique error code if any occurred.</span></span> [<span data-ttu-id="c65b5-120">Saiba mais</span><span class="sxs-lookup"><span data-stu-id="c65b5-120">Learn more</span></span>](/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|<span data-ttu-id="c65b5-121">motivo</span><span class="sxs-lookup"><span data-stu-id="c65b5-121">reason</span></span>|<span data-ttu-id="c65b5-122">String</span><span class="sxs-lookup"><span data-stu-id="c65b5-122">String</span></span>|<span data-ttu-id="c65b5-123">Resume o status e descreve por que o status aconteceu.</span><span class="sxs-lookup"><span data-stu-id="c65b5-123">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="c65b5-124">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="c65b5-124">recommendedAction</span></span>|<span data-ttu-id="c65b5-125">String</span><span class="sxs-lookup"><span data-stu-id="c65b5-125">String</span></span>|<span data-ttu-id="c65b5-126">Fornece a resolução do erro correspondente.</span><span class="sxs-lookup"><span data-stu-id="c65b5-126">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c65b5-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c65b5-127">JSON representation</span></span>

<span data-ttu-id="c65b5-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c65b5-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningErrorInfo",
  "baseType": null
}-->

```json
{
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
  "description": "provisioningErrorInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


