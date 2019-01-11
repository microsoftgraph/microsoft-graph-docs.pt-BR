---
title: tipo de recurso calendar
description: Um calendário que é um contêiner para eventos. Pode ser um calendário para um user ou o calendário padrão de um group do Office 365.
localization_priority: Priority
ms.openlocfilehash: c567a37be651987f2ca5af08cf9837ba6f41076f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843243"
---
# <a name="calendar-resource-type"></a><span data-ttu-id="e457a-104">tipo de recurso calendar</span><span class="sxs-lookup"><span data-stu-id="e457a-104">calendar resource type</span></span>

<span data-ttu-id="e457a-105">Um calendário que é um contêiner para eventos.</span><span class="sxs-lookup"><span data-stu-id="e457a-105">A calendar which is a container for events.</span></span> <span data-ttu-id="e457a-106">Pode ser um calendário para um [user](user.md) ou o calendário padrão de um [group](group.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="e457a-106">It can be a calendar for a [user](user.md), or the default calendar of an Office 365 [group](group.md).</span></span>

> <span data-ttu-id="e457a-107">**Observação:** Existem algumas pequenas diferenças da maneira que você pode interagir com calendários do usuário e calendários de grupo:</span><span class="sxs-lookup"><span data-stu-id="e457a-107">**Note:** There are a few minor differences in the way you can interact with user calendars and group calendars:</span></span>

 - <span data-ttu-id="e457a-108">Você pode organizar somente os calendários de usuário em um [calendarGroup](calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="e457a-108">You can organize only user calendars in a [calendarGroup](calendargroup.md).</span></span>
 - <span data-ttu-id="e457a-109">Outlook automaticamente aceita todas as solicitações de reunião em nome de grupos.</span><span class="sxs-lookup"><span data-stu-id="e457a-109">Outlook automatically accepts all meeting requests on behalf of groups.</span></span> <span data-ttu-id="e457a-110">Você pode [Aceitar](../api/event-accept.md), [Aceitar provisoriamente](../api/event-tentativelyaccept.md)ou [Recusar](../api/event-decline.md) solicitações de reunião para apenas calendários de usuário.</span><span class="sxs-lookup"><span data-stu-id="e457a-110">You can [accept](../api/event-accept.md), [tentatively accept](../api/event-tentativelyaccept.md), or [decline](../api/event-decline.md)  meeting requests for user calendars only.</span></span>
  - <span data-ttu-id="e457a-111">O Outlook não oferece suporte a lembretes para eventos de grupo.</span><span class="sxs-lookup"><span data-stu-id="e457a-111">Outlook doesn't support reminders for group events.</span></span> <span data-ttu-id="e457a-112">É possível [Adiar](../api/event-snoozereminder.md) ou [Descartar](../api/event-dismissreminder.md) um [lembrete](reminder.md) para apenas calendários de usuário.</span><span class="sxs-lookup"><span data-stu-id="e457a-112">You can [snooze](../api/event-snoozereminder.md) or [dismiss](../api/event-dismissreminder.md) a [reminder](reminder.md) for user calendars only.</span></span>

## <a name="methods"></a><span data-ttu-id="e457a-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="e457a-113">Methods</span></span>

| <span data-ttu-id="e457a-114">Método</span><span class="sxs-lookup"><span data-stu-id="e457a-114">Method</span></span>       | <span data-ttu-id="e457a-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e457a-115">Return Type</span></span>  |<span data-ttu-id="e457a-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="e457a-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e457a-117">Listar calendários</span><span class="sxs-lookup"><span data-stu-id="e457a-117">List calendars</span></span>](../api/user-list-calendars.md)|<span data-ttu-id="e457a-118">Coleção [calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="e457a-118">[calendar](calendar.md) collection</span></span>|<span data-ttu-id="e457a-119">Obtenha todos os calendários do usuário ou os calendários no grupo de calendários padrão ou em outro grupo de calendários específico.</span><span class="sxs-lookup"><span data-stu-id="e457a-119">Get all the user's calendars, or the calendars in the default or other specific calendar group.</span></span>|
|[<span data-ttu-id="e457a-120">Criar calendário</span><span class="sxs-lookup"><span data-stu-id="e457a-120">Create calendar</span></span>](../api/user-post-calendars.md) |[<span data-ttu-id="e457a-121">calendar</span><span class="sxs-lookup"><span data-stu-id="e457a-121">calendar</span></span>](calendar.md)| <span data-ttu-id="e457a-122">Crie um novo calendário no grupo de calendário padrão ou no grupo de calendários especificado para um usuário.</span><span class="sxs-lookup"><span data-stu-id="e457a-122">Create a new calendar in the default calendar group or specified calendar group for a user.</span></span>|
|[<span data-ttu-id="e457a-123">Obter calendário</span><span class="sxs-lookup"><span data-stu-id="e457a-123">Get calendar</span></span>](../api/calendar-get.md) | [<span data-ttu-id="e457a-124">calendar</span><span class="sxs-lookup"><span data-stu-id="e457a-124">calendar</span></span>](calendar.md) |<span data-ttu-id="e457a-125">Obtenha as propriedades e as relações de um objeto **calendar**.</span><span class="sxs-lookup"><span data-stu-id="e457a-125">Get the properties and relationships of a **calendar** object.</span></span> <span data-ttu-id="e457a-126">O calendário pode ser um para um usuário ou o calendário padrão de um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="e457a-126">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="e457a-127">Atualizar</span><span class="sxs-lookup"><span data-stu-id="e457a-127">Update</span></span>](../api/calendar-update.md) | [<span data-ttu-id="e457a-128">calendar</span><span class="sxs-lookup"><span data-stu-id="e457a-128">calendar</span></span>](calendar.md)  |<span data-ttu-id="e457a-129">Atualize as propriedades de um objeto **calendar**.</span><span class="sxs-lookup"><span data-stu-id="e457a-129">Update the properties of a **calendar** object.</span></span> <span data-ttu-id="e457a-130">O calendário pode ser um para um usuário ou o calendário padrão de um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="e457a-130">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="e457a-131">Excluir</span><span class="sxs-lookup"><span data-stu-id="e457a-131">Delete</span></span>](../api/calendar-delete.md) | <span data-ttu-id="e457a-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e457a-132">None</span></span> |<span data-ttu-id="e457a-133">Exclua um objeto calendar.</span><span class="sxs-lookup"><span data-stu-id="e457a-133">Delete calendar object.</span></span> |
|[<span data-ttu-id="e457a-134">Listar calendarView</span><span class="sxs-lookup"><span data-stu-id="e457a-134">List calendarView</span></span>](../api/calendar-list-calendarview.md) |<span data-ttu-id="e457a-135">Coleção [event](event.md)</span><span class="sxs-lookup"><span data-stu-id="e457a-135">[event](event.md) collection</span></span>| <span data-ttu-id="e457a-136">Obtenha as ocorrências, as exceções e as instâncias de eventos únicas em uma visão de calendário definida por um intervalo de tempo, do calendário principal do usuário `(../me/calendarview)` ou de um calendário especificado.</span><span class="sxs-lookup"><span data-stu-id="e457a-136">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's primary calendar `(../me/calendarview)` or from a specified calendar.</span></span>|
|[<span data-ttu-id="e457a-137">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="e457a-137">List events</span></span>](../api/calendar-list-events.md) |<span data-ttu-id="e457a-138">Coleção [event](event.md)</span><span class="sxs-lookup"><span data-stu-id="e457a-138">[event](event.md) collection</span></span>| <span data-ttu-id="e457a-p107">Recupera uma lista de eventos em um calendário.  A lista contém reuniões de instância única e reuniões mestres da série.</span><span class="sxs-lookup"><span data-stu-id="e457a-p107">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="e457a-141">Criar evento</span><span class="sxs-lookup"><span data-stu-id="e457a-141">Create event</span></span>](../api/calendar-post-events.md) |[<span data-ttu-id="e457a-142">event</span><span class="sxs-lookup"><span data-stu-id="e457a-142">event</span></span>](event.md)| <span data-ttu-id="e457a-143">Crie um novo evento no padrão ou calendário especificado.</span><span class="sxs-lookup"><span data-stu-id="e457a-143">Create a new event in the default or specified calendar.</span></span>|
|[<span data-ttu-id="e457a-144">findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="e457a-144">findMeetingTimes</span></span>](../api/user-findmeetingtimes.md) |[<span data-ttu-id="e457a-145">meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="e457a-145">meetingTimeSuggestionsResult</span></span>](meetingtimesuggestionsresult.md) |<span data-ttu-id="e457a-146">Sugerir horários de reunião e locais com base na disponibilidade do organizador e participante e restrições de tempo ou local.</span><span class="sxs-lookup"><span data-stu-id="e457a-146">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints.</span></span> |
|[<span data-ttu-id="e457a-147">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="e457a-147">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="e457a-148">calendar</span><span class="sxs-lookup"><span data-stu-id="e457a-148">calendar</span></span>](calendar.md)  |<span data-ttu-id="e457a-149">Criar uma ou mais propriedades estendidas de valor único em um calendário novo ou existente.</span><span class="sxs-lookup"><span data-stu-id="e457a-149">Create one or more single-value extended properties in a new or existing calendar.</span></span>   |
|[<span data-ttu-id="e457a-150">Obter calendário com propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="e457a-150">Get calendar with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="e457a-151">calendar</span><span class="sxs-lookup"><span data-stu-id="e457a-151">calendar</span></span>](calendar.md) | <span data-ttu-id="e457a-152">Obter calendários que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="e457a-152">Get calendars that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="e457a-153">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="e457a-153">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="e457a-154">calendar</span><span class="sxs-lookup"><span data-stu-id="e457a-154">calendar</span></span>](calendar.md) | <span data-ttu-id="e457a-155">Criar uma ou mais propriedades estendidas de vários valores em um calendário novo ou existente.</span><span class="sxs-lookup"><span data-stu-id="e457a-155">Create one or more multi-value extended properties in a new or existing calendar.</span></span>  |
|[<span data-ttu-id="e457a-156">Obter calendário com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="e457a-156">Get calendar with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="e457a-157">calendar</span><span class="sxs-lookup"><span data-stu-id="e457a-157">calendar</span></span>](calendar.md) | <span data-ttu-id="e457a-158">Obter um calendário que contenha uma propriedade estendida de vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="e457a-158">Get a calendar that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="e457a-159">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e457a-159">Properties</span></span>
| <span data-ttu-id="e457a-160">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e457a-160">Property</span></span>     | <span data-ttu-id="e457a-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="e457a-161">Type</span></span>   |<span data-ttu-id="e457a-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="e457a-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e457a-163">canEdit</span><span class="sxs-lookup"><span data-stu-id="e457a-163">canEdit</span></span> |<span data-ttu-id="e457a-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="e457a-164">Boolean</span></span> |<span data-ttu-id="e457a-p108">Verdadeira se o usuário pode gravar o calendário, falsa caso contrário. Essa propriedade é verdadeira para o usuário que criou o calendário. Esta propriedade também é verdadeira para um usuário com o qual tenha sido compartilhado um calendário e tenha sido concedido acesso de gravação.</span><span class="sxs-lookup"><span data-stu-id="e457a-p108">True if the user can write to the calendar, false otherwise. This property is true for the user who created the calendar. This property is also true for a user who has been shared a calendar and granted write access.</span></span> |
|<span data-ttu-id="e457a-168">canShare</span><span class="sxs-lookup"><span data-stu-id="e457a-168">canShare</span></span> |<span data-ttu-id="e457a-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="e457a-169">Boolean</span></span> |<span data-ttu-id="e457a-p109">Verdadeira se o usuário tem permissão para compartilhar o calendário, falsa caso contrário. Somente o usuário que criou o calendário pode compartilhá-lo.</span><span class="sxs-lookup"><span data-stu-id="e457a-p109">True if the user has the permission to share the calendar, false otherwise. Only the user who created the calendar can share it.</span></span> |
|<span data-ttu-id="e457a-172">canViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="e457a-172">canViewPrivateItems</span></span> |<span data-ttu-id="e457a-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="e457a-173">Boolean</span></span> |<span data-ttu-id="e457a-174">Verdadeira se o usuário pode ler itens do calendário que foram marcados como particulares, falsa caso contrário.</span><span class="sxs-lookup"><span data-stu-id="e457a-174">True if the user can read calendar items that have been marked private, false otherwise.</span></span> |
|<span data-ttu-id="e457a-175">changeKey</span><span class="sxs-lookup"><span data-stu-id="e457a-175">changeKey</span></span>|<span data-ttu-id="e457a-176">String</span><span class="sxs-lookup"><span data-stu-id="e457a-176">String</span></span>|<span data-ttu-id="e457a-p110">Identifica a versão do objeto calendar. Toda vez que o calendário é alterado, a changeKey também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e457a-p110">Identifies the version of the calendar object. Every time the calendar is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span>|
|<span data-ttu-id="e457a-181">color</span><span class="sxs-lookup"><span data-stu-id="e457a-181">color</span></span>|<span data-ttu-id="e457a-182">calendarColor</span><span class="sxs-lookup"><span data-stu-id="e457a-182">calendarColor</span></span>|<span data-ttu-id="e457a-p111">Especifica o tema de cores para distinguir o calendário de outros calendários em uma interface do usuário. Os valores de propriedade são: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="e457a-p111">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="e457a-185">id</span><span class="sxs-lookup"><span data-stu-id="e457a-185">id</span></span>|<span data-ttu-id="e457a-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e457a-186">String</span></span>|<span data-ttu-id="e457a-p112">O identificador exclusivo do grupo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e457a-p112">The group's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="e457a-189">name</span><span class="sxs-lookup"><span data-stu-id="e457a-189">name</span></span>|<span data-ttu-id="e457a-190">String</span><span class="sxs-lookup"><span data-stu-id="e457a-190">String</span></span>|<span data-ttu-id="e457a-191">O nome do calendário.</span><span class="sxs-lookup"><span data-stu-id="e457a-191">The calendar name.</span></span>|
|<span data-ttu-id="e457a-192">owner</span><span class="sxs-lookup"><span data-stu-id="e457a-192">owner</span></span> |[<span data-ttu-id="e457a-193">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e457a-193">emailAddress</span></span>](emailaddress.md) | <span data-ttu-id="e457a-p113">Se definida, representa o usuário que criou ou adicionou o calendário. Para um calendário que o usuário criou ou adicionou, a propriedade **owner** é definida para o usuário. Para um calendário compartilhado com o usuário, a propriedade **owner** é definida para a pessoa que compartilhou o calendário com o usuário.</span><span class="sxs-lookup"><span data-stu-id="e457a-p113">If set, this represents the user who created or added the calendar. For a calendar that the user created or added, the **owner** property is set to the user. For a calendar shared with the user, the **owner** property is set to the person who shared that calendar with the user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e457a-197">Relações</span><span class="sxs-lookup"><span data-stu-id="e457a-197">Relationships</span></span>
| <span data-ttu-id="e457a-198">Relação</span><span class="sxs-lookup"><span data-stu-id="e457a-198">Relationship</span></span> | <span data-ttu-id="e457a-199">Tipo</span><span class="sxs-lookup"><span data-stu-id="e457a-199">Type</span></span>   |<span data-ttu-id="e457a-200">Descrição</span><span class="sxs-lookup"><span data-stu-id="e457a-200">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e457a-201">calendarView</span><span class="sxs-lookup"><span data-stu-id="e457a-201">calendarView</span></span>|<span data-ttu-id="e457a-202">Coleção [Event](event.md)</span><span class="sxs-lookup"><span data-stu-id="e457a-202">[Event](event.md) collection</span></span>|<span data-ttu-id="e457a-p114">O modo de exibição do calendário. Propriedade de navegação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e457a-p114">The calendar view for the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="e457a-206">events</span><span class="sxs-lookup"><span data-stu-id="e457a-206">events</span></span>|<span data-ttu-id="e457a-207">Coleção [Event](event.md)</span><span class="sxs-lookup"><span data-stu-id="e457a-207">[Event](event.md) collection</span></span>|<span data-ttu-id="e457a-p115">Os eventos do calendário. Propriedade de navegação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e457a-p115">The events in the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="e457a-211">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="e457a-211">multiValueExtendedProperties</span></span>|<span data-ttu-id="e457a-212">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="e457a-212">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="e457a-p116">A coleção de propriedades estendidas de vários valores definidas para o calendário. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="e457a-p116">The collection of multi-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e457a-216">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="e457a-216">singleValueExtendedProperties</span></span>|<span data-ttu-id="e457a-217">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="e457a-217">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="e457a-p117">A coleção de propriedades estendidas de vários valores definidas para a mensagem. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="e457a-p117">The collection of single-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e457a-221">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e457a-221">JSON representation</span></span>

<span data-ttu-id="e457a-222">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e457a-222">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendar",
  "@odata.annotations": [
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "id": "string (identifier)",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
