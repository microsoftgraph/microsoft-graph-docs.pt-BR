---
title: tipo de recurso threatAssessmentResult
description: Representa um item de resultado de avaliação de ameaça.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b6f3b9bdf72a7bf7224693e694ba58868c0ed3ce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090883"
---
# <a name="threatassessmentresult-resource-type"></a><span data-ttu-id="4f68a-103">tipo de recurso threatAssessmentResult</span><span class="sxs-lookup"><span data-stu-id="4f68a-103">threatAssessmentResult resource type</span></span>

<span data-ttu-id="4f68a-104">Representa um item de resultado de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="4f68a-104">Represents a threat assessment result item.</span></span>

## <a name="properties"></a><span data-ttu-id="4f68a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4f68a-105">Properties</span></span>

| <span data-ttu-id="4f68a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f68a-106">Property</span></span>     | <span data-ttu-id="4f68a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f68a-107">Type</span></span>        | <span data-ttu-id="4f68a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f68a-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4f68a-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f68a-109">createdDateTime</span></span>|<span data-ttu-id="4f68a-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f68a-110">DateTimeOffset</span></span>|<span data-ttu-id="4f68a-111">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4f68a-111">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4f68a-112">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4f68a-112">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="4f68a-113">id</span><span class="sxs-lookup"><span data-stu-id="4f68a-113">id</span></span>|<span data-ttu-id="4f68a-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f68a-114">String</span></span>|<span data-ttu-id="4f68a-115">A ID do resultado da avaliação da ameaça é um identificador global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="4f68a-115">The threat assessment result ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="4f68a-116">mensagem</span><span class="sxs-lookup"><span data-stu-id="4f68a-116">message</span></span>|<span data-ttu-id="4f68a-117">String</span><span class="sxs-lookup"><span data-stu-id="4f68a-117">String</span></span>|<span data-ttu-id="4f68a-118">A mensagem de resultado para cada avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="4f68a-118">The result message for each threat assessment.</span></span>|
|<span data-ttu-id="4f68a-119">resultType</span><span class="sxs-lookup"><span data-stu-id="4f68a-119">resultType</span></span>|[<span data-ttu-id="4f68a-120">threatAssessmentResultType</span><span class="sxs-lookup"><span data-stu-id="4f68a-120">threatAssessmentResultType</span></span>](enums.md#threatassessmentresulttype-values)|<span data-ttu-id="4f68a-121">O tipo de resultado de avaliação da ameaça.</span><span class="sxs-lookup"><span data-stu-id="4f68a-121">The threat assessment result type.</span></span> <span data-ttu-id="4f68a-122">Os valores possíveis são: `checkPolicy` e `rescan`.</span><span class="sxs-lookup"><span data-stu-id="4f68a-122">Possible values are: `checkPolicy`, `rescan`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f68a-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4f68a-123">JSON representation</span></span>

<span data-ttu-id="4f68a-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4f68a-124">The following is a JSON representation of the resource.</span></span>

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

