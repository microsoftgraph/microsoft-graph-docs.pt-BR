---
title: Tipo de recurso calendarGroup
description: Um grupo de calendários do usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 4d141b63b840daa7730d17f9dcfc2e527c1ed66b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810322"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="17d67-103">Tipo de recurso calendarGroup</span><span class="sxs-lookup"><span data-stu-id="17d67-103">calendarGroup resource type</span></span>

> <span data-ttu-id="17d67-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="17d67-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17d67-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="17d67-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="17d67-106">Um grupo de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="17d67-106">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="17d67-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="17d67-107">Methods</span></span>

| <span data-ttu-id="17d67-108">Método</span><span class="sxs-lookup"><span data-stu-id="17d67-108">Method</span></span>                                                      | <span data-ttu-id="17d67-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="17d67-109">Return Type</span></span>                        | <span data-ttu-id="17d67-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="17d67-110">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="17d67-111">List calendar groups</span><span class="sxs-lookup"><span data-stu-id="17d67-111">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="17d67-112">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="17d67-112">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="17d67-113">Obter os grupos de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="17d67-113">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="17d67-114">Create calendar group</span><span class="sxs-lookup"><span data-stu-id="17d67-114">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="17d67-115">Calendar</span><span class="sxs-lookup"><span data-stu-id="17d67-115">Calendar</span></span>](calendar.md)            | <span data-ttu-id="17d67-116">Criar um novo grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="17d67-116">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="17d67-117">Get calendar group</span><span class="sxs-lookup"><span data-stu-id="17d67-117">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="17d67-118">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="17d67-118">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="17d67-119">Leia as propriedades e os relacionamentos de um objeto de grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="17d67-119">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="17d67-120">Update</span><span class="sxs-lookup"><span data-stu-id="17d67-120">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="17d67-121">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="17d67-121">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="17d67-122">Atualize o objeto calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="17d67-122">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="17d67-123">Delete</span><span class="sxs-lookup"><span data-stu-id="17d67-123">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="17d67-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="17d67-124">None</span></span>                               | <span data-ttu-id="17d67-125">Exclua o objeto calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="17d67-125">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="17d67-126">List calendars</span><span class="sxs-lookup"><span data-stu-id="17d67-126">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="17d67-127">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="17d67-127">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="17d67-128">Liste os calendários em um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="17d67-128">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="17d67-129">Create Calendar</span><span class="sxs-lookup"><span data-stu-id="17d67-129">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="17d67-130">Calendar</span><span class="sxs-lookup"><span data-stu-id="17d67-130">Calendar</span></span>](calendar.md)            | <span data-ttu-id="17d67-131">Crie um novo calendário em um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="17d67-131">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="17d67-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="17d67-132">Properties</span></span>

| <span data-ttu-id="17d67-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17d67-133">Property</span></span>  | <span data-ttu-id="17d67-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="17d67-134">Type</span></span>   | <span data-ttu-id="17d67-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="17d67-135">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="17d67-136">name</span><span class="sxs-lookup"><span data-stu-id="17d67-136">name</span></span>      | <span data-ttu-id="17d67-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17d67-137">String</span></span> | <span data-ttu-id="17d67-138">O nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="17d67-138">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="17d67-139">changeKey</span><span class="sxs-lookup"><span data-stu-id="17d67-139">changeKey</span></span> | <span data-ttu-id="17d67-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17d67-140">String</span></span> | <span data-ttu-id="17d67-p102">Identifica a versão do grupo de calendários. Toda vez que o grupo de calendários é alterado, ChangeKey também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="17d67-p102">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="17d67-145">classId</span><span class="sxs-lookup"><span data-stu-id="17d67-145">classId</span></span>   | <span data-ttu-id="17d67-146">Guid</span><span class="sxs-lookup"><span data-stu-id="17d67-146">Guid</span></span>   | <span data-ttu-id="17d67-p103">O identificador de classe. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="17d67-p103">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="17d67-149">id</span><span class="sxs-lookup"><span data-stu-id="17d67-149">id</span></span>        | <span data-ttu-id="17d67-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17d67-150">String</span></span> | <span data-ttu-id="17d67-p104">O identificador exclusivo do grupo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="17d67-p104">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="17d67-153">Relações</span><span class="sxs-lookup"><span data-stu-id="17d67-153">Relationships</span></span>

| <span data-ttu-id="17d67-154">Relação</span><span class="sxs-lookup"><span data-stu-id="17d67-154">Relationship</span></span> | <span data-ttu-id="17d67-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="17d67-155">Type</span></span>                               | <span data-ttu-id="17d67-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="17d67-156">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="17d67-157">calendars</span><span class="sxs-lookup"><span data-stu-id="17d67-157">calendars</span></span>    | <span data-ttu-id="17d67-158">Coleção [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="17d67-158">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="17d67-p105">Os calendários no grupo de calendários. Propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="17d67-p105">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="17d67-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17d67-163">JSON representation</span></span>

<span data-ttu-id="17d67-164">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="17d67-164">Here is a JSON representation of the resource</span></span>

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
