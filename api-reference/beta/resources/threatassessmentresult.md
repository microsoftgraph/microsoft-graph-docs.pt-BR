---
title: tipo de recurso threatAssessmentResult
description: Representa um item de resultado de avaliação de ameaça.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cde4965d1b535b9ca147fda175556b8d3637e308
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075536"
---
# <a name="threatassessmentresult-resource-type"></a><span data-ttu-id="d9566-103">tipo de recurso threatAssessmentResult</span><span class="sxs-lookup"><span data-stu-id="d9566-103">threatAssessmentResult resource type</span></span>

<span data-ttu-id="d9566-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9566-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9566-105">Representa um item de resultado de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="d9566-105">Represents a threat assessment result item.</span></span>

## <a name="properties"></a><span data-ttu-id="d9566-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9566-106">Properties</span></span>

| <span data-ttu-id="d9566-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9566-107">Property</span></span>     | <span data-ttu-id="d9566-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9566-108">Type</span></span>        | <span data-ttu-id="d9566-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9566-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d9566-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9566-110">createdDateTime</span></span>|<span data-ttu-id="d9566-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9566-111">DateTimeOffset</span></span>|<span data-ttu-id="d9566-112">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d9566-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d9566-113">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d9566-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="d9566-114">id</span><span class="sxs-lookup"><span data-stu-id="d9566-114">id</span></span>|<span data-ttu-id="d9566-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9566-115">String</span></span>|<span data-ttu-id="d9566-116">A ID do resultado da avaliação da ameaça é um identificador global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="d9566-116">The threat assessment result ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="d9566-117">mensagem</span><span class="sxs-lookup"><span data-stu-id="d9566-117">message</span></span>|<span data-ttu-id="d9566-118">String</span><span class="sxs-lookup"><span data-stu-id="d9566-118">String</span></span>|<span data-ttu-id="d9566-119">A mensagem de resultado para cada avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="d9566-119">The result message for each threat assessment.</span></span>|
|<span data-ttu-id="d9566-120">resultType</span><span class="sxs-lookup"><span data-stu-id="d9566-120">resultType</span></span>|[<span data-ttu-id="d9566-121">threatAssessmentResultType</span><span class="sxs-lookup"><span data-stu-id="d9566-121">threatAssessmentResultType</span></span>](enums.md#threatassessmentresulttype-values)|<span data-ttu-id="d9566-122">O tipo de resultado de avaliação da ameaça.</span><span class="sxs-lookup"><span data-stu-id="d9566-122">The threat assessment result type.</span></span> <span data-ttu-id="d9566-123">Os valores possíveis são: `checkPolicy` e `rescan`.</span><span class="sxs-lookup"><span data-stu-id="d9566-123">Possible values are: `checkPolicy`, `rescan`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d9566-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9566-124">JSON representation</span></span>

<span data-ttu-id="d9566-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d9566-125">The following is a JSON representation of the resource.</span></span>

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


