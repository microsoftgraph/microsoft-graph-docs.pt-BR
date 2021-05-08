---
title: Tipo de recurso provisioningErrorInfo
description: Descreve o status do evento de provisionamento e os erros associados.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d22d68b7c040ea07e6aef2cc0f606bd378b3b47c
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241482"
---
# <a name="provisioningerrorinfo-resource-type"></a><span data-ttu-id="36083-103">Tipo de recurso provisioningErrorInfo</span><span class="sxs-lookup"><span data-stu-id="36083-103">provisioningErrorInfo resource type</span></span>

<span data-ttu-id="36083-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36083-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="36083-105">Descreve o status do evento de provisionamento e os erros associados.</span><span class="sxs-lookup"><span data-stu-id="36083-105">Describes the status of the provisioning event and the associated errors.</span></span> 

## <a name="properties"></a><span data-ttu-id="36083-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36083-106">Properties</span></span>

| <span data-ttu-id="36083-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36083-107">Property</span></span>     | <span data-ttu-id="36083-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="36083-108">Type</span></span>        | <span data-ttu-id="36083-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="36083-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="36083-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="36083-110">additionalDetails</span></span>|<span data-ttu-id="36083-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36083-111">String</span></span>|<span data-ttu-id="36083-112">Detalhes adicionais em caso de erro.</span><span class="sxs-lookup"><span data-stu-id="36083-112">Additional details in case of error.</span></span>|
|<span data-ttu-id="36083-113">errorCategory</span><span class="sxs-lookup"><span data-stu-id="36083-113">errorCategory</span></span>|<span data-ttu-id="36083-114">provisioningStatusErrorCategory</span><span class="sxs-lookup"><span data-stu-id="36083-114">provisioningStatusErrorCategory</span></span>|<span data-ttu-id="36083-115">Categoriza o código de erro.</span><span class="sxs-lookup"><span data-stu-id="36083-115">Categorizes the error code.</span></span> <span data-ttu-id="36083-116">Os valores possíveis `failure` são `nonServiceFailure` , , `success` , `unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="36083-116">Possible values are `failure`, `nonServiceFailure`, `success`, `unknownFutureValue`</span></span>|
|<span data-ttu-id="36083-117">errorCode</span><span class="sxs-lookup"><span data-stu-id="36083-117">errorCode</span></span>|<span data-ttu-id="36083-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36083-118">String</span></span>|<span data-ttu-id="36083-119">Código de erro exclusivo se ocorrer algum.</span><span class="sxs-lookup"><span data-stu-id="36083-119">Unique error code if any occurred.</span></span> [<span data-ttu-id="36083-120">Saiba Mais</span><span class="sxs-lookup"><span data-stu-id="36083-120">Learn more</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|<span data-ttu-id="36083-121">motivo</span><span class="sxs-lookup"><span data-stu-id="36083-121">reason</span></span>|<span data-ttu-id="36083-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36083-122">String</span></span>|<span data-ttu-id="36083-123">Resume o status e descreve por que o status aconteceu.</span><span class="sxs-lookup"><span data-stu-id="36083-123">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="36083-124">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="36083-124">recommendedAction</span></span>|<span data-ttu-id="36083-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36083-125">String</span></span>|<span data-ttu-id="36083-126">Fornece a resolução do erro correspondente.</span><span class="sxs-lookup"><span data-stu-id="36083-126">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36083-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36083-127">JSON representation</span></span>

<span data-ttu-id="36083-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36083-128">The following is a JSON representation of the resource.</span></span>

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


