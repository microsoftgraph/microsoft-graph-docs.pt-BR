# <a name="calendargroup-resource-type"></a><span data-ttu-id="29dd5-101">Tipo de recurso calendarGroup</span><span class="sxs-lookup"><span data-stu-id="29dd5-101">calendarGroup resource type</span></span>

<span data-ttu-id="29dd5-102">Um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="29dd5-102">A group of calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="29dd5-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="29dd5-103">Methods</span></span>

| <span data-ttu-id="29dd5-104">Método</span><span class="sxs-lookup"><span data-stu-id="29dd5-104">Method</span></span>                                                      | <span data-ttu-id="29dd5-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="29dd5-105">Return Type</span></span>                        | <span data-ttu-id="29dd5-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="29dd5-106">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="29dd5-107">List calendar groups</span><span class="sxs-lookup"><span data-stu-id="29dd5-107">List calendar groups</span></span>](../api/user_list_calendargroups.md)  | <span data-ttu-id="29dd5-108">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="29dd5-108">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="29dd5-109">Obter os grupos de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="29dd5-109">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="29dd5-110">Create calendar group</span><span class="sxs-lookup"><span data-stu-id="29dd5-110">Create calendar group</span></span>](../api/user_post_calendargroups.md) | [<span data-ttu-id="29dd5-111">Calendar</span><span class="sxs-lookup"><span data-stu-id="29dd5-111">Calendar</span></span>](calendar.md)            | <span data-ttu-id="29dd5-112">Criar um novo grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="29dd5-112">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="29dd5-113">Get calendar group</span><span class="sxs-lookup"><span data-stu-id="29dd5-113">Get calendar group</span></span>](../api/calendargroup_get.md)           | [<span data-ttu-id="29dd5-114">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="29dd5-114">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="29dd5-115">Leia as propriedades e os relacionamentos de um objeto de grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="29dd5-115">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="29dd5-116">Update</span><span class="sxs-lookup"><span data-stu-id="29dd5-116">Update</span></span>](../api/calendargroup_update.md)                    | [<span data-ttu-id="29dd5-117">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="29dd5-117">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="29dd5-118">Atualize o objeto calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="29dd5-118">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="29dd5-119">Delete</span><span class="sxs-lookup"><span data-stu-id="29dd5-119">Delete</span></span>](../api/calendargroup_delete.md)                    | <span data-ttu-id="29dd5-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="29dd5-120">None</span></span>                               | <span data-ttu-id="29dd5-121">Exclua o objeto calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="29dd5-121">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="29dd5-122">List calendars</span><span class="sxs-lookup"><span data-stu-id="29dd5-122">List calendars</span></span>](../api/calendargroup_list_calendars.md)    | <span data-ttu-id="29dd5-123">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="29dd5-123">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="29dd5-124">Liste os calendários em um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="29dd5-124">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="29dd5-125">Create Calendar</span><span class="sxs-lookup"><span data-stu-id="29dd5-125">Create Calendar</span></span>](../api/calendargroup_post_calendars.md)   | [<span data-ttu-id="29dd5-126">Calendar</span><span class="sxs-lookup"><span data-stu-id="29dd5-126">Calendar</span></span>](calendar.md)            | <span data-ttu-id="29dd5-127">Crie um novo calendário em um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="29dd5-127">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="29dd5-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29dd5-128">Properties</span></span>

| <span data-ttu-id="29dd5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29dd5-129">Property</span></span>  | <span data-ttu-id="29dd5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="29dd5-130">Type</span></span>   | <span data-ttu-id="29dd5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="29dd5-131">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="29dd5-132">name</span><span class="sxs-lookup"><span data-stu-id="29dd5-132">name</span></span>      | <span data-ttu-id="29dd5-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29dd5-133">String</span></span> | <span data-ttu-id="29dd5-134">O nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="29dd5-134">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="29dd5-135">changeKey</span><span class="sxs-lookup"><span data-stu-id="29dd5-135">changeKey</span></span> | <span data-ttu-id="29dd5-136">String</span><span class="sxs-lookup"><span data-stu-id="29dd5-136">String</span></span> | <span data-ttu-id="29dd5-p101">Identifica a versão do grupo de calendários. Toda vez que o grupo de calendários é alterado, ChangeKey também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29dd5-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="29dd5-141">classId</span><span class="sxs-lookup"><span data-stu-id="29dd5-141">classId</span></span>   | <span data-ttu-id="29dd5-142">Guid</span><span class="sxs-lookup"><span data-stu-id="29dd5-142">Guid</span></span>   | <span data-ttu-id="29dd5-p102">O identificador de classe. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29dd5-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="29dd5-145">id</span><span class="sxs-lookup"><span data-stu-id="29dd5-145">id</span></span>        | <span data-ttu-id="29dd5-146">String</span><span class="sxs-lookup"><span data-stu-id="29dd5-146">String</span></span> | <span data-ttu-id="29dd5-p103">O identificador exclusivo do grupo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29dd5-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="29dd5-149">Relações</span><span class="sxs-lookup"><span data-stu-id="29dd5-149">Relationships</span></span>

| <span data-ttu-id="29dd5-150">Relação</span><span class="sxs-lookup"><span data-stu-id="29dd5-150">Relationship</span></span> | <span data-ttu-id="29dd5-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="29dd5-151">Type</span></span>                               | <span data-ttu-id="29dd5-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="29dd5-152">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="29dd5-153">calendars</span><span class="sxs-lookup"><span data-stu-id="29dd5-153">calendars</span></span>    | <span data-ttu-id="29dd5-154">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="29dd5-154">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="29dd5-p104">Os calendários no grupo de calendários. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="29dd5-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="29dd5-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29dd5-159">JSON representation</span></span>

<span data-ttu-id="29dd5-160">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="29dd5-160">Here is a JSON representation of the resource</span></span>

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
