---
title: tipo de recurso calendarPermission
description: As permissões de um usuário com quem o calendário é compartilhado.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5d19a1738d3369f2d910dd590062016acf3047ab
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950448"
---
# <a name="calendarpermission-resource-type"></a><span data-ttu-id="9d416-103">tipo de recurso calendarPermission</span><span class="sxs-lookup"><span data-stu-id="9d416-103">calendarPermission resource type</span></span>

<span data-ttu-id="9d416-104">As permissões de um usuário com quem o calendário é compartilhado.</span><span class="sxs-lookup"><span data-stu-id="9d416-104">The permissions of a user with whom the calendar is shared.</span></span> 

## <a name="methods"></a><span data-ttu-id="9d416-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="9d416-105">Methods</span></span>

| <span data-ttu-id="9d416-106">Método</span><span class="sxs-lookup"><span data-stu-id="9d416-106">Method</span></span>       | <span data-ttu-id="9d416-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9d416-107">Return Type</span></span> | <span data-ttu-id="9d416-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d416-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9d416-109">Obter calendarPermission</span><span class="sxs-lookup"><span data-stu-id="9d416-109">Get calendarPermission</span></span>](../api/calendarpermission-get.md) | [<span data-ttu-id="9d416-110">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="9d416-110">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="9d416-111">Leia as propriedades e os relacionamentos do objeto calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="9d416-111">Read properties and relationships of calendarPermission object.</span></span> |
| [<span data-ttu-id="9d416-112">Update</span><span class="sxs-lookup"><span data-stu-id="9d416-112">Update</span></span>](../api/calendarpermission-update.md) | [<span data-ttu-id="9d416-113">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="9d416-113">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="9d416-114">Atualize o objeto calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="9d416-114">Update calendarPermission object.</span></span> |
| [<span data-ttu-id="9d416-115">Delete</span><span class="sxs-lookup"><span data-stu-id="9d416-115">Delete</span></span>](../api/calendarpermission-delete.md) | <span data-ttu-id="9d416-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9d416-116">None</span></span> | <span data-ttu-id="9d416-117">Exclua o objeto calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="9d416-117">Delete calendarPermission object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9d416-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d416-118">Properties</span></span>

| <span data-ttu-id="9d416-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d416-119">Property</span></span>     | <span data-ttu-id="9d416-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d416-120">Type</span></span>        | <span data-ttu-id="9d416-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d416-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9d416-122">allowedRoles</span><span class="sxs-lookup"><span data-stu-id="9d416-122">allowedRoles</span></span>|<span data-ttu-id="9d416-123">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d416-123">string collection</span></span>| <span data-ttu-id="9d416-124">Lista de níveis de permissão de compartilhamento permitidos para o calendário.</span><span class="sxs-lookup"><span data-stu-id="9d416-124">List of allowed sharing permission levels for the calendar.</span></span> <span data-ttu-id="9d416-125">Os valores possíveis são: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="9d416-125">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="9d416-126">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9d416-126">emailAddress</span></span>|[<span data-ttu-id="9d416-127">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9d416-127">emailAddress</span></span>](emailaddress.md)| <span data-ttu-id="9d416-128">Representa um compartilhamento que tem acesso ao calendário.</span><span class="sxs-lookup"><span data-stu-id="9d416-128">Represents a sharee who has access to the calendar.</span></span> <span data-ttu-id="9d416-129">Para o compartilhamento "minha organização", a propriedade **Address** é NULL.</span><span class="sxs-lookup"><span data-stu-id="9d416-129">For the "My Organization" sharee, the **address** property is null.</span></span> |
|<span data-ttu-id="9d416-130">id</span><span class="sxs-lookup"><span data-stu-id="9d416-130">id</span></span>|<span data-ttu-id="9d416-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d416-131">String</span></span>| <span data-ttu-id="9d416-132">O identificador exclusivo do usuário (compartilhamento) com o qual o calendário foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="9d416-132">The unique identifier of the user (sharee) with whom the calendar has been shared.</span></span> <span data-ttu-id="9d416-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9d416-133">Read-only.</span></span>|
|<span data-ttu-id="9d416-134">isInsideOrganization</span><span class="sxs-lookup"><span data-stu-id="9d416-134">isInsideOrganization</span></span>|<span data-ttu-id="9d416-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="9d416-135">Boolean</span></span>| <span data-ttu-id="9d416-136">True se o usuário em contexto (compartilhamento) estiver dentro da mesma organização que o proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="9d416-136">True if the user in context (sharee) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="9d416-137">isRemovable</span><span class="sxs-lookup"><span data-stu-id="9d416-137">isRemovable</span></span>|<span data-ttu-id="9d416-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="9d416-138">Boolean</span></span>| <span data-ttu-id="9d416-139">`True`Se o usuário puder ser removido da lista de compartilhamentos do calendário especificado, `false` caso contrário.</span><span class="sxs-lookup"><span data-stu-id="9d416-139">`True` if the user can be removed from the list of sharees for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="9d416-140">O usuário "minha organização" determina as permissões que outras pessoas dentro da sua organização têm para o calendário especificado.</span><span class="sxs-lookup"><span data-stu-id="9d416-140">The "My organization" user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="9d416-141">Não é possível remover "minha organização" como um compartilhamento para um calendário.</span><span class="sxs-lookup"><span data-stu-id="9d416-141">You cannot remove "My organization" as a sharee to a calendar.</span></span>|
|<span data-ttu-id="9d416-142">role</span><span class="sxs-lookup"><span data-stu-id="9d416-142">role</span></span>|<span data-ttu-id="9d416-143">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="9d416-143">calendarRoleType</span></span>| <span data-ttu-id="9d416-144">Nível de permissão atual do compartilhamento de calendário.</span><span class="sxs-lookup"><span data-stu-id="9d416-144">Current permission level of the calendar sharee.</span></span> <span data-ttu-id="9d416-145">Os valores possíveis são: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="9d416-145">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d416-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d416-146">JSON representation</span></span>

<span data-ttu-id="9d416-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d416-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.calendarPermission",
  "keyProperty": "id"
}-->

```json
{
  "allowedRoles": ["string"],
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "id": "String (identifier)",
  "isInsideOrganization": "boolean",
  "isRemovable": "boolean",
  "role": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendarPermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->