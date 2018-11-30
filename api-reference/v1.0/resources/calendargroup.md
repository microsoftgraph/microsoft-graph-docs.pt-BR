---
title: Tipo de recurso calendarGroup
description: Um grupo de calendários do usuário.
ms.openlocfilehash: 6cc3ec5ed206109b341d0fc69845c9bd19df9373
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003476"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="fc112-103">Tipo de recurso calendarGroup</span><span class="sxs-lookup"><span data-stu-id="fc112-103">calendarGroup resource type</span></span>

<span data-ttu-id="fc112-104">Um grupo de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="fc112-104">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="fc112-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="fc112-105">Methods</span></span>

| <span data-ttu-id="fc112-106">Método</span><span class="sxs-lookup"><span data-stu-id="fc112-106">Method</span></span>                                                      | <span data-ttu-id="fc112-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fc112-107">Return Type</span></span>                        | <span data-ttu-id="fc112-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc112-108">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="fc112-109">List calendar groups</span><span class="sxs-lookup"><span data-stu-id="fc112-109">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="fc112-110">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="fc112-110">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="fc112-111">Obter os grupos de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="fc112-111">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="fc112-112">Create calendar group</span><span class="sxs-lookup"><span data-stu-id="fc112-112">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="fc112-113">Calendar</span><span class="sxs-lookup"><span data-stu-id="fc112-113">Calendar</span></span>](calendar.md)            | <span data-ttu-id="fc112-114">Criar um novo grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="fc112-114">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="fc112-115">Get calendar group</span><span class="sxs-lookup"><span data-stu-id="fc112-115">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="fc112-116">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="fc112-116">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="fc112-117">Leia as propriedades e os relacionamentos de um objeto de grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="fc112-117">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="fc112-118">Update</span><span class="sxs-lookup"><span data-stu-id="fc112-118">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="fc112-119">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="fc112-119">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="fc112-120">Atualize o objeto calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="fc112-120">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="fc112-121">Delete</span><span class="sxs-lookup"><span data-stu-id="fc112-121">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="fc112-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc112-122">None</span></span>                               | <span data-ttu-id="fc112-123">Exclua o objeto calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="fc112-123">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="fc112-124">List calendars</span><span class="sxs-lookup"><span data-stu-id="fc112-124">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="fc112-125">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="fc112-125">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="fc112-126">Liste os calendários em um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="fc112-126">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="fc112-127">Create Calendar</span><span class="sxs-lookup"><span data-stu-id="fc112-127">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="fc112-128">Calendar</span><span class="sxs-lookup"><span data-stu-id="fc112-128">Calendar</span></span>](calendar.md)            | <span data-ttu-id="fc112-129">Crie um novo calendário em um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="fc112-129">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="fc112-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc112-130">Properties</span></span>

| <span data-ttu-id="fc112-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc112-131">Property</span></span>  | <span data-ttu-id="fc112-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc112-132">Type</span></span>   | <span data-ttu-id="fc112-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc112-133">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="fc112-134">name</span><span class="sxs-lookup"><span data-stu-id="fc112-134">name</span></span>      | <span data-ttu-id="fc112-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc112-135">String</span></span> | <span data-ttu-id="fc112-136">O nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="fc112-136">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="fc112-137">changeKey</span><span class="sxs-lookup"><span data-stu-id="fc112-137">changeKey</span></span> | <span data-ttu-id="fc112-138">String</span><span class="sxs-lookup"><span data-stu-id="fc112-138">String</span></span> | <span data-ttu-id="fc112-p101">Identifica a versão do grupo de calendários. Toda vez que o grupo de calendários é alterado, ChangeKey também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fc112-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="fc112-143">classId</span><span class="sxs-lookup"><span data-stu-id="fc112-143">classId</span></span>   | <span data-ttu-id="fc112-144">Guid</span><span class="sxs-lookup"><span data-stu-id="fc112-144">Guid</span></span>   | <span data-ttu-id="fc112-p102">O identificador de classe. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fc112-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="fc112-147">id</span><span class="sxs-lookup"><span data-stu-id="fc112-147">id</span></span>        | <span data-ttu-id="fc112-148">String</span><span class="sxs-lookup"><span data-stu-id="fc112-148">String</span></span> | <span data-ttu-id="fc112-p103">O identificador exclusivo do grupo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fc112-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="fc112-151">Relações</span><span class="sxs-lookup"><span data-stu-id="fc112-151">Relationships</span></span>

| <span data-ttu-id="fc112-152">Relação</span><span class="sxs-lookup"><span data-stu-id="fc112-152">Relationship</span></span> | <span data-ttu-id="fc112-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc112-153">Type</span></span>                               | <span data-ttu-id="fc112-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc112-154">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="fc112-155">calendars</span><span class="sxs-lookup"><span data-stu-id="fc112-155">calendars</span></span>    | <span data-ttu-id="fc112-156">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="fc112-156">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="fc112-p104">Os calendários no grupo de calendários. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="fc112-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fc112-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc112-161">JSON representation</span></span>

<span data-ttu-id="fc112-162">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="fc112-162">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendarGroup",
  "@odata.annotations": [
    {
      "property": "calendars",
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
