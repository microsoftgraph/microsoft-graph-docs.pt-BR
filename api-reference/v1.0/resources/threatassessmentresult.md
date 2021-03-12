---
title: Tipo de recurso threatAssessmentResult
description: Representa um item de resultado de avaliação de ameaça.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0657cef555cd982c6649f6a8a4f40b7e5e15eaab
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722098"
---
# <a name="threatassessmentresult-resource-type"></a><span data-ttu-id="10adb-103">Tipo de recurso threatAssessmentResult</span><span class="sxs-lookup"><span data-stu-id="10adb-103">threatAssessmentResult resource type</span></span>

<span data-ttu-id="10adb-104">Representa um item de resultado de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="10adb-104">Represents a threat assessment result item.</span></span>

## <a name="properties"></a><span data-ttu-id="10adb-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10adb-105">Properties</span></span>

| <span data-ttu-id="10adb-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10adb-106">Property</span></span>     | <span data-ttu-id="10adb-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="10adb-107">Type</span></span>        | <span data-ttu-id="10adb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="10adb-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="10adb-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="10adb-109">createdDateTime</span></span>|<span data-ttu-id="10adb-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10adb-110">DateTimeOffset</span></span>|<span data-ttu-id="10adb-111">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="10adb-111">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="10adb-112">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="10adb-112">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="10adb-113">id</span><span class="sxs-lookup"><span data-stu-id="10adb-113">id</span></span>|<span data-ttu-id="10adb-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10adb-114">String</span></span>|<span data-ttu-id="10adb-115">A ID do resultado da avaliação de ameaças é um GUID (identificador global exclusivo).</span><span class="sxs-lookup"><span data-stu-id="10adb-115">The threat assessment result ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="10adb-116">mensagem</span><span class="sxs-lookup"><span data-stu-id="10adb-116">message</span></span>|<span data-ttu-id="10adb-117">String</span><span class="sxs-lookup"><span data-stu-id="10adb-117">String</span></span>|<span data-ttu-id="10adb-118">A mensagem de resultado para cada avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="10adb-118">The result message for each threat assessment.</span></span>|
|<span data-ttu-id="10adb-119">resultType</span><span class="sxs-lookup"><span data-stu-id="10adb-119">resultType</span></span>|[<span data-ttu-id="10adb-120">threatAssessmentResultType</span><span class="sxs-lookup"><span data-stu-id="10adb-120">threatAssessmentResultType</span></span>](enums.md#threatassessmentresulttype-values)|<span data-ttu-id="10adb-121">O tipo de resultado da avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="10adb-121">The threat assessment result type.</span></span> <span data-ttu-id="10adb-122">Os valores possíveis são: `checkPolicy` e `rescan`.</span><span class="sxs-lookup"><span data-stu-id="10adb-122">Possible values are: `checkPolicy`, `rescan`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10adb-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10adb-123">JSON representation</span></span>

<span data-ttu-id="10adb-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10adb-124">The following is a JSON representation of the resource.</span></span>

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

