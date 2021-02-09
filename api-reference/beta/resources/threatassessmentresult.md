---
title: Tipo de recurso threatAssessmentResult
description: Representa um item de resultado da avaliação de ameaças.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 35a5d10b631a22f19c881b1d3c2326ab6b09b46c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155514"
---
# <a name="threatassessmentresult-resource-type"></a><span data-ttu-id="d7e27-103">Tipo de recurso threatAssessmentResult</span><span class="sxs-lookup"><span data-stu-id="d7e27-103">threatAssessmentResult resource type</span></span>

<span data-ttu-id="d7e27-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7e27-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7e27-105">Representa um item de resultado da avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="d7e27-105">Represents a threat assessment result item.</span></span>

## <a name="properties"></a><span data-ttu-id="d7e27-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d7e27-106">Properties</span></span>

| <span data-ttu-id="d7e27-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7e27-107">Property</span></span>     | <span data-ttu-id="d7e27-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7e27-108">Type</span></span>        | <span data-ttu-id="d7e27-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7e27-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d7e27-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7e27-110">createdDateTime</span></span>|<span data-ttu-id="d7e27-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7e27-111">DateTimeOffset</span></span>|<span data-ttu-id="d7e27-112">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d7e27-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d7e27-113">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d7e27-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="d7e27-114">id</span><span class="sxs-lookup"><span data-stu-id="d7e27-114">id</span></span>|<span data-ttu-id="d7e27-115">String</span><span class="sxs-lookup"><span data-stu-id="d7e27-115">String</span></span>|<span data-ttu-id="d7e27-116">A ID do resultado da avaliação de ameaças é um identificador global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="d7e27-116">The threat assessment result ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="d7e27-117">mensagem</span><span class="sxs-lookup"><span data-stu-id="d7e27-117">message</span></span>|<span data-ttu-id="d7e27-118">String</span><span class="sxs-lookup"><span data-stu-id="d7e27-118">String</span></span>|<span data-ttu-id="d7e27-119">A mensagem de resultado para cada avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="d7e27-119">The result message for each threat assessment.</span></span>|
|<span data-ttu-id="d7e27-120">resultType</span><span class="sxs-lookup"><span data-stu-id="d7e27-120">resultType</span></span>|[<span data-ttu-id="d7e27-121">threatAssessmentResultType</span><span class="sxs-lookup"><span data-stu-id="d7e27-121">threatAssessmentResultType</span></span>](enums.md#threatassessmentresulttype-values)|<span data-ttu-id="d7e27-122">O tipo de resultado da avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="d7e27-122">The threat assessment result type.</span></span> <span data-ttu-id="d7e27-123">Os valores possíveis são: `checkPolicy` e `rescan`.</span><span class="sxs-lookup"><span data-stu-id="d7e27-123">Possible values are: `checkPolicy`, `rescan`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7e27-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d7e27-124">JSON representation</span></span>

<span data-ttu-id="d7e27-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d7e27-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.threatAssessmentResult",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "message": "String",
  "resultType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "threatAssessmentResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


