---
title: tipo de recurso statusDetails
description: Descreve o status do evento de provisionamento e os erros associados.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 853f7ba95ca4e569efd57bb46024b4258b098d90
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520314"
---
# <a name="statusdetails-resource-type"></a><span data-ttu-id="ee624-103">tipo de recurso statusDetails</span><span class="sxs-lookup"><span data-stu-id="ee624-103">statusDetails resource type</span></span>

<span data-ttu-id="ee624-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ee624-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee624-105">Descreve o status do evento de provisionamento e os erros associados.</span><span class="sxs-lookup"><span data-stu-id="ee624-105">Describes the status of the provisioning event and the associated errors.</span></span> <span data-ttu-id="ee624-106">Ela é herdada de [statusBase](/graph/api/resources/statusbase?view=graph-rest-beta) e usada apenas quando status é definido como ' Failure '.</span><span class="sxs-lookup"><span data-stu-id="ee624-106">It is inherited from [statusBase](/graph/api/resources/statusbase?view=graph-rest-beta) and only used when status is set to 'failure'.</span></span>  

## <a name="properties"></a><span data-ttu-id="ee624-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee624-107">Properties</span></span>

| <span data-ttu-id="ee624-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee624-108">Property</span></span>     | <span data-ttu-id="ee624-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee624-109">Type</span></span>        | <span data-ttu-id="ee624-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee624-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ee624-111">status</span><span class="sxs-lookup"><span data-stu-id="ee624-111">status</span></span>|<span data-ttu-id="ee624-112">String</span><span class="sxs-lookup"><span data-stu-id="ee624-112">String</span></span>|<span data-ttu-id="ee624-113">Os valores possíveis são: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ee624-113">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span> <span data-ttu-id="ee624-114">Herdado de statusBase.</span><span class="sxs-lookup"><span data-stu-id="ee624-114">Inherited from statusBase.</span></span>|
|<span data-ttu-id="ee624-115">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="ee624-115">additionalDetails</span></span>|<span data-ttu-id="ee624-116">String</span><span class="sxs-lookup"><span data-stu-id="ee624-116">String</span></span>|<span data-ttu-id="ee624-117">Detalhes adicionais em caso de erro.</span><span class="sxs-lookup"><span data-stu-id="ee624-117">Additional details in case of error.</span></span>|
|<span data-ttu-id="ee624-118">errorCategory</span><span class="sxs-lookup"><span data-stu-id="ee624-118">errorCategory</span></span>|<span data-ttu-id="ee624-119">String</span><span class="sxs-lookup"><span data-stu-id="ee624-119">String</span></span>|<span data-ttu-id="ee624-120">Categoriza o código de erro.</span><span class="sxs-lookup"><span data-stu-id="ee624-120">Categorizes the error code.</span></span>|
|<span data-ttu-id="ee624-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="ee624-121">errorCode</span></span>|<span data-ttu-id="ee624-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee624-122">String</span></span>|<span data-ttu-id="ee624-123">Código de erro exclusivo, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="ee624-123">Unique error code if any occurred.</span></span>|
|<span data-ttu-id="ee624-124">motivo</span><span class="sxs-lookup"><span data-stu-id="ee624-124">reason</span></span>|<span data-ttu-id="ee624-125">String</span><span class="sxs-lookup"><span data-stu-id="ee624-125">String</span></span>|<span data-ttu-id="ee624-126">Resume o status e descreve por que o status ocorreu.</span><span class="sxs-lookup"><span data-stu-id="ee624-126">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="ee624-127">recomendado</span><span class="sxs-lookup"><span data-stu-id="ee624-127">recommendedAction</span></span>|<span data-ttu-id="ee624-128">String</span><span class="sxs-lookup"><span data-stu-id="ee624-128">String</span></span>|<span data-ttu-id="ee624-129">Fornece a resolução para o erro correspondente.</span><span class="sxs-lookup"><span data-stu-id="ee624-129">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee624-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee624-130">JSON representation</span></span>

<span data-ttu-id="ee624-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee624-131">The following is a JSON representation of the resource.</span></span>

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
