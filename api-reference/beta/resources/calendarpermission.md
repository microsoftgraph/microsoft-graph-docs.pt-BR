---
title: tipo de recurso calendarPermission
description: As permissões de um usuário com quem o calendário é compartilhado.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 80c704dbb3e50d3f4d0ba586a40f06f74f032321
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2020
ms.locfileid: "41651733"
---
# <a name="calendarpermission-resource-type"></a><span data-ttu-id="31535-103">tipo de recurso calendarPermission</span><span class="sxs-lookup"><span data-stu-id="31535-103">calendarPermission resource type</span></span>

<span data-ttu-id="31535-104">As permissões de um usuário com o qual o calendário foi compartilhado ou delegado em um cliente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="31535-104">The permissions of a user with whom the calendar has been shared or delegated in an Outlook client.</span></span>

<span data-ttu-id="31535-105">Obter, atualizar e excluir permissões de calendário é suportada em nome apenas do proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="31535-105">Get, update, and delete of calendar permissions is supported on behalf of only the calendar owner.</span></span>

<span data-ttu-id="31535-106">Obter as permissões de calendário de um calendário em nome de um compartilhamento ou representante retorna uma coleção de permissões de calendário vazia.</span><span class="sxs-lookup"><span data-stu-id="31535-106">Getting the calendar permissions of a calendar on behalf of a sharee or delegate returns an empty calendar permissions collection.</span></span>

<span data-ttu-id="31535-107">Depois que um compartilhamento ou representante tiver sido configurado para um calendário, você poderá [Atualizar](../api/calendarpermission-update.md) somente a propriedade **role** para alterar as permissões de um compartilhamento ou representante.</span><span class="sxs-lookup"><span data-stu-id="31535-107">Once a sharee or delegate has been set up for a calendar, you can [update](../api/calendarpermission-update.md) only the **role** property to change the permissions of a sharee or delegate.</span></span> <span data-ttu-id="31535-108">Não é possível **Atualizar** a propriedade **allowedRoles**, **EmailAddress**, **isInsideOrganization**ou **isRemovable** .</span><span class="sxs-lookup"><span data-stu-id="31535-108">You cannot **update** the **allowedRoles**, **emailAddress**, **isInsideOrganization**, or **isRemovable** property.</span></span> <span data-ttu-id="31535-109">Para alterar essas propriedades, você deve [excluir](../api/calendarpermission-delete.md) o objeto **calendarPermission** correspondente e criar outro compartilhamento ou representante em um cliente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="31535-109">To change these properties, you should [delete](../api/calendarpermission-delete.md) the corresponding **calendarPermission** object and create another sharee or delegate in an Outlook client.</span></span>

## <a name="methods"></a><span data-ttu-id="31535-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="31535-110">Methods</span></span>

