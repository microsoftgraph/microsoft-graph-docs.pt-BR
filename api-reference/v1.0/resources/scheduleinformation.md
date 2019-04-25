---
title: tipo de recurso scheduleInformation
description: Representa a disponibilidade de um usuário, lista de distribuição ou recurso por um período de tempo especificado.
localization_priority: Normal
ms.openlocfilehash: a19689eeafe9723cdadeb6147700933ab171637c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579265"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="13a61-103">tipo de recurso scheduleInformation</span><span class="sxs-lookup"><span data-stu-id="13a61-103">scheduleInformation resource type</span></span>

<span data-ttu-id="13a61-104">Representa a disponibilidade de um usuário, lista de distribuição ou recurso (sala ou equipamento) por um período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="13a61-104">Represents the availability of a user, distribution list, or resource (room or equipment) for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="13a61-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13a61-105">Properties</span></span>
| <span data-ttu-id="13a61-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13a61-106">Property</span></span>     | <span data-ttu-id="13a61-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="13a61-107">Type</span></span>   |<span data-ttu-id="13a61-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="13a61-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13a61-109">availabilityView</span><span class="sxs-lookup"><span data-stu-id="13a61-109">availabilityView</span></span> |<span data-ttu-id="13a61-110">String</span><span class="sxs-lookup"><span data-stu-id="13a61-110">String</span></span> |<span data-ttu-id="13a61-111">Representa um modo de exibição mesclado de disponibilidade de todos os `scheduleItems`itens no.</span><span class="sxs-lookup"><span data-stu-id="13a61-111">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="13a61-112">O modo de exibição consiste em intervalos de tempo.</span><span class="sxs-lookup"><span data-stu-id="13a61-112">The view consists of time slots.</span></span> <span data-ttu-id="13a61-113">A disponibilidade durante cada intervalo de tempo é indicada `0`por: = `1`livre, = `2`provisório, = `3`ocupado, = ausência temporária `4`, = trabalhando em outro lugar.</span><span class="sxs-lookup"><span data-stu-id="13a61-113">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="13a61-114">erro</span><span class="sxs-lookup"><span data-stu-id="13a61-114">error</span></span> |[<span data-ttu-id="13a61-115">freeBusyError</span><span class="sxs-lookup"><span data-stu-id="13a61-115">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="13a61-116">Informações de erro da tentativa de obter a disponibilidade do usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="13a61-116">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="13a61-117">ScheduleID</span><span class="sxs-lookup"><span data-stu-id="13a61-117">scheduleId</span></span> |<span data-ttu-id="13a61-118">String</span><span class="sxs-lookup"><span data-stu-id="13a61-118">String</span></span> |<span data-ttu-id="13a61-119">Um endereço SMTP do usuário, lista de distribuição ou recurso, identificando uma instância do **scheduleInformation**.</span><span class="sxs-lookup"><span data-stu-id="13a61-119">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="13a61-120">scheduleItems</span><span class="sxs-lookup"><span data-stu-id="13a61-120">scheduleItems</span></span> |<span data-ttu-id="13a61-121">coleção [scheduleItem](scheduleitem.md)</span><span class="sxs-lookup"><span data-stu-id="13a61-121">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="13a61-122">Contém os itens que descrevem a disponibilidade do usuário ou do recurso.</span><span class="sxs-lookup"><span data-stu-id="13a61-122">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="13a61-123">workingHours</span><span class="sxs-lookup"><span data-stu-id="13a61-123">workingHours</span></span> |[<span data-ttu-id="13a61-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="13a61-124">workingHours</span></span>](workinghours.md) |<span data-ttu-id="13a61-125">Os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="13a61-125">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="13a61-126">Eles são definidos como parte do [mailboxSettings](mailboxsettings.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="13a61-126">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="13a61-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13a61-127">JSON representation</span></span>

<span data-ttu-id="13a61-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13a61-128">The following is a JSON representation of the resource.</span></span>

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
