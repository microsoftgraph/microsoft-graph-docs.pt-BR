---
title: Tipo de recurso threatAssessmentResult
description: Representa um item de resultado de avaliação de ameaça.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 307b3bbebd9059ffee057781b5f647e407657684
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950259"
---
# <a name="threatassessmentresult-resource-type"></a><span data-ttu-id="fab4b-103">Tipo de recurso threatAssessmentResult</span><span class="sxs-lookup"><span data-stu-id="fab4b-103">threatAssessmentResult resource type</span></span>

<span data-ttu-id="fab4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fab4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fab4b-105">Representa um item de resultado de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="fab4b-105">Represents a threat assessment result item.</span></span>

## <a name="properties"></a><span data-ttu-id="fab4b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fab4b-106">Properties</span></span>

| <span data-ttu-id="fab4b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fab4b-107">Property</span></span>     | <span data-ttu-id="fab4b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fab4b-108">Type</span></span>        | <span data-ttu-id="fab4b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fab4b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fab4b-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fab4b-110">createdDateTime</span></span>|<span data-ttu-id="fab4b-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fab4b-111">DateTimeOffset</span></span>|<span data-ttu-id="fab4b-112">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="fab4b-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fab4b-113">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="fab4b-113">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="fab4b-114">id</span><span class="sxs-lookup"><span data-stu-id="fab4b-114">id</span></span>|<span data-ttu-id="fab4b-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fab4b-115">String</span></span>|<span data-ttu-id="fab4b-116">A ID do resultado da avaliação de ameaças é um GUID (identificador global exclusivo).</span><span class="sxs-lookup"><span data-stu-id="fab4b-116">The threat assessment result ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="fab4b-117">mensagem</span><span class="sxs-lookup"><span data-stu-id="fab4b-117">message</span></span>|<span data-ttu-id="fab4b-118">String</span><span class="sxs-lookup"><span data-stu-id="fab4b-118">String</span></span>|<span data-ttu-id="fab4b-119">A mensagem de resultado para cada avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="fab4b-119">The result message for each threat assessment.</span></span>|
|<span data-ttu-id="fab4b-120">resultType</span><span class="sxs-lookup"><span data-stu-id="fab4b-120">resultType</span></span>|<span data-ttu-id="fab4b-121">threatAssessmentResultType</span><span class="sxs-lookup"><span data-stu-id="fab4b-121">threatAssessmentResultType</span></span>|<span data-ttu-id="fab4b-122">O tipo de resultado da avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="fab4b-122">The threat assessment result type.</span></span> <span data-ttu-id="fab4b-123">Os valores possíveis são: `checkPolicy` (somente para avaliação de email), `rescan` .</span><span class="sxs-lookup"><span data-stu-id="fab4b-123">Possible values are: `checkPolicy` (only for mail assessment), `rescan`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fab4b-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fab4b-124">JSON representation</span></span>

<span data-ttu-id="fab4b-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fab4b-125">The following is a JSON representation of the resource.</span></span>

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


