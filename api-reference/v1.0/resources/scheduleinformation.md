---
title: tipo de recurso scheduleInformation
description: Representa a disponibilidade de um usuário, lista de distribuição ou recurso por um período de tempo especificado.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 50c5b3fc5109493f8036ee00d996d92b0ac73098
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812636"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="0299b-103">tipo de recurso scheduleInformation</span><span class="sxs-lookup"><span data-stu-id="0299b-103">scheduleInformation resource type</span></span>

<span data-ttu-id="0299b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0299b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0299b-105">Representa a disponibilidade de um usuário, lista de distribuição ou recurso (sala ou equipamento) por um período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="0299b-105">Represents the availability of a user, distribution list, or resource (room or equipment) for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="0299b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0299b-106">Properties</span></span>
| <span data-ttu-id="0299b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0299b-107">Property</span></span>     | <span data-ttu-id="0299b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0299b-108">Type</span></span>   |<span data-ttu-id="0299b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0299b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0299b-110">availabilityView</span><span class="sxs-lookup"><span data-stu-id="0299b-110">availabilityView</span></span> |<span data-ttu-id="0299b-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0299b-111">String</span></span> |<span data-ttu-id="0299b-112">Representa um modo de exibição mesclado de disponibilidade de todos os itens no `scheduleItems` .</span><span class="sxs-lookup"><span data-stu-id="0299b-112">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="0299b-113">O modo de exibição consiste em intervalos de tempo.</span><span class="sxs-lookup"><span data-stu-id="0299b-113">The view consists of time slots.</span></span> <span data-ttu-id="0299b-114">A disponibilidade durante cada intervalo de tempo é indicada por: `0` = livre, `1` = provisório, `2` = ocupado, `3` = ausência temporária, `4` = trabalhando em outro lugar.</span><span class="sxs-lookup"><span data-stu-id="0299b-114">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="0299b-115">erro</span><span class="sxs-lookup"><span data-stu-id="0299b-115">error</span></span> |[<span data-ttu-id="0299b-116">freeBusyError</span><span class="sxs-lookup"><span data-stu-id="0299b-116">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="0299b-117">Informações de erro da tentativa de obter a disponibilidade do usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="0299b-117">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="0299b-118">ScheduleID</span><span class="sxs-lookup"><span data-stu-id="0299b-118">scheduleId</span></span> |<span data-ttu-id="0299b-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0299b-119">String</span></span> |<span data-ttu-id="0299b-120">Um endereço SMTP do usuário, lista de distribuição ou recurso, identificando uma instância do **scheduleInformation**.</span><span class="sxs-lookup"><span data-stu-id="0299b-120">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="0299b-121">scheduleItems</span><span class="sxs-lookup"><span data-stu-id="0299b-121">scheduleItems</span></span> |<span data-ttu-id="0299b-122">coleção [scheduleItem](scheduleitem.md)</span><span class="sxs-lookup"><span data-stu-id="0299b-122">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="0299b-123">Contém os itens que descrevem a disponibilidade do usuário ou do recurso.</span><span class="sxs-lookup"><span data-stu-id="0299b-123">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="0299b-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="0299b-124">workingHours</span></span> |[<span data-ttu-id="0299b-125">workingHours</span><span class="sxs-lookup"><span data-stu-id="0299b-125">workingHours</span></span>](workinghours.md) |<span data-ttu-id="0299b-126">Os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="0299b-126">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="0299b-127">Eles são definidos como parte do [mailboxSettings](mailboxsettings.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="0299b-127">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0299b-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0299b-128">JSON representation</span></span>

<span data-ttu-id="0299b-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0299b-129">The following is a JSON representation of the resource.</span></span>

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
  "tocPath": ""
}
-->
