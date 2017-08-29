# <a name="calendargroup-resource-type"></a><span data-ttu-id="86fe7-101">Tipo de recurso calendarGroup</span><span class="sxs-lookup"><span data-stu-id="86fe7-101">calendarGroup resource type</span></span>

<span data-ttu-id="86fe7-102">Um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="86fe7-102">A group of calendars.</span></span>

<span data-ttu-id="86fe7-p101">**Observação** O Outlook.com oferece suporte somente para o grupo de calendário padrão que pode ser acessado pelo atalho ../me/calendars. Você não pode excluir esse grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="86fe7-p101">**Note** Outlook.com supports only the default calendar group which is accessible by the ../me/calendars shortcut. You cannot delete that calendar group.</span></span>

## <a name="methods"></a><span data-ttu-id="86fe7-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="86fe7-105">Methods</span></span>

| <span data-ttu-id="86fe7-106">Método</span><span class="sxs-lookup"><span data-stu-id="86fe7-106">Method</span></span>       | <span data-ttu-id="86fe7-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="86fe7-107">Return Type</span></span>  |<span data-ttu-id="86fe7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="86fe7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="86fe7-109">List calendar groups</span><span class="sxs-lookup"><span data-stu-id="86fe7-109">List calendar groups</span></span>](../api/user_list_calendargroups.md) |<span data-ttu-id="86fe7-110">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="86fe7-110">[Calendar](calendar.md) collection</span></span>| <span data-ttu-id="86fe7-111">Obter os grupos de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="86fe7-111">Get the user's calendar groups.</span></span>|
|[<span data-ttu-id="86fe7-112">Create calendar group</span><span class="sxs-lookup"><span data-stu-id="86fe7-112">Create calendar group</span></span>](../api/user_post_calendargroups.md) |[<span data-ttu-id="86fe7-113">Calendar</span><span class="sxs-lookup"><span data-stu-id="86fe7-113">Calendar</span></span>](calendar.md)| <span data-ttu-id="86fe7-114">Criar um novo grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="86fe7-114">Create a new calendar group.</span></span>|
|[<span data-ttu-id="86fe7-115">Get calendar group</span><span class="sxs-lookup"><span data-stu-id="86fe7-115">Get calendar group</span></span>](../api/calendargroup_get.md) | [<span data-ttu-id="86fe7-116">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="86fe7-116">calendarGroup</span></span>](calendargroup.md) |<span data-ttu-id="86fe7-117">Leia as propriedades e os relacionamentos de um objeto de grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="86fe7-117">Read properties and relationships of a calendar group object.</span></span>|
|[<span data-ttu-id="86fe7-118">Update</span><span class="sxs-lookup"><span data-stu-id="86fe7-118">Update</span></span>](../api/calendargroup_update.md) | [<span data-ttu-id="86fe7-119">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="86fe7-119">calendarGroup</span></span>](calendargroup.md) |<span data-ttu-id="86fe7-120">Atualize o objeto calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="86fe7-120">Update calendarGroup object.</span></span> |
|[<span data-ttu-id="86fe7-121">Delete</span><span class="sxs-lookup"><span data-stu-id="86fe7-121">Delete</span></span>](../api/calendargroup_delete.md) | <span data-ttu-id="86fe7-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="86fe7-122">None</span></span> |<span data-ttu-id="86fe7-123">Exclua o objeto calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="86fe7-123">Delete calendarGroup object.</span></span> |
|[<span data-ttu-id="86fe7-124">List calendars</span><span class="sxs-lookup"><span data-stu-id="86fe7-124">List calendars</span></span>](../api/calendargroup_list_calendars.md) |<span data-ttu-id="86fe7-125">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="86fe7-125">[Calendar](calendar.md) collection</span></span>| <span data-ttu-id="86fe7-126">Liste os calendários em um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="86fe7-126">List calendars in a calendar group.</span></span>|
|[<span data-ttu-id="86fe7-127">Create Calendar</span><span class="sxs-lookup"><span data-stu-id="86fe7-127">Create Calendar</span></span>](../api/calendargroup_post_calendars.md) |[<span data-ttu-id="86fe7-128">Calendar</span><span class="sxs-lookup"><span data-stu-id="86fe7-128">Calendar</span></span>](calendar.md)| <span data-ttu-id="86fe7-129">Crie um novo calendário em um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="86fe7-129">Create a new Calendar in a calendar group.</span></span>|

## <a name="properties"></a><span data-ttu-id="86fe7-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86fe7-130">Properties</span></span>
| <span data-ttu-id="86fe7-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86fe7-131">Property</span></span>     | <span data-ttu-id="86fe7-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="86fe7-132">Type</span></span>   |<span data-ttu-id="86fe7-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="86fe7-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86fe7-134">name</span><span class="sxs-lookup"><span data-stu-id="86fe7-134">name</span></span>|<span data-ttu-id="86fe7-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86fe7-135">String</span></span>|<span data-ttu-id="86fe7-136">O nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="86fe7-136">The group name.</span></span>|
|<span data-ttu-id="86fe7-137">changeKey</span><span class="sxs-lookup"><span data-stu-id="86fe7-137">changeKey</span></span>|<span data-ttu-id="86fe7-138">String</span><span class="sxs-lookup"><span data-stu-id="86fe7-138">String</span></span>|<span data-ttu-id="86fe7-p102">Identifica a versão do grupo de calendários. Toda vez que o grupo de calendários é alterado, ChangeKey também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="86fe7-p102">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span>|
|<span data-ttu-id="86fe7-143">classId</span><span class="sxs-lookup"><span data-stu-id="86fe7-143">classId</span></span>|<span data-ttu-id="86fe7-144">Guid</span><span class="sxs-lookup"><span data-stu-id="86fe7-144">Guid</span></span>|<span data-ttu-id="86fe7-p103">O identificador de classe. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="86fe7-p103">The class identifier. Read-only.</span></span>|
|<span data-ttu-id="86fe7-147">id</span><span class="sxs-lookup"><span data-stu-id="86fe7-147">id</span></span>|<span data-ttu-id="86fe7-148">String</span><span class="sxs-lookup"><span data-stu-id="86fe7-148">String</span></span>|<span data-ttu-id="86fe7-p104">O identificador exclusivo do grupo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="86fe7-p104">The group's unique identifier. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86fe7-151">Relações</span><span class="sxs-lookup"><span data-stu-id="86fe7-151">Relationships</span></span>
| <span data-ttu-id="86fe7-152">Relação</span><span class="sxs-lookup"><span data-stu-id="86fe7-152">Relationship</span></span> | <span data-ttu-id="86fe7-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="86fe7-153">Type</span></span>   |<span data-ttu-id="86fe7-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="86fe7-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86fe7-155">calendars</span><span class="sxs-lookup"><span data-stu-id="86fe7-155">calendars</span></span>|<span data-ttu-id="86fe7-156">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="86fe7-156">[Calendar](calendar.md) collection</span></span>|<span data-ttu-id="86fe7-p105">Os calendários no grupo de calendários. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="86fe7-p105">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86fe7-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86fe7-161">JSON representation</span></span>

<span data-ttu-id="86fe7-162">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="86fe7-162">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendarGroup"
}-->

```json
{
  "changeKey": "string",
  "classId": "guid",
  "id": "string (identifier)",
  "name": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
