---
title: tipo de recurso inferenceData
description: tipo de recurso inferenceData
localization_priority: Normal
author: kevinbellinger
ms.prod: profile
doc_type: resourcePageType
ms.openlocfilehash: 2097dc14de984f3d1517b4d17e8043f38411b89a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496170"
---
# <a name="inferencedata-resource-type"></a><span data-ttu-id="5c984-103">tipo de recurso inferenceData</span><span class="sxs-lookup"><span data-stu-id="5c984-103">inferenceData resource type</span></span>

<span data-ttu-id="5c984-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5c984-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c984-105">O tipo de recurso [inferenceData](inferencedata.md) fornece detalhes adicionais sobre uma entidade que foi criada através de informações de referência sobre o usuário.</span><span class="sxs-lookup"><span data-stu-id="5c984-105">The [inferenceData](inferencedata.md) resource type provides additional detail about an entity which has been created through inferring information about the user.</span></span> <span data-ttu-id="5c984-106">Essas informações estarão presentes sempre que os dados dentro de uma entidade específica tiverem sido derivados de uma máquina de aprendizado ou de outro processo de sistema Iterando sobre os dados.</span><span class="sxs-lookup"><span data-stu-id="5c984-106">This information will be present whenever the data within a particular entity was derived from a machine learning or other system process iterating over data.</span></span>

## <a name="properties"></a><span data-ttu-id="5c984-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5c984-107">Properties</span></span>

| <span data-ttu-id="5c984-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c984-108">Property</span></span>              | <span data-ttu-id="5c984-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c984-109">Type</span></span>        | <span data-ttu-id="5c984-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c984-110">Description</span></span>                                                                     |
|:----------------------|:------------|:--------------------------------------------------------------------------------|
|<span data-ttu-id="5c984-111">confidenceScore</span><span class="sxs-lookup"><span data-stu-id="5c984-111">confidenceScore</span></span>        |<span data-ttu-id="5c984-112">Duplo</span><span class="sxs-lookup"><span data-stu-id="5c984-112">Double</span></span>       | <span data-ttu-id="5c984-113">A pontuação de confiança reflete a precisão dos dados inferidos sobre o usuário.</span><span class="sxs-lookup"><span data-stu-id="5c984-113">Confidence score reflecting the accuracy of the data inferred about the user.</span></span>   |
|<span data-ttu-id="5c984-114">userHasVerifiedAccuracy</span><span class="sxs-lookup"><span data-stu-id="5c984-114">userHasVerifiedAccuracy</span></span>|<span data-ttu-id="5c984-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c984-115">Boolean</span></span>      | <span data-ttu-id="5c984-116">Registros se o usuário confirmou essa inferência como true ou false.</span><span class="sxs-lookup"><span data-stu-id="5c984-116">Records if the user has confirmed this inference as being True or False.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="5c984-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5c984-117">JSON representation</span></span>

<span data-ttu-id="5c984-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5c984-118">The following is a JSON representation of the resource.</span></span>

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