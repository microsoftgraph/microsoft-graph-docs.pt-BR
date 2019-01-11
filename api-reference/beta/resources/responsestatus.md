---
title: Tipo de recurso responseStatus
description: O status de resposta de uma solicitação de reunião.
localization_priority: Normal
ms.openlocfilehash: b337422615e2c34791cd5181a446c25201c183e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843026"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="b11bc-103">Tipo de recurso responseStatus</span><span class="sxs-lookup"><span data-stu-id="b11bc-103">responseStatus resource type</span></span>

> <span data-ttu-id="b11bc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b11bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b11bc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b11bc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b11bc-106">O status de resposta de uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="b11bc-106">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="b11bc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b11bc-107">Properties</span></span>

| <span data-ttu-id="b11bc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b11bc-108">Property</span></span> | <span data-ttu-id="b11bc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b11bc-109">Type</span></span>           | <span data-ttu-id="b11bc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b11bc-110">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="b11bc-111">response</span><span class="sxs-lookup"><span data-stu-id="b11bc-111">response</span></span> | <span data-ttu-id="b11bc-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b11bc-112">String</span></span>         | <span data-ttu-id="b11bc-113">O tipo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b11bc-113">The response type.</span></span> <span data-ttu-id="b11bc-114">Os valores possíveis são: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="b11bc-114">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="b11bc-115">time</span><span class="sxs-lookup"><span data-stu-id="b11bc-115">time</span></span>     | <span data-ttu-id="b11bc-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b11bc-116">DateTimeOffset</span></span> | <span data-ttu-id="b11bc-p103">A data e hora em que a resposta retornou. Usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b11bc-p103">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="b11bc-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b11bc-120">JSON representation</span></span>

<span data-ttu-id="b11bc-121">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b11bc-121">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->

```json
{
  "response": "String",
  "time": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
