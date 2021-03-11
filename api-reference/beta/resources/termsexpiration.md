---
title: tipo de recurso termsExpiration
description: Fornece configurações adicionais ao definir a expiração agendada do contrato.
localization_priority: Normal
ms.prod: governance
author: raprakasMSFT
doc_type: resourcePageType
ms.openlocfilehash: 29489f3e225b24cc57c20826d9a6071c2a501154
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721723"
---
# <a name="termsexpiration-resource-type"></a><span data-ttu-id="587b8-103">tipo de recurso termsExpiration</span><span class="sxs-lookup"><span data-stu-id="587b8-103">termsExpiration resource type</span></span>

<span data-ttu-id="587b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="587b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="587b8-105">Fornece configurações adicionais ao definir a expiração agendada do contrato.</span><span class="sxs-lookup"><span data-stu-id="587b8-105">Provides additional settings when setting the scheduled expiration of the agreement.</span></span>

## <a name="properties"></a><span data-ttu-id="587b8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="587b8-106">Properties</span></span>

| <span data-ttu-id="587b8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="587b8-107">Property</span></span>                     | <span data-ttu-id="587b8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="587b8-108">Type</span></span>                      | <span data-ttu-id="587b8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="587b8-109">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="587b8-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="587b8-110">startDateTime</span></span>|<span data-ttu-id="587b8-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="587b8-111">DateTimeOffset</span></span> | <span data-ttu-id="587b8-112">DateTime quando o contrato está definido para expirar para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="587b8-112">The DateTime when the agreement is set to expire for all users.</span></span> <span data-ttu-id="587b8-113">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="587b8-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="587b8-114">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="587b8-114">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
| <span data-ttu-id="587b8-115">frequency</span><span class="sxs-lookup"><span data-stu-id="587b8-115">frequency</span></span>| <span data-ttu-id="587b8-116">Duration</span><span class="sxs-lookup"><span data-stu-id="587b8-116">Duration</span></span> | <span data-ttu-id="587b8-117">Representa a frequência na qual os termos expiram, após sua primeira expiração, conforme definido em **startDateTime**.</span><span class="sxs-lookup"><span data-stu-id="587b8-117">Represents the frequency at which the terms will expire, after its first expiration as set in **startDateTime**.</span></span> <span data-ttu-id="587b8-118">O valor é representado no formato ISO 8601 por durações.</span><span class="sxs-lookup"><span data-stu-id="587b8-118">The value is represented in ISO 8601 format for durations.</span></span> <span data-ttu-id="587b8-119">Por exemplo, `PT1M` representa um período de tempo de 1 mês.</span><span class="sxs-lookup"><span data-stu-id="587b8-119">For example, `PT1M` represents a time period of 1 month.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="587b8-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="587b8-120">JSON representation</span></span>

<span data-ttu-id="587b8-121">A seguir está uma representação JSON desse recurso.</span><span class="sxs-lookup"><span data-stu-id="587b8-121">The following is a JSON representation of this resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.termsExpiration",
}-->

```json
{
   "startDateTime": "2018-10-01T00:00:00.0000000Z",
   "frequency": "Duration"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "termsExpiration complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


