---
title: Tipo de recurso calendarGroup
description: Um grupo de calendários do usuário.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a630d35f5527494ce4cf477219dfd1f22547c490
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471493"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="64f7c-103">Tipo de recurso calendarGroup</span><span class="sxs-lookup"><span data-stu-id="64f7c-103">calendarGroup resource type</span></span>

<span data-ttu-id="64f7c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64f7c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64f7c-105">Um grupo de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="64f7c-105">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="64f7c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="64f7c-106">Methods</span></span>

| <span data-ttu-id="64f7c-107">Método</span><span class="sxs-lookup"><span data-stu-id="64f7c-107">Method</span></span>                                                      | <span data-ttu-id="64f7c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="64f7c-108">Return Type</span></span>                        | <span data-ttu-id="64f7c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="64f7c-109">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="64f7c-110">List calendar groups</span><span class="sxs-lookup"><span data-stu-id="64f7c-110">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="64f7c-111">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="64f7c-111">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="64f7c-112">Obter os grupos de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="64f7c-112">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="64f7c-113">Create calendar group</span><span class="sxs-lookup"><span data-stu-id="64f7c-113">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="64f7c-114">Calendar</span><span class="sxs-lookup"><span data-stu-id="64f7c-114">Calendar</span></span>](calendar.md)            | <span data-ttu-id="64f7c-115">Criar um novo grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="64f7c-115">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="64f7c-116">Get calendar group</span><span class="sxs-lookup"><span data-stu-id="64f7c-116">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="64f7c-117">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="64f7c-117">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="64f7c-118">Leia as propriedades e os relacionamentos de um objeto de grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="64f7c-118">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="64f7c-119">Update</span><span class="sxs-lookup"><span data-stu-id="64f7c-119">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="64f7c-120">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="64f7c-120">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="64f7c-121">Atualize o objeto calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="64f7c-121">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="64f7c-122">Excluir</span><span class="sxs-lookup"><span data-stu-id="64f7c-122">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="64f7c-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64f7c-123">None</span></span>                               | <span data-ttu-id="64f7c-124">Exclua o objeto calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="64f7c-124">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="64f7c-125">Listar calendários</span><span class="sxs-lookup"><span data-stu-id="64f7c-125">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="64f7c-126">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="64f7c-126">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="64f7c-127">Liste os calendários em um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="64f7c-127">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="64f7c-128">Create Calendar</span><span class="sxs-lookup"><span data-stu-id="64f7c-128">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="64f7c-129">Calendar</span><span class="sxs-lookup"><span data-stu-id="64f7c-129">Calendar</span></span>](calendar.md)            | <span data-ttu-id="64f7c-130">Crie um novo calendário em um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="64f7c-130">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="64f7c-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64f7c-131">Properties</span></span>

| <span data-ttu-id="64f7c-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64f7c-132">Property</span></span>  | <span data-ttu-id="64f7c-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="64f7c-133">Type</span></span>   | <span data-ttu-id="64f7c-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="64f7c-134">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="64f7c-135">nome</span><span class="sxs-lookup"><span data-stu-id="64f7c-135">name</span></span>      | <span data-ttu-id="64f7c-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64f7c-136">String</span></span> | <span data-ttu-id="64f7c-137">O nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="64f7c-137">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="64f7c-138">changeKey</span><span class="sxs-lookup"><span data-stu-id="64f7c-138">changeKey</span></span> | <span data-ttu-id="64f7c-139">String</span><span class="sxs-lookup"><span data-stu-id="64f7c-139">String</span></span> | <span data-ttu-id="64f7c-p101">Identifica a versão do grupo de calendários. Toda vez que o grupo de calendários é alterado, ChangeKey também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="64f7c-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="64f7c-144">classId</span><span class="sxs-lookup"><span data-stu-id="64f7c-144">classId</span></span>   | <span data-ttu-id="64f7c-145">Guid</span><span class="sxs-lookup"><span data-stu-id="64f7c-145">Guid</span></span>   | <span data-ttu-id="64f7c-p102">O identificador de classe. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="64f7c-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="64f7c-148">id</span><span class="sxs-lookup"><span data-stu-id="64f7c-148">id</span></span>        | <span data-ttu-id="64f7c-149">String</span><span class="sxs-lookup"><span data-stu-id="64f7c-149">String</span></span> | <span data-ttu-id="64f7c-p103">O identificador exclusivo do grupo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="64f7c-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="64f7c-152">Relações</span><span class="sxs-lookup"><span data-stu-id="64f7c-152">Relationships</span></span>

| <span data-ttu-id="64f7c-153">Relação</span><span class="sxs-lookup"><span data-stu-id="64f7c-153">Relationship</span></span> | <span data-ttu-id="64f7c-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="64f7c-154">Type</span></span>                               | <span data-ttu-id="64f7c-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="64f7c-155">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="64f7c-156">calendars</span><span class="sxs-lookup"><span data-stu-id="64f7c-156">calendars</span></span>    | <span data-ttu-id="64f7c-157">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="64f7c-157">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="64f7c-p104">Os calendários no grupo de calendários. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="64f7c-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="64f7c-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64f7c-162">JSON representation</span></span>

<span data-ttu-id="64f7c-163">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="64f7c-163">Here is a JSON representation of the resource</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
