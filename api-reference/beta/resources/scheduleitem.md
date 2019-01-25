---
title: tipo de recurso de scheduleItem
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: ed6b7441996cdf00b33be03f70afb888cc9bb251
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511349"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="eb858-104">tipo de recurso de scheduleItem</span><span class="sxs-lookup"><span data-stu-id="eb858-104">scheduleItem resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="eb858-105">Um item que descreve a disponibilidade de um usuário correspondente a um evento real no calendário de padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="eb858-105">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="eb858-106">Esse item se aplica a um recurso também.</span><span class="sxs-lookup"><span data-stu-id="eb858-106">This item applies to a resource as well.</span></span>

## <a name="properties"></a><span data-ttu-id="eb858-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb858-107">Properties</span></span>
| <span data-ttu-id="eb858-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb858-108">Property</span></span>     | <span data-ttu-id="eb858-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb858-109">Type</span></span>   |<span data-ttu-id="eb858-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb858-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb858-111">end</span><span class="sxs-lookup"><span data-stu-id="eb858-111">end</span></span> |[<span data-ttu-id="eb858-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="eb858-112">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="eb858-113">A data, hora e fuso horário que termina o evento correspondente.</span><span class="sxs-lookup"><span data-stu-id="eb858-113">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="eb858-114">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="eb858-114">isPrivate</span></span> |<span data-ttu-id="eb858-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb858-115">Boolean</span></span> |<span data-ttu-id="eb858-116">A sensibilidade do evento correspondente.</span><span class="sxs-lookup"><span data-stu-id="eb858-116">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="eb858-117">True se o evento é marcado como `private`, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="eb858-117">True if the event is marked `private`, false otherwise.</span></span> |
|<span data-ttu-id="eb858-118">location</span><span class="sxs-lookup"><span data-stu-id="eb858-118">location</span></span> |<span data-ttu-id="eb858-119">String</span><span class="sxs-lookup"><span data-stu-id="eb858-119">String</span></span> | <span data-ttu-id="eb858-120">O local onde o evento correspondente é mantido ou participou da.</span><span class="sxs-lookup"><span data-stu-id="eb858-120">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="eb858-121">Opcional.</span><span class="sxs-lookup"><span data-stu-id="eb858-121">Optional.</span></span>|
|<span data-ttu-id="eb858-122">start</span><span class="sxs-lookup"><span data-stu-id="eb858-122">start</span></span> |[<span data-ttu-id="eb858-123">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="eb858-123">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="eb858-124">A data, hora e fuso horário que inicia o evento correspondente.</span><span class="sxs-lookup"><span data-stu-id="eb858-124">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="eb858-125">status</span><span class="sxs-lookup"><span data-stu-id="eb858-125">status</span></span> |<span data-ttu-id="eb858-126">String</span><span class="sxs-lookup"><span data-stu-id="eb858-126">String</span></span> | <span data-ttu-id="eb858-127">O status de disponibilidade do usuário ou recurso durante o evento correspondente.</span><span class="sxs-lookup"><span data-stu-id="eb858-127">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="eb858-128">Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="eb858-128">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="eb858-129">subject</span><span class="sxs-lookup"><span data-stu-id="eb858-129">subject</span></span> |<span data-ttu-id="eb858-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb858-130">String</span></span> | <span data-ttu-id="eb858-131">Linha de assunto do evento correspondente.</span><span class="sxs-lookup"><span data-stu-id="eb858-131">The corresponding event's subject line.</span></span> <span data-ttu-id="eb858-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="eb858-132">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="eb858-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb858-133">JSON representation</span></span>

<span data-ttu-id="eb858-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb858-134">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