| <span data-ttu-id="31535-111">Método</span><span class="sxs-lookup"><span data-stu-id="31535-111">Method</span></span>       | <span data-ttu-id="31535-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="31535-112">Return Type</span></span> | <span data-ttu-id="31535-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="31535-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="31535-114">Obter calendarPermission</span><span class="sxs-lookup"><span data-stu-id="31535-114">Get calendarPermission</span></span>](../api/calendarpermission-get.md) | [<span data-ttu-id="31535-115">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="31535-115">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="31535-116">Leia as propriedades e os relacionamentos do objeto calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="31535-116">Read properties and relationships of calendarPermission object.</span></span> |
| [<span data-ttu-id="31535-117">Atualização</span><span class="sxs-lookup"><span data-stu-id="31535-117">Update</span></span>](../api/calendarpermission-update.md) | [<span data-ttu-id="31535-118">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="31535-118">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="31535-119">Atualize o objeto calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="31535-119">Update calendarPermission object.</span></span> |
| [<span data-ttu-id="31535-120">Delete</span><span class="sxs-lookup"><span data-stu-id="31535-120">Delete</span></span>](../api/calendarpermission-delete.md) | <span data-ttu-id="31535-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="31535-121">None</span></span> | <span data-ttu-id="31535-122">Exclua o objeto calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="31535-122">Delete calendarPermission object.</span></span> |

## <a name="properties"></a><span data-ttu-id="31535-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="31535-123">Properties</span></span>

| <span data-ttu-id="31535-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31535-124">Property</span></span>     | <span data-ttu-id="31535-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="31535-125">Type</span></span>        | <span data-ttu-id="31535-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="31535-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="31535-127">allowedRoles</span><span class="sxs-lookup"><span data-stu-id="31535-127">allowedRoles</span></span>|<span data-ttu-id="31535-128">coleção [calendarRoleType](#calendarroletype-values)</span><span class="sxs-lookup"><span data-stu-id="31535-128">[calendarRoleType](#calendarroletype-values) collection</span></span>| <span data-ttu-id="31535-129">Lista de níveis de permissão de compartilhamento ou de delegação permitidos para o calendário.</span><span class="sxs-lookup"><span data-stu-id="31535-129">List of allowed sharing or delegating permission levels for the calendar.</span></span> <span data-ttu-id="31535-130">Os valores possíveis são: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="31535-130">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="31535-131">emailAddress</span><span class="sxs-lookup"><span data-stu-id="31535-131">emailAddress</span></span>|[<span data-ttu-id="31535-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="31535-132">emailAddress</span></span>](emailaddress.md)| <span data-ttu-id="31535-133">Representa um compartilhamento ou representante que tem acesso ao calendário.</span><span class="sxs-lookup"><span data-stu-id="31535-133">Represents a sharee or delegate who has access to the calendar.</span></span> <span data-ttu-id="31535-134">Para o compartilhamento "minha organização", a propriedade **Address** é NULL.</span><span class="sxs-lookup"><span data-stu-id="31535-134">For the "My Organization" sharee, the **address** property is null.</span></span> <span data-ttu-id="31535-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31535-135">Read-only.</span></span> |
|<span data-ttu-id="31535-136">id</span><span class="sxs-lookup"><span data-stu-id="31535-136">id</span></span>|<span data-ttu-id="31535-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31535-137">String</span></span>| <span data-ttu-id="31535-138">O identificador exclusivo do usuário (compartilhamento ou representante) com o qual o calendário foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="31535-138">The unique identifier of the user (sharee or delegate) with whom the calendar has been shared.</span></span> <span data-ttu-id="31535-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31535-139">Read-only.</span></span>|
|<span data-ttu-id="31535-140">isInsideOrganization</span><span class="sxs-lookup"><span data-stu-id="31535-140">isInsideOrganization</span></span>|<span data-ttu-id="31535-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="31535-141">Boolean</span></span>| <span data-ttu-id="31535-142">True se o usuário em contexto (compartilhamento ou representante) estiver dentro da mesma organização que o proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="31535-142">True if the user in context (sharee or delegate) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="31535-143">isRemovable</span><span class="sxs-lookup"><span data-stu-id="31535-143">isRemovable</span></span>|<span data-ttu-id="31535-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="31535-144">Boolean</span></span>| <span data-ttu-id="31535-145">`True`Se o usuário puder ser removido da lista de compartilhamentos ou representantes do calendário especificado, `false` caso contrário.</span><span class="sxs-lookup"><span data-stu-id="31535-145">`True` if the user can be removed from the list of sharees or delegates for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="31535-146">O usuário "minha organização" determina as permissões que outras pessoas dentro da sua organização têm para o calendário especificado.</span><span class="sxs-lookup"><span data-stu-id="31535-146">The "My organization" user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="31535-147">Não é possível remover "minha organização" como um compartilhamento para um calendário.</span><span class="sxs-lookup"><span data-stu-id="31535-147">You cannot remove "My organization" as a sharee to a calendar.</span></span>|
|<span data-ttu-id="31535-148">role</span><span class="sxs-lookup"><span data-stu-id="31535-148">role</span></span>|[<span data-ttu-id="31535-149">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="31535-149">calendarRoleType</span></span>](#calendarroletype-values)| <span data-ttu-id="31535-150">Nível de permissão atual do compartilhamento ou representante do calendário.</span><span class="sxs-lookup"><span data-stu-id="31535-150">Current permission level of the calendar sharee or delegate.</span></span> |

### <a name="calendarroletype-values"></a><span data-ttu-id="31535-151">valores de calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="31535-151">calendarRoleType values</span></span>

| <span data-ttu-id="31535-152">Valores</span><span class="sxs-lookup"><span data-stu-id="31535-152">Values</span></span>        | <span data-ttu-id="31535-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="31535-153">Description</span></span> |
|:--------------|:------------|
| <span data-ttu-id="31535-154">nenhuma</span><span class="sxs-lookup"><span data-stu-id="31535-154">none</span></span> | <span data-ttu-id="31535-155">O calendário não é compartilhado com o usuário.</span><span class="sxs-lookup"><span data-stu-id="31535-155">Calendar is not shared with the user.</span></span> |
| <span data-ttu-id="31535-156">freeBusyRead</span><span class="sxs-lookup"><span data-stu-id="31535-156">freeBusyRead</span></span> | <span data-ttu-id="31535-157">O usuário é um compartilhamento que pode exibir o status de disponibilidade do proprietário no calendário.</span><span class="sxs-lookup"><span data-stu-id="31535-157">User is a sharee who can view free/busy status of the owner on the calendar.</span></span> |
| <span data-ttu-id="31535-158">limitedRead</span><span class="sxs-lookup"><span data-stu-id="31535-158">limitedRead</span></span> | <span data-ttu-id="31535-159">O usuário é um compartilhamento que pode exibir o status de disponibilidade e os títulos e locais dos eventos no calendário.</span><span class="sxs-lookup"><span data-stu-id="31535-159">User is a sharee who can view free/busy status, and titles and locations of the events on the calendar.</span></span> |
| <span data-ttu-id="31535-160">Saiba</span><span class="sxs-lookup"><span data-stu-id="31535-160">read</span></span> | <span data-ttu-id="31535-161">O usuário é um compartilhamento que pode exibir todos os detalhes dos eventos no calendário, exceto os eventos privados do proprietário.</span><span class="sxs-lookup"><span data-stu-id="31535-161">User is a sharee who can view all the details of the events on the calendar, except for the owner's private events.</span></span> |
| <span data-ttu-id="31535-162">gravável</span><span class="sxs-lookup"><span data-stu-id="31535-162">write</span></span> | <span data-ttu-id="31535-163">O usuário é um compartilhamento que pode exibir todos os detalhes (exceto eventos privados) e editar eventos no calendário.</span><span class="sxs-lookup"><span data-stu-id="31535-163">User is a sharee who can view all the details (except for private events) and edit events on the calendar.</span></span> |
| <span data-ttu-id="31535-164">delegateWithoutPrivateEventAccess</span><span class="sxs-lookup"><span data-stu-id="31535-164">delegateWithoutPrivateEventAccess</span></span> | <span data-ttu-id="31535-165">O usuário é um representante que tem acesso de gravação, mas não pode exibir informações dos eventos privados do proprietário no calendário.</span><span class="sxs-lookup"><span data-stu-id="31535-165">User is a delegate who has write access but cannot view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="31535-166">delegateWithPrivateEventAccess</span><span class="sxs-lookup"><span data-stu-id="31535-166">delegateWithPrivateEventAccess</span></span> | <span data-ttu-id="31535-167">O usuário é um representante que tem acesso de gravação e pode exibir informações dos eventos privados do proprietário no calendário.</span><span class="sxs-lookup"><span data-stu-id="31535-167">User is a delegate who has write access and can view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="31535-168">cliente</span><span class="sxs-lookup"><span data-stu-id="31535-168">custom</span></span> | <span data-ttu-id="31535-169">O usuário tem permissões personalizadas para o calendário.</span><span class="sxs-lookup"><span data-stu-id="31535-169">User has custom permissions to the calendar.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="31535-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="31535-170">JSON representation</span></span>

<span data-ttu-id="31535-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="31535-171">The following is a JSON representation of the resource.</span></span>

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