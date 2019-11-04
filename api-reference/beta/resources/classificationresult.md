---
title: tipo de recurso classificationResult
description: Representa o resultado de uma solicitação de classificação.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 51b03cf4a579ccab642fe9bdce2e71becebba4be
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938762"
---
# <a name="classificationresult-resource-type"></a><span data-ttu-id="fe011-103">tipo de recurso classificationResult</span><span class="sxs-lookup"><span data-stu-id="fe011-103">classificationResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe011-104">Representa o resultado de uma operação de classificação do mecanismo de classificação da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fe011-104">Represents the result of a classification operation from the Microsoft Classification Engine.</span></span> <span data-ttu-id="fe011-105">Os resultados de classificação de dados da proteção de informações do Azure, Office e outros serviços da Microsoft podem retornar um [conjunto bem definido de tipos de classificação](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="fe011-105">Data classification results from Azure Information Protection, Office, and other Microsoft services may return a [well-defined set of classification types](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span> <span data-ttu-id="fe011-106">Esses tipos podem ser fornecidos para a API [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) para resolver informações confidenciais em um rótulo de proteção de informações da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fe011-106">These types can be provided to the [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) API to resolve a sensitive information to a Microsoft Information Protection label.</span></span> 

## <a name="properties"></a><span data-ttu-id="fe011-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe011-107">Properties</span></span>

| <span data-ttu-id="fe011-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe011-108">Property</span></span>        | <span data-ttu-id="fe011-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe011-109">Type</span></span>  | <span data-ttu-id="fe011-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe011-110">Description</span></span>                                                            |
| :-------------- | :---- | :--------------------------------------------------------------------- |
| <span data-ttu-id="fe011-111">confidenceLevel</span><span class="sxs-lookup"><span data-stu-id="fe011-111">confidenceLevel</span></span> | <span data-ttu-id="fe011-112">Int32</span><span class="sxs-lookup"><span data-stu-id="fe011-112">Int32</span></span> | <span data-ttu-id="fe011-113">O nível de confiança, de 0 a 100, do resultado.</span><span class="sxs-lookup"><span data-stu-id="fe011-113">The confidence level, 0 to 100, of the result.</span></span>                         |
| <span data-ttu-id="fe011-114">Count</span><span class="sxs-lookup"><span data-stu-id="fe011-114">count</span></span>           | <span data-ttu-id="fe011-115">Int32</span><span class="sxs-lookup"><span data-stu-id="fe011-115">Int32</span></span> | <span data-ttu-id="fe011-116">O número de instâncias do tipo de informação específico na entrada.</span><span class="sxs-lookup"><span data-stu-id="fe011-116">The number of instances of the specific information type in the input.</span></span> |
| <span data-ttu-id="fe011-117">sensitiveTypeId</span><span class="sxs-lookup"><span data-stu-id="fe011-117">sensitiveTypeId</span></span> | <span data-ttu-id="fe011-118">GUID</span><span class="sxs-lookup"><span data-stu-id="fe011-118">GUID</span></span>  | <span data-ttu-id="fe011-119">O GUID do tipo de informação confidencial descoberto.</span><span class="sxs-lookup"><span data-stu-id="fe011-119">The GUID of the discovered sensitive information type.</span></span>                 |

## <a name="json-representation"></a><span data-ttu-id="fe011-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe011-120">JSON representation</span></span>

<span data-ttu-id="fe011-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe011-121">The following is a JSON representation of the resource.</span></span>

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
