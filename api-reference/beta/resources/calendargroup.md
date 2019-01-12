---
title: Tipo de recurso calendarGroup
description: Um grupo de calendários do usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 10a840fd9ae9835eb5ca6a96b88719605f89245b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985288"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="008ab-103">Tipo de recurso calendarGroup</span><span class="sxs-lookup"><span data-stu-id="008ab-103">calendarGroup resource type</span></span>

> <span data-ttu-id="008ab-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="008ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="008ab-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="008ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="008ab-106">Um grupo de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="008ab-106">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="008ab-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="008ab-107">Methods</span></span>

| <span data-ttu-id="008ab-108">Método</span><span class="sxs-lookup"><span data-stu-id="008ab-108">Method</span></span>                                                      | <span data-ttu-id="008ab-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="008ab-109">Return Type</span></span>                        | <span data-ttu-id="008ab-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="008ab-110">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="008ab-111">List calendar groups</span><span class="sxs-lookup"><span data-stu-id="008ab-111">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="008ab-112">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="008ab-112">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="008ab-113">Obter os grupos de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="008ab-113">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="008ab-114">Create calendar group</span><span class="sxs-lookup"><span data-stu-id="008ab-114">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="008ab-115">Calendar</span><span class="sxs-lookup"><span data-stu-id="008ab-115">Calendar</span></span>](calendar.md)            | <span data-ttu-id="008ab-116">Criar um novo grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="008ab-116">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="008ab-117">Get calendar group</span><span class="sxs-lookup"><span data-stu-id="008ab-117">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="008ab-118">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="008ab-118">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="008ab-119">Leia as propriedades e os relacionamentos de um objeto de grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="008ab-119">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="008ab-120">Update</span><span class="sxs-lookup"><span data-stu-id="008ab-120">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="008ab-121">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="008ab-121">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="008ab-122">Atualize o objeto calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="008ab-122">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="008ab-123">Delete</span><span class="sxs-lookup"><span data-stu-id="008ab-123">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="008ab-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="008ab-124">None</span></span>                               | <span data-ttu-id="008ab-125">Exclua o objeto calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="008ab-125">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="008ab-126">List calendars</span><span class="sxs-lookup"><span data-stu-id="008ab-126">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="008ab-127">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="008ab-127">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="008ab-128">Liste os calendários em um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="008ab-128">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="008ab-129">Create Calendar</span><span class="sxs-lookup"><span data-stu-id="008ab-129">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="008ab-130">Calendar</span><span class="sxs-lookup"><span data-stu-id="008ab-130">Calendar</span></span>](calendar.md)            | <span data-ttu-id="008ab-131">Crie um novo calendário em um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="008ab-131">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="008ab-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="008ab-132">Properties</span></span>

| <span data-ttu-id="008ab-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="008ab-133">Property</span></span>  | <span data-ttu-id="008ab-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="008ab-134">Type</span></span>   | <span data-ttu-id="008ab-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="008ab-135">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="008ab-136">name</span><span class="sxs-lookup"><span data-stu-id="008ab-136">name</span></span>      | <span data-ttu-id="008ab-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="008ab-137">String</span></span> | <span data-ttu-id="008ab-138">O nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="008ab-138">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="008ab-139">changeKey</span><span class="sxs-lookup"><span data-stu-id="008ab-139">changeKey</span></span> | <span data-ttu-id="008ab-140">String</span><span class="sxs-lookup"><span data-stu-id="008ab-140">String</span></span> | <span data-ttu-id="008ab-p102">Identifica a versão do grupo de calendários. Toda vez que o grupo de calendários é alterado, ChangeKey também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="008ab-p102">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="008ab-145">classId</span><span class="sxs-lookup"><span data-stu-id="008ab-145">classId</span></span>   | <span data-ttu-id="008ab-146">Guid</span><span class="sxs-lookup"><span data-stu-id="008ab-146">Guid</span></span>   | <span data-ttu-id="008ab-p103">O identificador de classe. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="008ab-p103">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="008ab-149">id</span><span class="sxs-lookup"><span data-stu-id="008ab-149">id</span></span>        | <span data-ttu-id="008ab-150">String</span><span class="sxs-lookup"><span data-stu-id="008ab-150">String</span></span> | <span data-ttu-id="008ab-p104">O identificador exclusivo do grupo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="008ab-p104">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="008ab-153">Relações</span><span class="sxs-lookup"><span data-stu-id="008ab-153">Relationships</span></span>

| <span data-ttu-id="008ab-154">Relação</span><span class="sxs-lookup"><span data-stu-id="008ab-154">Relationship</span></span> | <span data-ttu-id="008ab-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="008ab-155">Type</span></span>                               | <span data-ttu-id="008ab-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="008ab-156">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="008ab-157">calendars</span><span class="sxs-lookup"><span data-stu-id="008ab-157">calendars</span></span>    | <span data-ttu-id="008ab-158">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="008ab-158">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="008ab-p105">Os calendários no grupo de calendários. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="008ab-p105">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="008ab-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="008ab-163">JSON representation</span></span>

<span data-ttu-id="008ab-164">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="008ab-164">Here is a JSON representation of the resource</span></span>

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
