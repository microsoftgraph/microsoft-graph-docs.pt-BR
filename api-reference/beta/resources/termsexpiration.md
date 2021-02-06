---
title: Tipo de recurso termsExpiration
description: Fornece configurações adicionais ao definir a expiração agendada do contrato.
localization_priority: Normal
ms.prod: governance
author: raprakasMSFT
doc_type: resourcePageType
ms.openlocfilehash: 3f31489a80c87dd17a31500818c0c650c57c8a7c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128502"
---
# <a name="termsexpiration-resource-type"></a><span data-ttu-id="30c8e-103">Tipo de recurso termsExpiration</span><span class="sxs-lookup"><span data-stu-id="30c8e-103">termsExpiration resource type</span></span>

<span data-ttu-id="30c8e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30c8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30c8e-105">Fornece configurações adicionais ao definir a expiração agendada do contrato.</span><span class="sxs-lookup"><span data-stu-id="30c8e-105">Provides additional settings when setting the scheduled expiration of the agreement.</span></span>

## <a name="properties"></a><span data-ttu-id="30c8e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="30c8e-106">Properties</span></span>

| <span data-ttu-id="30c8e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30c8e-107">Property</span></span>                     | <span data-ttu-id="30c8e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="30c8e-108">Type</span></span>                      | <span data-ttu-id="30c8e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="30c8e-109">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="30c8e-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="30c8e-110">startDateTime</span></span>|<span data-ttu-id="30c8e-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30c8e-111">DateTimeOffset</span></span> | <span data-ttu-id="30c8e-112">DateTime quando o contrato está definido para expirar para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="30c8e-112">The DateTime when the agreement is set to expire for all users.</span></span> <span data-ttu-id="30c8e-113">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="30c8e-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="30c8e-114">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="30c8e-114">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
| <span data-ttu-id="30c8e-115">frequency</span><span class="sxs-lookup"><span data-stu-id="30c8e-115">frequency</span></span>| <span data-ttu-id="30c8e-116">Duration</span><span class="sxs-lookup"><span data-stu-id="30c8e-116">Duration</span></span> | <span data-ttu-id="30c8e-117">Representa a frequência na qual os termos expiram, após sua primeira expiração, conforme definido em **startDateTime**.</span><span class="sxs-lookup"><span data-stu-id="30c8e-117">Represents the frequency at which the terms will expire, after its first expiration as set in **startDateTime**.</span></span> <span data-ttu-id="30c8e-118">O valor é representado no formato ISO 8601 por durações.</span><span class="sxs-lookup"><span data-stu-id="30c8e-118">The value is represented in ISO 8601 format for durations.</span></span> <span data-ttu-id="30c8e-119">Por exemplo, `PT1M` representa um período de tempo de 1 mês.</span><span class="sxs-lookup"><span data-stu-id="30c8e-119">For example, `PT1M` represents a time period of 1 month.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30c8e-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="30c8e-120">JSON representation</span></span>

<span data-ttu-id="30c8e-121">A seguir está uma representação JSON desse recurso.</span><span class="sxs-lookup"><span data-stu-id="30c8e-121">The following is a JSON representation of this resource.</span></span>

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


