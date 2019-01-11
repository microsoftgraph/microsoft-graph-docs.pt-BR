---
title: tipo de recurso de scheduleInformation
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: e535f5c2b47e810fc767cb29d0b24f28ed3c7bf0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828704"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="51871-104">tipo de recurso de scheduleInformation</span><span class="sxs-lookup"><span data-stu-id="51871-104">scheduleInformation resource type</span></span>

 > <span data-ttu-id="51871-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="51871-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51871-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="51871-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="51871-107">Representa a disponibilidade de um usuário, uma lista de distribuição ou um recurso por um período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="51871-107">Represents the availability of a user, distribution list, or resource for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="51871-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51871-108">Properties</span></span>
| <span data-ttu-id="51871-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51871-109">Property</span></span>     | <span data-ttu-id="51871-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="51871-110">Type</span></span>   |<span data-ttu-id="51871-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="51871-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51871-112">availabilityView</span><span class="sxs-lookup"><span data-stu-id="51871-112">availabilityView</span></span> |<span data-ttu-id="51871-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51871-113">String</span></span> |<span data-ttu-id="51871-114">Representa um modo de exibição mesclado de disponibilidade de todos os itens em `scheduleItems`.</span><span class="sxs-lookup"><span data-stu-id="51871-114">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="51871-115">O modo de exibição consiste em intervalos de tempo.</span><span class="sxs-lookup"><span data-stu-id="51871-115">The view consists of time slots.</span></span> <span data-ttu-id="51871-116">Disponibilidade durante cada intervalo de tempo é indicada com: `0`= gratuito, `1`= provisório, `2`= ocupado, `3`= ausência temporária, `4`= trabalhando em outros lugares.</span><span class="sxs-lookup"><span data-stu-id="51871-116">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="51871-117">erro</span><span class="sxs-lookup"><span data-stu-id="51871-117">error</span></span> |[<span data-ttu-id="51871-118">freeBusyError</span><span class="sxs-lookup"><span data-stu-id="51871-118">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="51871-119">Informações de erro da tentativa de obter a disponibilidade do usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="51871-119">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="51871-120">scheduleId</span><span class="sxs-lookup"><span data-stu-id="51871-120">scheduleId</span></span> |<span data-ttu-id="51871-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51871-121">String</span></span> |<span data-ttu-id="51871-122">Um endereço SMTP do usuário, lista de distribuição ou recurso, que identifica uma instância de **scheduleInformation**.</span><span class="sxs-lookup"><span data-stu-id="51871-122">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="51871-123">scheduleItems</span><span class="sxs-lookup"><span data-stu-id="51871-123">scheduleItems</span></span> |<span data-ttu-id="51871-124">coleção [scheduleItem](scheduleitem.md)</span><span class="sxs-lookup"><span data-stu-id="51871-124">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="51871-125">Contém os itens que descrevem a disponibilidade do usuário ou recurso.</span><span class="sxs-lookup"><span data-stu-id="51871-125">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="51871-126">workingHours</span><span class="sxs-lookup"><span data-stu-id="51871-126">workingHours</span></span> |[<span data-ttu-id="51871-127">workingHours</span><span class="sxs-lookup"><span data-stu-id="51871-127">workingHours</span></span>](workinghours.md) |<span data-ttu-id="51871-128">Os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="51871-128">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="51871-129">Elas são definidas como parte do do usuário [mailboxSettings](mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="51871-129">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="51871-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51871-130">JSON representation</span></span>

<span data-ttu-id="51871-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51871-131">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
