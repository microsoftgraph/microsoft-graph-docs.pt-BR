---
title: tipo de recurso de scheduleItem
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: e5d14826a27153af27648484554ec864d62ed6c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890430"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="73dc1-104">tipo de recurso de scheduleItem</span><span class="sxs-lookup"><span data-stu-id="73dc1-104">scheduleItem resource type</span></span>

 > <span data-ttu-id="73dc1-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="73dc1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73dc1-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="73dc1-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="73dc1-107">Um item que descreve a disponibilidade de um usuário correspondente a um evento real no calendário de padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="73dc1-107">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="73dc1-108">Esse item se aplica a um recurso também.</span><span class="sxs-lookup"><span data-stu-id="73dc1-108">This item applies to a resource as well.</span></span>

## <a name="properties"></a><span data-ttu-id="73dc1-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73dc1-109">Properties</span></span>
| <span data-ttu-id="73dc1-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73dc1-110">Property</span></span>     | <span data-ttu-id="73dc1-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="73dc1-111">Type</span></span>   |<span data-ttu-id="73dc1-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="73dc1-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73dc1-113">end</span><span class="sxs-lookup"><span data-stu-id="73dc1-113">end</span></span> |[<span data-ttu-id="73dc1-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="73dc1-114">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="73dc1-115">A data, hora e fuso horário que termina o evento correspondente.</span><span class="sxs-lookup"><span data-stu-id="73dc1-115">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="73dc1-116">isPrivate</span><span class="sxs-lookup"><span data-stu-id="73dc1-116">isPrivate</span></span> |<span data-ttu-id="73dc1-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="73dc1-117">Boolean</span></span> |<span data-ttu-id="73dc1-118">A sensibilidade do evento correspondente.</span><span class="sxs-lookup"><span data-stu-id="73dc1-118">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="73dc1-119">True se o evento é marcado como `private`, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="73dc1-119">True if the event is marked `private`, false otherwise.</span></span> |
|<span data-ttu-id="73dc1-120">location</span><span class="sxs-lookup"><span data-stu-id="73dc1-120">location</span></span> |<span data-ttu-id="73dc1-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73dc1-121">String</span></span> | <span data-ttu-id="73dc1-122">O local onde o evento correspondente é mantido ou participou da.</span><span class="sxs-lookup"><span data-stu-id="73dc1-122">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="73dc1-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="73dc1-123">Optional.</span></span>|
|<span data-ttu-id="73dc1-124">start</span><span class="sxs-lookup"><span data-stu-id="73dc1-124">start</span></span> |[<span data-ttu-id="73dc1-125">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="73dc1-125">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="73dc1-126">A data, hora e fuso horário que inicia o evento correspondente.</span><span class="sxs-lookup"><span data-stu-id="73dc1-126">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="73dc1-127">status</span><span class="sxs-lookup"><span data-stu-id="73dc1-127">status</span></span> |<span data-ttu-id="73dc1-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73dc1-128">String</span></span> | <span data-ttu-id="73dc1-129">O status de disponibilidade do usuário ou recurso durante o evento correspondente.</span><span class="sxs-lookup"><span data-stu-id="73dc1-129">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="73dc1-130">Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="73dc1-130">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="73dc1-131">subject</span><span class="sxs-lookup"><span data-stu-id="73dc1-131">subject</span></span> |<span data-ttu-id="73dc1-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73dc1-132">String</span></span> | <span data-ttu-id="73dc1-133">Linha de assunto do evento correspondente.</span><span class="sxs-lookup"><span data-stu-id="73dc1-133">The corresponding event's subject line.</span></span> <span data-ttu-id="73dc1-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="73dc1-134">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="73dc1-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73dc1-135">JSON representation</span></span>

<span data-ttu-id="73dc1-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73dc1-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleItem"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "isPrivate": true,
  "location": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
