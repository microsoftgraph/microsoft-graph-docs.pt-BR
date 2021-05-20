---
title: provisionamentoErrorInfo tipo de recurso
description: Descreve o status do evento de provisionamento e os erros associados.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a682e176b40d58e2dc0a794b58b8561f8948d5a5
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547152"
---
# <a name="provisioningerrorinfo-resource-type"></a><span data-ttu-id="7c40f-103">provisionamentoErrorInfo tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="7c40f-103">provisioningErrorInfo resource type</span></span>

<span data-ttu-id="7c40f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c40f-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="7c40f-105">Descreve o status do evento de provisionamento e os erros associados.</span><span class="sxs-lookup"><span data-stu-id="7c40f-105">Describes the status of the provisioning event and the associated errors.</span></span> 

## <a name="properties"></a><span data-ttu-id="7c40f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c40f-106">Properties</span></span>

| <span data-ttu-id="7c40f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c40f-107">Property</span></span>     | <span data-ttu-id="7c40f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c40f-108">Type</span></span>        | <span data-ttu-id="7c40f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c40f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7c40f-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="7c40f-110">additionalDetails</span></span>|<span data-ttu-id="7c40f-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c40f-111">String</span></span>|<span data-ttu-id="7c40f-112">Detalhes adicionais em caso de erro.</span><span class="sxs-lookup"><span data-stu-id="7c40f-112">Additional details in case of error.</span></span>|
|<span data-ttu-id="7c40f-113">erroCategoria</span><span class="sxs-lookup"><span data-stu-id="7c40f-113">errorCategory</span></span>|<span data-ttu-id="7c40f-114">provisionamentoStatusErrorCategory</span><span class="sxs-lookup"><span data-stu-id="7c40f-114">provisioningStatusErrorCategory</span></span>|<span data-ttu-id="7c40f-115">Categoriza o código de erro.</span><span class="sxs-lookup"><span data-stu-id="7c40f-115">Categorizes the error code.</span></span> <span data-ttu-id="7c40f-116">Os valores possíveis `failure` `nonServiceFailure` são, `success` , , `unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="7c40f-116">Possible values are `failure`, `nonServiceFailure`, `success`, `unknownFutureValue`</span></span>|
|<span data-ttu-id="7c40f-117">errorCode</span><span class="sxs-lookup"><span data-stu-id="7c40f-117">errorCode</span></span>|<span data-ttu-id="7c40f-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c40f-118">String</span></span>|<span data-ttu-id="7c40f-119">Código de erro único, se ocorreu algum.</span><span class="sxs-lookup"><span data-stu-id="7c40f-119">Unique error code if any occurred.</span></span> [<span data-ttu-id="7c40f-120">Saiba mais</span><span class="sxs-lookup"><span data-stu-id="7c40f-120">Learn more</span></span>](/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|<span data-ttu-id="7c40f-121">motivo</span><span class="sxs-lookup"><span data-stu-id="7c40f-121">reason</span></span>|<span data-ttu-id="7c40f-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c40f-122">String</span></span>|<span data-ttu-id="7c40f-123">Resume o status e descreve por que o status aconteceu.</span><span class="sxs-lookup"><span data-stu-id="7c40f-123">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="7c40f-124">recomendaçãoAction</span><span class="sxs-lookup"><span data-stu-id="7c40f-124">recommendedAction</span></span>|<span data-ttu-id="7c40f-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c40f-125">String</span></span>|<span data-ttu-id="7c40f-126">Fornece a resolução para o erro correspondente.</span><span class="sxs-lookup"><span data-stu-id="7c40f-126">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7c40f-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7c40f-127">JSON representation</span></span>

<span data-ttu-id="7c40f-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7c40f-128">The following is a JSON representation of the resource.</span></span>

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


