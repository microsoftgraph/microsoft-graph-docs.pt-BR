---
title: tipo de recurso classificationResult
description: Representa o resultado de uma solicitação de classificação.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5281156752ceb290772daf841530b4ddb80350d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507660"
---
# <a name="classificationresult-resource-type"></a><span data-ttu-id="50240-103">tipo de recurso classificationResult</span><span class="sxs-lookup"><span data-stu-id="50240-103">classificationResult resource type</span></span>

<span data-ttu-id="50240-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="50240-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50240-105">Representa o resultado de uma operação de classificação do mecanismo de classificação da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="50240-105">Represents the result of a classification operation from the Microsoft Classification Engine.</span></span> <span data-ttu-id="50240-106">Os resultados de classificação de dados da proteção de informações do Azure, Office e outros serviços da Microsoft podem retornar um [conjunto bem definido de tipos de classificação](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="50240-106">Data classification results from Azure Information Protection, Office, and other Microsoft services may return a [well-defined set of classification types](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span> <span data-ttu-id="50240-107">Esses tipos podem ser fornecidos para a API [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) para resolver informações confidenciais em um rótulo de proteção de informações da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="50240-107">These types can be provided to the [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) API to resolve a sensitive information to a Microsoft Information Protection label.</span></span> 

## <a name="properties"></a><span data-ttu-id="50240-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50240-108">Properties</span></span>

| <span data-ttu-id="50240-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50240-109">Property</span></span>        | <span data-ttu-id="50240-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="50240-110">Type</span></span>  | <span data-ttu-id="50240-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="50240-111">Description</span></span>                                                            |
| :-------------- | :---- | :--------------------------------------------------------------------- |
| <span data-ttu-id="50240-112">confidenceLevel</span><span class="sxs-lookup"><span data-stu-id="50240-112">confidenceLevel</span></span> | <span data-ttu-id="50240-113">Int32</span><span class="sxs-lookup"><span data-stu-id="50240-113">Int32</span></span> | <span data-ttu-id="50240-114">O nível de confiança, de 0 a 100, do resultado.</span><span class="sxs-lookup"><span data-stu-id="50240-114">The confidence level, 0 to 100, of the result.</span></span>                         |
| <span data-ttu-id="50240-115">Count</span><span class="sxs-lookup"><span data-stu-id="50240-115">count</span></span>           | <span data-ttu-id="50240-116">Int32</span><span class="sxs-lookup"><span data-stu-id="50240-116">Int32</span></span> | <span data-ttu-id="50240-117">O número de instâncias do tipo de informação específico na entrada.</span><span class="sxs-lookup"><span data-stu-id="50240-117">The number of instances of the specific information type in the input.</span></span> |
| <span data-ttu-id="50240-118">sensitiveTypeId</span><span class="sxs-lookup"><span data-stu-id="50240-118">sensitiveTypeId</span></span> | <span data-ttu-id="50240-119">GUID</span><span class="sxs-lookup"><span data-stu-id="50240-119">GUID</span></span>  | <span data-ttu-id="50240-120">O GUID do tipo de informação confidencial descoberto.</span><span class="sxs-lookup"><span data-stu-id="50240-120">The GUID of the discovered sensitive information type.</span></span>                 |

## <a name="json-representation"></a><span data-ttu-id="50240-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50240-121">JSON representation</span></span>

<span data-ttu-id="50240-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50240-122">The following is a JSON representation of the resource.</span></span>

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
