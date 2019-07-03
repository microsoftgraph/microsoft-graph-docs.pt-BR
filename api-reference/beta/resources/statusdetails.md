---
title: tipo de recurso statusDetails
description: Descreve o status do evento de provisionamento e os erros associados.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 88880fbe88c0bd702eefeac5bed9668aac12a356
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455179"
---
# <a name="statusdetails-resource-type"></a><span data-ttu-id="37029-103">tipo de recurso statusDetails</span><span class="sxs-lookup"><span data-stu-id="37029-103">statusDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37029-104">Descreve o status do evento de provisionamento e os erros associados.</span><span class="sxs-lookup"><span data-stu-id="37029-104">Describes the status of the provisioning event and the associated errors.</span></span> <span data-ttu-id="37029-105">Ela é herdada de [statusBase](/graph/api/resources/statusbase?view=graph-rest-beta) e usada apenas quando status é definido como ' Failure '.</span><span class="sxs-lookup"><span data-stu-id="37029-105">It is inherited from [statusBase](/graph/api/resources/statusbase?view=graph-rest-beta) and only used when status is set to 'failure'.</span></span>  

## <a name="properties"></a><span data-ttu-id="37029-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37029-106">Properties</span></span>

| <span data-ttu-id="37029-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37029-107">Property</span></span>     | <span data-ttu-id="37029-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="37029-108">Type</span></span>        | <span data-ttu-id="37029-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="37029-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="37029-110">status</span><span class="sxs-lookup"><span data-stu-id="37029-110">status</span></span>|<span data-ttu-id="37029-111">String</span><span class="sxs-lookup"><span data-stu-id="37029-111">String</span></span>|<span data-ttu-id="37029-112">Os valores possíveis são: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="37029-112">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span> <span data-ttu-id="37029-113">Herdado de statusBase.</span><span class="sxs-lookup"><span data-stu-id="37029-113">Inherited from statusBase.</span></span>|
|<span data-ttu-id="37029-114">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="37029-114">additionalDetails</span></span>|<span data-ttu-id="37029-115">String</span><span class="sxs-lookup"><span data-stu-id="37029-115">String</span></span>|<span data-ttu-id="37029-116">Detalhes adicionais em caso de erro.</span><span class="sxs-lookup"><span data-stu-id="37029-116">Additional details in case of error.</span></span>|
|<span data-ttu-id="37029-117">errorCategory</span><span class="sxs-lookup"><span data-stu-id="37029-117">errorCategory</span></span>|<span data-ttu-id="37029-118">String</span><span class="sxs-lookup"><span data-stu-id="37029-118">String</span></span>|<span data-ttu-id="37029-119">Categoriza o código de erro.</span><span class="sxs-lookup"><span data-stu-id="37029-119">Categorizes the error code.</span></span>|
|<span data-ttu-id="37029-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="37029-120">errorCode</span></span>|<span data-ttu-id="37029-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37029-121">String</span></span>|<span data-ttu-id="37029-122">Código de erro exclusivo, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="37029-122">Unique error code if any occurred.</span></span>|
|<span data-ttu-id="37029-123">motivos</span><span class="sxs-lookup"><span data-stu-id="37029-123">reason</span></span>|<span data-ttu-id="37029-124">String</span><span class="sxs-lookup"><span data-stu-id="37029-124">String</span></span>|<span data-ttu-id="37029-125">Resume o status e descreve por que o status ocorreu.</span><span class="sxs-lookup"><span data-stu-id="37029-125">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="37029-126">recomendado</span><span class="sxs-lookup"><span data-stu-id="37029-126">recommendedAction</span></span>|<span data-ttu-id="37029-127">String</span><span class="sxs-lookup"><span data-stu-id="37029-127">String</span></span>|<span data-ttu-id="37029-128">Fornece a resolução para o erro correspondente.</span><span class="sxs-lookup"><span data-stu-id="37029-128">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37029-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37029-129">JSON representation</span></span>

<span data-ttu-id="37029-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37029-130">The following is a JSON representation of the resource.</span></span>

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
