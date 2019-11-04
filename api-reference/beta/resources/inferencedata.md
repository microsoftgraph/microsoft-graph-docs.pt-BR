---
title: tipo de recurso inferenceData
description: tipo de recurso inferenceData
localization_priority: Normal
author: kevinbellinger
ms.prod: profile
doc_type: resourcePageType
ms.openlocfilehash: 43d6585243eed560a6a8f77268305b7d7f5824a8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938846"
---
# <a name="inferencedata-resource-type"></a><span data-ttu-id="1e2a9-103">tipo de recurso inferenceData</span><span class="sxs-lookup"><span data-stu-id="1e2a9-103">inferenceData resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e2a9-104">O tipo de recurso [inferenceData](inferencedata.md) fornece detalhes adicionais sobre uma entidade que foi criada através de informações de referência sobre o usuário.</span><span class="sxs-lookup"><span data-stu-id="1e2a9-104">The [inferenceData](inferencedata.md) resource type provides additional detail about an entity which has been created through inferring information about the user.</span></span> <span data-ttu-id="1e2a9-105">Essas informações estarão presentes sempre que os dados dentro de uma entidade específica tiverem sido derivados de uma máquina de aprendizado ou de outro processo de sistema Iterando sobre os dados.</span><span class="sxs-lookup"><span data-stu-id="1e2a9-105">This information will be present whenever the data within a particular entity was derived from a machine learning or other system process iterating over data.</span></span>

## <a name="properties"></a><span data-ttu-id="1e2a9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e2a9-106">Properties</span></span>

| <span data-ttu-id="1e2a9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e2a9-107">Property</span></span>              | <span data-ttu-id="1e2a9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e2a9-108">Type</span></span>        | <span data-ttu-id="1e2a9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e2a9-109">Description</span></span>                                                                     |
|:----------------------|:------------|:--------------------------------------------------------------------------------|
|<span data-ttu-id="1e2a9-110">confidenceScore</span><span class="sxs-lookup"><span data-stu-id="1e2a9-110">confidenceScore</span></span>        |<span data-ttu-id="1e2a9-111">Duplo</span><span class="sxs-lookup"><span data-stu-id="1e2a9-111">Double</span></span>       | <span data-ttu-id="1e2a9-112">A pontuação de confiança reflete a precisão dos dados inferidos sobre o usuário.</span><span class="sxs-lookup"><span data-stu-id="1e2a9-112">Confidence score reflecting the accuracy of the data inferred about the user.</span></span>   |
|<span data-ttu-id="1e2a9-113">userHasVerifiedAccuracy</span><span class="sxs-lookup"><span data-stu-id="1e2a9-113">userHasVerifiedAccuracy</span></span>|<span data-ttu-id="1e2a9-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e2a9-114">Boolean</span></span>      | <span data-ttu-id="1e2a9-115">Registros se o usuário confirmou essa inferência como true ou false.</span><span class="sxs-lookup"><span data-stu-id="1e2a9-115">Records if the user has confirmed this inference as being True or False.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="1e2a9-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e2a9-116">JSON representation</span></span>

<span data-ttu-id="1e2a9-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e2a9-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceData",
  "baseType": null
}-->

```json
{
  "confidenceScore": 1024,
  "userHasVerifiedAccuracy": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->