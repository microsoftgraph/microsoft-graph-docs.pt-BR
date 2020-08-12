---
title: tipo de recurso termsExpiration
description: Fornece configurações adicionais ao definir a expiração agendada do contrato.
localization_priority: Normal
ms.prod: microsoft-identity-platform
author: raprakasMSFT
doc_type: resourcePageType
ms.openlocfilehash: e811e4816fa63e98201d1a14403d6c3525ace2c0
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/12/2020
ms.locfileid: "46644022"
---
# <a name="termsexpiration-resource-type"></a><span data-ttu-id="80bd4-103">tipo de recurso termsExpiration</span><span class="sxs-lookup"><span data-stu-id="80bd4-103">termsExpiration resource type</span></span>

<span data-ttu-id="80bd4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80bd4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80bd4-105">Fornece configurações adicionais ao definir a expiração agendada do contrato.</span><span class="sxs-lookup"><span data-stu-id="80bd4-105">Provides additional settings when setting the scheduled expiration of the agreement.</span></span>

## <a name="properties"></a><span data-ttu-id="80bd4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80bd4-106">Properties</span></span>

| <span data-ttu-id="80bd4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80bd4-107">Property</span></span>                     | <span data-ttu-id="80bd4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="80bd4-108">Type</span></span>                      | <span data-ttu-id="80bd4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="80bd4-109">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="80bd4-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="80bd4-110">startDateTime</span></span>|<span data-ttu-id="80bd4-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80bd4-111">DateTimeOffset</span></span> | <span data-ttu-id="80bd4-112">O DateTime quando o contrato é definido como expire para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="80bd4-112">The DateTime when the agreement is set to expire for all users.</span></span> <span data-ttu-id="80bd4-113">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="80bd4-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="80bd4-114">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="80bd4-114">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
| <span data-ttu-id="80bd4-115">proje</span><span class="sxs-lookup"><span data-stu-id="80bd4-115">frequency</span></span>| <span data-ttu-id="80bd4-116">Duração</span><span class="sxs-lookup"><span data-stu-id="80bd4-116">Duration</span></span> | <span data-ttu-id="80bd4-117">Isso representa a frequência com a qual os termos expiram, após a primeira expiração definida em ' startDatetime '.</span><span class="sxs-lookup"><span data-stu-id="80bd4-117">This represents the frequency at which the terms will expire, after its first expiration as set in 'startDateTime'.</span></span> <span data-ttu-id="80bd4-118">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="80bd4-118">The value is represented in ISO 8601 format for durations.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="80bd4-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80bd4-119">JSON representation</span></span>

<span data-ttu-id="80bd4-120">Veja a seguir uma representação JSON desse recurso.</span><span class="sxs-lookup"><span data-stu-id="80bd4-120">The following is a JSON representation of this resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.termsExpiration",
  "baseType": ""
}-->

```json
{
   "startDateTime": "2018-10-01T00:00:00.0000000Z",
   "frequency": ""
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
