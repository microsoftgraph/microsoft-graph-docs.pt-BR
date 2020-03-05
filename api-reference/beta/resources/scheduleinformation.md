---
title: tipo de recurso scheduleInformation
description: 'Representa a disponibilidade de um usuário, lista de distribuição ou recurso por um período de tempo especificado. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: ''
ms.openlocfilehash: e43bd0fc88cd8b7cdcb793deca8940ccaae9461f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520974"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="16c6b-103">tipo de recurso scheduleInformation</span><span class="sxs-lookup"><span data-stu-id="16c6b-103">scheduleInformation resource type</span></span>

<span data-ttu-id="16c6b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="16c6b-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="16c6b-105">Representa a disponibilidade de um usuário, lista de distribuição ou recurso (sala ou equipamento) por um período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="16c6b-105">Represents the availability of a user, distribution list, or resource (room or equipment) for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="16c6b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16c6b-106">Properties</span></span>
| <span data-ttu-id="16c6b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16c6b-107">Property</span></span>     | <span data-ttu-id="16c6b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="16c6b-108">Type</span></span>   |<span data-ttu-id="16c6b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="16c6b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16c6b-110">availabilityView</span><span class="sxs-lookup"><span data-stu-id="16c6b-110">availabilityView</span></span> |<span data-ttu-id="16c6b-111">String</span><span class="sxs-lookup"><span data-stu-id="16c6b-111">String</span></span> |<span data-ttu-id="16c6b-112">Representa um modo de exibição mesclado de disponibilidade de todos os `scheduleItems`itens no.</span><span class="sxs-lookup"><span data-stu-id="16c6b-112">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="16c6b-113">O modo de exibição consiste em intervalos de tempo.</span><span class="sxs-lookup"><span data-stu-id="16c6b-113">The view consists of time slots.</span></span> <span data-ttu-id="16c6b-114">A disponibilidade durante cada intervalo de tempo é indicada `0`por: = `1`livre, = `2`provisório, = `3`ocupado, = ausência temporária `4`, = trabalhando em outro lugar.</span><span class="sxs-lookup"><span data-stu-id="16c6b-114">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="16c6b-115">erro</span><span class="sxs-lookup"><span data-stu-id="16c6b-115">error</span></span> |[<span data-ttu-id="16c6b-116">freeBusyError</span><span class="sxs-lookup"><span data-stu-id="16c6b-116">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="16c6b-117">Informações de erro da tentativa de obter a disponibilidade do usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="16c6b-117">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="16c6b-118">ScheduleID</span><span class="sxs-lookup"><span data-stu-id="16c6b-118">scheduleId</span></span> |<span data-ttu-id="16c6b-119">String</span><span class="sxs-lookup"><span data-stu-id="16c6b-119">String</span></span> |<span data-ttu-id="16c6b-120">Um endereço SMTP do usuário, lista de distribuição ou recurso, identificando uma instância do **scheduleInformation**.</span><span class="sxs-lookup"><span data-stu-id="16c6b-120">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="16c6b-121">scheduleItems</span><span class="sxs-lookup"><span data-stu-id="16c6b-121">scheduleItems</span></span> |<span data-ttu-id="16c6b-122">coleção [scheduleItem](scheduleitem.md)</span><span class="sxs-lookup"><span data-stu-id="16c6b-122">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="16c6b-123">Contém os itens que descrevem a disponibilidade do usuário ou do recurso.</span><span class="sxs-lookup"><span data-stu-id="16c6b-123">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="16c6b-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="16c6b-124">workingHours</span></span> |[<span data-ttu-id="16c6b-125">workingHours</span><span class="sxs-lookup"><span data-stu-id="16c6b-125">workingHours</span></span>](workinghours.md) |<span data-ttu-id="16c6b-126">Os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="16c6b-126">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="16c6b-127">Eles são definidos como parte do [mailboxSettings](mailboxsettings.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="16c6b-127">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="16c6b-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16c6b-128">JSON representation</span></span>

<span data-ttu-id="16c6b-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16c6b-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleInformation"
}-->

```json
{
  "availabilityView": "String",
  "error": {"@odata.type": "microsoft.graph.freeBusyError"},
  "scheduleId": "String",
  "scheduleItems": [{"@odata.type": "microsoft.graph.scheduleItem"}],
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
