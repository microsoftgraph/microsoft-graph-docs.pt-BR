---
title: tipo de recurso termsExpiration
description: Fornece configurações adicionais ao definir a expiração agendada do contrato.
localization_priority: Normal
ms.prod: microsoft-identity-platform
author: raprakasMSFT
doc_type: resourcePageType
ms.openlocfilehash: 5acacae700bfddcfe68431e03b2a5b03e00fed8a
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777705"
---
# <a name="termsexpiration-resource-type"></a><span data-ttu-id="43cd8-103">tipo de recurso termsExpiration</span><span class="sxs-lookup"><span data-stu-id="43cd8-103">termsExpiration resource type</span></span>

<span data-ttu-id="43cd8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43cd8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43cd8-105">Fornece configurações adicionais ao definir a expiração agendada do contrato.</span><span class="sxs-lookup"><span data-stu-id="43cd8-105">Provides additional settings when setting the scheduled expiration of the agreement.</span></span>

## <a name="properties"></a><span data-ttu-id="43cd8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43cd8-106">Properties</span></span>

| <span data-ttu-id="43cd8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43cd8-107">Property</span></span>                     | <span data-ttu-id="43cd8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="43cd8-108">Type</span></span>                      | <span data-ttu-id="43cd8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="43cd8-109">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="43cd8-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="43cd8-110">startDateTime</span></span>|<span data-ttu-id="43cd8-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43cd8-111">DateTimeOffset</span></span> | <span data-ttu-id="43cd8-112">O DateTime quando o contrato é definido como expire para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="43cd8-112">The DateTime when the agreement is set to expire for all users.</span></span> <span data-ttu-id="43cd8-113">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="43cd8-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="43cd8-114">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="43cd8-114">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
| <span data-ttu-id="43cd8-115">proje</span><span class="sxs-lookup"><span data-stu-id="43cd8-115">frequency</span></span>| <span data-ttu-id="43cd8-116">Duração</span><span class="sxs-lookup"><span data-stu-id="43cd8-116">Duration</span></span> | <span data-ttu-id="43cd8-117">Representa a frequência na qual os termos expiram, após sua primeira expiração, conforme definido em **StartDateTime**.</span><span class="sxs-lookup"><span data-stu-id="43cd8-117">Represents the frequency at which the terms will expire, after its first expiration as set in **startDateTime**.</span></span> <span data-ttu-id="43cd8-118">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="43cd8-118">The value is represented in ISO 8601 format for durations.</span></span> <span data-ttu-id="43cd8-119">Por exemplo, `PT1M` representa um período de tempo de 1 mês.</span><span class="sxs-lookup"><span data-stu-id="43cd8-119">For example, `PT1M` represents a time period of 1 month.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43cd8-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43cd8-120">JSON representation</span></span>

<span data-ttu-id="43cd8-121">Veja a seguir uma representação JSON desse recurso.</span><span class="sxs-lookup"><span data-stu-id="43cd8-121">The following is a JSON representation of this resource.</span></span>

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


