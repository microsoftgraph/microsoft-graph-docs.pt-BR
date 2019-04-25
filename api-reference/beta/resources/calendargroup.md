---
title: Tipo de recurso calendarGroup
description: Um grupo de calendários do usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cea68da3a91396972c4e237d1fdaf0e16d65e3a3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543732"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="98715-103">Tipo de recurso calendarGroup</span><span class="sxs-lookup"><span data-stu-id="98715-103">calendarGroup resource type</span></span>

<span data-ttu-id="98715-104">Um grupo de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="98715-104">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="98715-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="98715-105">Methods</span></span>

| <span data-ttu-id="98715-106">Método</span><span class="sxs-lookup"><span data-stu-id="98715-106">Method</span></span>                                                      | <span data-ttu-id="98715-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="98715-107">Return Type</span></span>                        | <span data-ttu-id="98715-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="98715-108">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="98715-109">List calendar groups</span><span class="sxs-lookup"><span data-stu-id="98715-109">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="98715-110">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="98715-110">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="98715-111">Obter os grupos de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="98715-111">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="98715-112">Create calendar group</span><span class="sxs-lookup"><span data-stu-id="98715-112">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="98715-113">Calendar</span><span class="sxs-lookup"><span data-stu-id="98715-113">Calendar</span></span>](calendar.md)            | <span data-ttu-id="98715-114">Criar um novo grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="98715-114">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="98715-115">Get calendar group</span><span class="sxs-lookup"><span data-stu-id="98715-115">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="98715-116">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="98715-116">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="98715-117">Leia as propriedades e os relacionamentos de um objeto de grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="98715-117">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="98715-118">Update</span><span class="sxs-lookup"><span data-stu-id="98715-118">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="98715-119">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="98715-119">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="98715-120">Atualize o objeto calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="98715-120">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="98715-121">Excluir</span><span class="sxs-lookup"><span data-stu-id="98715-121">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="98715-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="98715-122">None</span></span>                               | <span data-ttu-id="98715-123">Exclua o objeto calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="98715-123">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="98715-124">Listar calendários</span><span class="sxs-lookup"><span data-stu-id="98715-124">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="98715-125">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="98715-125">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="98715-126">Liste os calendários em um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="98715-126">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="98715-127">Create Calendar</span><span class="sxs-lookup"><span data-stu-id="98715-127">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="98715-128">Calendar</span><span class="sxs-lookup"><span data-stu-id="98715-128">Calendar</span></span>](calendar.md)            | <span data-ttu-id="98715-129">Crie um novo calendário em um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="98715-129">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="98715-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="98715-130">Properties</span></span>

| <span data-ttu-id="98715-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98715-131">Property</span></span>  | <span data-ttu-id="98715-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="98715-132">Type</span></span>   | <span data-ttu-id="98715-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="98715-133">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="98715-134">name</span><span class="sxs-lookup"><span data-stu-id="98715-134">name</span></span>      | <span data-ttu-id="98715-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98715-135">String</span></span> | <span data-ttu-id="98715-136">O nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="98715-136">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="98715-137">changeKey</span><span class="sxs-lookup"><span data-stu-id="98715-137">changeKey</span></span> | <span data-ttu-id="98715-138">String</span><span class="sxs-lookup"><span data-stu-id="98715-138">String</span></span> | <span data-ttu-id="98715-p101">Identifica a versão do grupo de calendários. Toda vez que o grupo de calendários é alterado, ChangeKey também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="98715-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="98715-143">classId</span><span class="sxs-lookup"><span data-stu-id="98715-143">classId</span></span>   | <span data-ttu-id="98715-144">Guid</span><span class="sxs-lookup"><span data-stu-id="98715-144">Guid</span></span>   | <span data-ttu-id="98715-p102">O identificador de classe. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="98715-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="98715-147">id</span><span class="sxs-lookup"><span data-stu-id="98715-147">id</span></span>        | <span data-ttu-id="98715-148">String</span><span class="sxs-lookup"><span data-stu-id="98715-148">String</span></span> | <span data-ttu-id="98715-p103">O identificador exclusivo do grupo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="98715-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="98715-151">Relações</span><span class="sxs-lookup"><span data-stu-id="98715-151">Relationships</span></span>

| <span data-ttu-id="98715-152">Relação</span><span class="sxs-lookup"><span data-stu-id="98715-152">Relationship</span></span> | <span data-ttu-id="98715-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="98715-153">Type</span></span>                               | <span data-ttu-id="98715-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="98715-154">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="98715-155">calendars</span><span class="sxs-lookup"><span data-stu-id="98715-155">calendars</span></span>    | <span data-ttu-id="98715-156">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="98715-156">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="98715-p104">Os calendários no grupo de calendários. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="98715-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="98715-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="98715-161">JSON representation</span></span>

<span data-ttu-id="98715-162">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="98715-162">Here is a JSON representation of the resource</span></span>

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
