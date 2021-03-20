---
title: Tipo de recurso classificationResult
description: Representa o resultado de uma solicitação de classificação.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5ecc16197ef4671c6e83883bc69aed45b3ffa200
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941817"
---
# <a name="classificationresult-resource-type"></a><span data-ttu-id="631ff-103">Tipo de recurso classificationResult</span><span class="sxs-lookup"><span data-stu-id="631ff-103">classificationResult resource type</span></span>

<span data-ttu-id="631ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="631ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="631ff-105">Representa o resultado de uma operação de classificação do Mecanismo de Classificação da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="631ff-105">Represents the result of a classification operation from the Microsoft Classification Engine.</span></span> <span data-ttu-id="631ff-106">Os resultados da classificação de dados da Proteção de Informações do Azure, do Office e de outros serviços da Microsoft podem retornar um conjunto bem [definido de tipos de classificação.](/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="631ff-106">Data classification results from Azure Information Protection, Office, and other Microsoft services may return a [well-defined set of classification types](/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span> <span data-ttu-id="631ff-107">Esses tipos podem ser fornecidos à API [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) para resolver uma informação confidenciais para um rótulo de Proteção de Informações da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="631ff-107">These types can be provided to the [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) API to resolve a sensitive information to a Microsoft Information Protection label.</span></span> 

## <a name="properties"></a><span data-ttu-id="631ff-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="631ff-108">Properties</span></span>

| <span data-ttu-id="631ff-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="631ff-109">Property</span></span>        | <span data-ttu-id="631ff-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="631ff-110">Type</span></span>  | <span data-ttu-id="631ff-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="631ff-111">Description</span></span>                                                            |
| :-------------- | :---- | :--------------------------------------------------------------------- |
| <span data-ttu-id="631ff-112">confidenceLevel</span><span class="sxs-lookup"><span data-stu-id="631ff-112">confidenceLevel</span></span> | <span data-ttu-id="631ff-113">Int32</span><span class="sxs-lookup"><span data-stu-id="631ff-113">Int32</span></span> | <span data-ttu-id="631ff-114">O nível de confiança, de 0 a 100, do resultado.</span><span class="sxs-lookup"><span data-stu-id="631ff-114">The confidence level, 0 to 100, of the result.</span></span>                         |
| <span data-ttu-id="631ff-115">Count</span><span class="sxs-lookup"><span data-stu-id="631ff-115">count</span></span>           | <span data-ttu-id="631ff-116">Int32</span><span class="sxs-lookup"><span data-stu-id="631ff-116">Int32</span></span> | <span data-ttu-id="631ff-117">O número de instâncias do tipo de informação específico na entrada.</span><span class="sxs-lookup"><span data-stu-id="631ff-117">The number of instances of the specific information type in the input.</span></span> |
| <span data-ttu-id="631ff-118">sensitiveTypeId</span><span class="sxs-lookup"><span data-stu-id="631ff-118">sensitiveTypeId</span></span> | <span data-ttu-id="631ff-119">GUID</span><span class="sxs-lookup"><span data-stu-id="631ff-119">GUID</span></span>  | <span data-ttu-id="631ff-120">O GUID do tipo de informação confidenciais descoberto.</span><span class="sxs-lookup"><span data-stu-id="631ff-120">The GUID of the discovered sensitive information type.</span></span>                 |

## <a name="json-representation"></a><span data-ttu-id="631ff-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="631ff-121">JSON representation</span></span>

<span data-ttu-id="631ff-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="631ff-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.classificationResult",
  "baseType": null
}-->

```json
{
  "confidenceLevel": 1024,
  "count": 1024,
  "sensitiveTypeId": "Guid"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "classificationResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->