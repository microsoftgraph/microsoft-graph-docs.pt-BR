---
title: tipo de recurso threatAssessmentResult
description: Representa um item de resultado de avaliação de ameaça.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e654c3c8878db10f160a4c4909fe2a8ca8b5d184
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591499"
---
# <a name="threatassessmentresult-resource-type"></a><span data-ttu-id="e78c9-103">tipo de recurso threatAssessmentResult</span><span class="sxs-lookup"><span data-stu-id="e78c9-103">threatAssessmentResult resource type</span></span>

<span data-ttu-id="e78c9-104">Representa um item de resultado de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="e78c9-104">Represents a threat assessment result item.</span></span>

## <a name="properties"></a><span data-ttu-id="e78c9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e78c9-105">Properties</span></span>

| <span data-ttu-id="e78c9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e78c9-106">Property</span></span>     | <span data-ttu-id="e78c9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e78c9-107">Type</span></span>        | <span data-ttu-id="e78c9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e78c9-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e78c9-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e78c9-109">createdDateTime</span></span>|<span data-ttu-id="e78c9-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e78c9-110">DateTimeOffset</span></span>|<span data-ttu-id="e78c9-111">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e78c9-111">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e78c9-112">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e78c9-112">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e78c9-113">id</span><span class="sxs-lookup"><span data-stu-id="e78c9-113">id</span></span>|<span data-ttu-id="e78c9-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e78c9-114">String</span></span>|<span data-ttu-id="e78c9-115">A ID do resultado da avaliação da ameaça é um identificador global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="e78c9-115">The threat assessment result ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="e78c9-116">mensagem</span><span class="sxs-lookup"><span data-stu-id="e78c9-116">message</span></span>|<span data-ttu-id="e78c9-117">String</span><span class="sxs-lookup"><span data-stu-id="e78c9-117">String</span></span>|<span data-ttu-id="e78c9-118">A mensagem de resultado para cada avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="e78c9-118">The result message for each threat assessment.</span></span>|
|<span data-ttu-id="e78c9-119">resultType</span><span class="sxs-lookup"><span data-stu-id="e78c9-119">resultType</span></span>|[<span data-ttu-id="e78c9-120">threatAssessmentResultType</span><span class="sxs-lookup"><span data-stu-id="e78c9-120">threatAssessmentResultType</span></span>](enums.md#threatassessmentresulttype-values)|<span data-ttu-id="e78c9-121">O tipo de resultado de avaliação da ameaça.</span><span class="sxs-lookup"><span data-stu-id="e78c9-121">The threat assessment result type.</span></span> <span data-ttu-id="e78c9-122">Os valores possíveis são: `checkPolicy` e `rescan`.</span><span class="sxs-lookup"><span data-stu-id="e78c9-122">Possible values are: `checkPolicy`, `rescan`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e78c9-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e78c9-123">JSON representation</span></span>

<span data-ttu-id="e78c9-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e78c9-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.threatAssessmentResult",
  "baseType": "",
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
