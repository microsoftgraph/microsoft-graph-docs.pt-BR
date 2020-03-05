---
title: Tipo de recurso calendarGroup
description: Um grupo de calendários do usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 175b3b8372214851ef62cf0740779b19fd2d4ce1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507828"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="a2752-103">Tipo de recurso calendarGroup</span><span class="sxs-lookup"><span data-stu-id="a2752-103">calendarGroup resource type</span></span>

<span data-ttu-id="a2752-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a2752-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2752-105">Um grupo de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="a2752-105">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="a2752-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="a2752-106">Methods</span></span>

| <span data-ttu-id="a2752-107">Método</span><span class="sxs-lookup"><span data-stu-id="a2752-107">Method</span></span>                                                      | <span data-ttu-id="a2752-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a2752-108">Return Type</span></span>                        | <span data-ttu-id="a2752-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2752-109">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="a2752-110">List calendar groups</span><span class="sxs-lookup"><span data-stu-id="a2752-110">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="a2752-111">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="a2752-111">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="a2752-112">Obter os grupos de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="a2752-112">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="a2752-113">Create calendar group</span><span class="sxs-lookup"><span data-stu-id="a2752-113">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="a2752-114">Calendar</span><span class="sxs-lookup"><span data-stu-id="a2752-114">Calendar</span></span>](calendar.md)            | <span data-ttu-id="a2752-115">Criar um novo grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="a2752-115">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="a2752-116">Get calendar group</span><span class="sxs-lookup"><span data-stu-id="a2752-116">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="a2752-117">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="a2752-117">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="a2752-118">Leia as propriedades e os relacionamentos de um objeto de grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="a2752-118">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="a2752-119">Update</span><span class="sxs-lookup"><span data-stu-id="a2752-119">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="a2752-120">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="a2752-120">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="a2752-121">Atualize o objeto calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="a2752-121">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="a2752-122">Delete</span><span class="sxs-lookup"><span data-stu-id="a2752-122">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="a2752-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a2752-123">None</span></span>                               | <span data-ttu-id="a2752-124">Exclua o objeto calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="a2752-124">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="a2752-125">Listar calendários</span><span class="sxs-lookup"><span data-stu-id="a2752-125">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="a2752-126">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="a2752-126">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="a2752-127">Liste os calendários em um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="a2752-127">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="a2752-128">Create Calendar</span><span class="sxs-lookup"><span data-stu-id="a2752-128">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="a2752-129">Calendar</span><span class="sxs-lookup"><span data-stu-id="a2752-129">Calendar</span></span>](calendar.md)            | <span data-ttu-id="a2752-130">Crie um novo calendário em um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="a2752-130">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="a2752-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2752-131">Properties</span></span>

| <span data-ttu-id="a2752-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2752-132">Property</span></span>  | <span data-ttu-id="a2752-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2752-133">Type</span></span>   | <span data-ttu-id="a2752-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2752-134">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="a2752-135">nome</span><span class="sxs-lookup"><span data-stu-id="a2752-135">name</span></span>      | <span data-ttu-id="a2752-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2752-136">String</span></span> | <span data-ttu-id="a2752-137">O nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="a2752-137">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="a2752-138">changeKey</span><span class="sxs-lookup"><span data-stu-id="a2752-138">changeKey</span></span> | <span data-ttu-id="a2752-139">String</span><span class="sxs-lookup"><span data-stu-id="a2752-139">String</span></span> | <span data-ttu-id="a2752-p101">Identifica a versão do grupo de calendários. Toda vez que o grupo de calendários é alterado, ChangeKey também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a2752-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="a2752-144">classId</span><span class="sxs-lookup"><span data-stu-id="a2752-144">classId</span></span>   | <span data-ttu-id="a2752-145">Guid</span><span class="sxs-lookup"><span data-stu-id="a2752-145">Guid</span></span>   | <span data-ttu-id="a2752-p102">O identificador de classe. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a2752-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="a2752-148">id</span><span class="sxs-lookup"><span data-stu-id="a2752-148">id</span></span>        | <span data-ttu-id="a2752-149">String</span><span class="sxs-lookup"><span data-stu-id="a2752-149">String</span></span> | <span data-ttu-id="a2752-p103">O identificador exclusivo do grupo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a2752-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="a2752-152">Relações</span><span class="sxs-lookup"><span data-stu-id="a2752-152">Relationships</span></span>

| <span data-ttu-id="a2752-153">Relação</span><span class="sxs-lookup"><span data-stu-id="a2752-153">Relationship</span></span> | <span data-ttu-id="a2752-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2752-154">Type</span></span>                               | <span data-ttu-id="a2752-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2752-155">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="a2752-156">calendars</span><span class="sxs-lookup"><span data-stu-id="a2752-156">calendars</span></span>    | <span data-ttu-id="a2752-157">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="a2752-157">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="a2752-p104">Os calendários no grupo de calendários. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="a2752-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a2752-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2752-162">JSON representation</span></span>

<span data-ttu-id="a2752-163">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a2752-163">Here is a JSON representation of the resource</span></span>

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
