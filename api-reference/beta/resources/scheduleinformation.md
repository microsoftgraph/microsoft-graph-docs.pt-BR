---
title: tipo de recurso de scheduleInformation
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: e84505ee2f30a5b7b52e9d5b589b8bb24d9a4c95
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521905"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="c80d9-104">tipo de recurso de scheduleInformation</span><span class="sxs-lookup"><span data-stu-id="c80d9-104">scheduleInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="c80d9-105">Representa a disponibilidade de um usuário, uma lista de distribuição ou um recurso por um período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="c80d9-105">Represents the availability of a user, distribution list, or resource for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="c80d9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c80d9-106">Properties</span></span>
| <span data-ttu-id="c80d9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c80d9-107">Property</span></span>     | <span data-ttu-id="c80d9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c80d9-108">Type</span></span>   |<span data-ttu-id="c80d9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c80d9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c80d9-110">availabilityView</span><span class="sxs-lookup"><span data-stu-id="c80d9-110">availabilityView</span></span> |<span data-ttu-id="c80d9-111">String</span><span class="sxs-lookup"><span data-stu-id="c80d9-111">String</span></span> |<span data-ttu-id="c80d9-112">Representa um modo de exibição mesclado de disponibilidade de todos os itens em `scheduleItems`.</span><span class="sxs-lookup"><span data-stu-id="c80d9-112">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="c80d9-113">O modo de exibição consiste em intervalos de tempo.</span><span class="sxs-lookup"><span data-stu-id="c80d9-113">The view consists of time slots.</span></span> <span data-ttu-id="c80d9-114">Disponibilidade durante cada intervalo de tempo é indicada com: `0`= gratuito, `1`= provisório, `2`= ocupado, `3`= ausência temporária, `4`= trabalhando em outros lugares.</span><span class="sxs-lookup"><span data-stu-id="c80d9-114">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="c80d9-115">erro</span><span class="sxs-lookup"><span data-stu-id="c80d9-115">error</span></span> |[<span data-ttu-id="c80d9-116">freeBusyError</span><span class="sxs-lookup"><span data-stu-id="c80d9-116">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="c80d9-117">Informações de erro da tentativa de obter a disponibilidade do usuário, lista de distribuição ou recurso.</span><span class="sxs-lookup"><span data-stu-id="c80d9-117">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="c80d9-118">scheduleId</span><span class="sxs-lookup"><span data-stu-id="c80d9-118">scheduleId</span></span> |<span data-ttu-id="c80d9-119">String</span><span class="sxs-lookup"><span data-stu-id="c80d9-119">String</span></span> |<span data-ttu-id="c80d9-120">Um endereço SMTP do usuário, lista de distribuição ou recurso, que identifica uma instância de **scheduleInformation**.</span><span class="sxs-lookup"><span data-stu-id="c80d9-120">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="c80d9-121">scheduleItems</span><span class="sxs-lookup"><span data-stu-id="c80d9-121">scheduleItems</span></span> |<span data-ttu-id="c80d9-122">coleção [scheduleItem](scheduleitem.md)</span><span class="sxs-lookup"><span data-stu-id="c80d9-122">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="c80d9-123">Contém os itens que descrevem a disponibilidade do usuário ou recurso.</span><span class="sxs-lookup"><span data-stu-id="c80d9-123">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="c80d9-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="c80d9-124">workingHours</span></span> |[<span data-ttu-id="c80d9-125">workingHours</span><span class="sxs-lookup"><span data-stu-id="c80d9-125">workingHours</span></span>](workinghours.md) |<span data-ttu-id="c80d9-126">Os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="c80d9-126">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="c80d9-127">Elas são definidas como parte do do usuário [mailboxSettings](mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="c80d9-127">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c80d9-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c80d9-128">JSON representation</span></span>

<span data-ttu-id="c80d9-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c80d9-129">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
