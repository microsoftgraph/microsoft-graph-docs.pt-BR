# <a name="workinghours-resource-type"></a><span data-ttu-id="94977-101">Tipo de recurso workingHours</span><span class="sxs-lookup"><span data-stu-id="94977-101">workingHours resource type</span></span>

<span data-ttu-id="94977-102">Representa os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="94977-102">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="94977-103">Ter acesso ao horário de trabalho de um usuário é útil em cenários que lidam com o planejamento de atividades ou recursos.</span><span class="sxs-lookup"><span data-stu-id="94977-103">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="94977-104">Você pode [obter](../api/user_get_mailboxsettings.md#request-3) e [definir](../api/user_update_mailboxsettings.md#request-2) o horário de trabalho de um usuário como parte das [configurações da caixa de correio](mailboxSettings.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="94977-104">You can [get](../api/user_get_mailboxsettings.md#request-3) and [set](../api/user_update_mailboxsettings.md#request-2) the working hours of a user as part of the user's [mailbox settings](mailboxSettings.md).</span></span> 

<span data-ttu-id="94977-105">Você pode optar por definir um fuso horário para seu horário de trabalho de maneira diferente do fuso horário definido no seu cliente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="94977-105">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="94977-106">Isso pode ser útil em casos como quando você viaja para um fuso horário diferente daquele no qual você normalmente trabalha.</span><span class="sxs-lookup"><span data-stu-id="94977-106">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="94977-107">É possível configurar o cliente do Outlook</span><span class="sxs-lookup"><span data-stu-id="94977-107">You can set the Outlook client</span></span>  
<span data-ttu-id="94977-108">no fuso horário de destino para que os valores de tempo do Outlook sejam exibidos no horário local enquanto você estiver lá.</span><span class="sxs-lookup"><span data-stu-id="94977-108">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="94977-109">Quando outras pessoas solicitarem reuniões de trabalho com você no seu local habitual de trabalho, elas ainda poderão respeitar seu horário de trabalho no fuso horário apropriado.</span><span class="sxs-lookup"><span data-stu-id="94977-109">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="94977-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94977-110">Properties</span></span>
| <span data-ttu-id="94977-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94977-111">Property</span></span>     | <span data-ttu-id="94977-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="94977-112">Type</span></span>   |<span data-ttu-id="94977-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="94977-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="94977-114">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="94977-114">daysOfWeek</span></span> | <span data-ttu-id="94977-115">coleção dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="94977-115">dayOfWeek collection</span></span> | <span data-ttu-id="94977-116">Os dias da semana em que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="94977-116">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="94977-117">startTime</span><span class="sxs-lookup"><span data-stu-id="94977-117">startTime</span></span> | <span data-ttu-id="94977-118">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="94977-118">Edm.TimeOfDay</span></span> | <span data-ttu-id="94977-119">A hora do dia em que o usuário começa a trabalhar.</span><span class="sxs-lookup"><span data-stu-id="94977-119">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="94977-120">endTime</span><span class="sxs-lookup"><span data-stu-id="94977-120">endTime</span></span> | <span data-ttu-id="94977-121">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="94977-121">Edm.TimeOfDay</span></span> | <span data-ttu-id="94977-122">A hora do dia em que o usuário para de trabalhar.</span><span class="sxs-lookup"><span data-stu-id="94977-122">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="94977-123">timeZone</span><span class="sxs-lookup"><span data-stu-id="94977-123">timeZone</span></span> | [<span data-ttu-id="94977-124">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="94977-124">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="94977-125">O fuso horário ao qual o horário de trabalho se aplica.</span><span class="sxs-lookup"><span data-stu-id="94977-125">The time zone to which the working hours apply.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="94977-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94977-126">JSON representation</span></span>

<span data-ttu-id="94977-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94977-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "TimeOfDay",
  "endTime": "TimeOfDay",
  "timeZone": {"@odata.type": "microsoft.graph.timeZoneBase"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/workinghours.md/microsoft.graph.workingHours/daysOfWeek:
      Inconsistent types between parameter (String) and table (Object)"
  ],
  "tocPath": ""
}-->