---
title: tipo de recurso calendarPermission
description: As permissões de um usuário com quem o calendário é compartilhado.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5ba8b0021a815f6c1ae329523741b7d536994ca1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071609"
---
# <a name="calendarpermission-resource-type"></a><span data-ttu-id="2713b-103">tipo de recurso calendarPermission</span><span class="sxs-lookup"><span data-stu-id="2713b-103">calendarPermission resource type</span></span>

<span data-ttu-id="2713b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2713b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2713b-105">As permissões de um usuário com o qual o calendário foi compartilhado ou delegado em um cliente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="2713b-105">The permissions of a user with whom the calendar has been shared or delegated in an Outlook client.</span></span>

<span data-ttu-id="2713b-106">Obter, atualizar e excluir permissões de calendário é suportada em nome apenas do proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="2713b-106">Get, update, and delete of calendar permissions is supported on behalf of only the calendar owner.</span></span>

<span data-ttu-id="2713b-107">Obter as permissões de calendário de um calendário em nome de um compartilhamento ou representante retorna uma coleção de permissões de calendário vazia.</span><span class="sxs-lookup"><span data-stu-id="2713b-107">Getting the calendar permissions of a calendar on behalf of a sharee or delegate returns an empty calendar permissions collection.</span></span>

<span data-ttu-id="2713b-108">Depois que um compartilhamento ou representante tiver sido configurado para um calendário, você poderá [Atualizar](../api/calendarpermission-update.md) somente a propriedade **role** para alterar as permissões de um compartilhamento ou representante.</span><span class="sxs-lookup"><span data-stu-id="2713b-108">Once a sharee or delegate has been set up for a calendar, you can [update](../api/calendarpermission-update.md) only the **role** property to change the permissions of a sharee or delegate.</span></span> <span data-ttu-id="2713b-109">Não é possível **Atualizar** a propriedade **allowedRoles**, **EmailAddress**, **isInsideOrganization**ou **isRemovable** .</span><span class="sxs-lookup"><span data-stu-id="2713b-109">You cannot **update** the **allowedRoles**, **emailAddress**, **isInsideOrganization**, or **isRemovable** property.</span></span> <span data-ttu-id="2713b-110">Para alterar essas propriedades, você deve [excluir](../api/calendarpermission-delete.md) o objeto **calendarPermission** correspondente e criar outro compartilhamento ou representante em um cliente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="2713b-110">To change these properties, you should [delete](../api/calendarpermission-delete.md) the corresponding **calendarPermission** object and create another sharee or delegate in an Outlook client.</span></span>

## <a name="methods"></a><span data-ttu-id="2713b-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="2713b-111">Methods</span></span>

| <span data-ttu-id="2713b-112">Método</span><span class="sxs-lookup"><span data-stu-id="2713b-112">Method</span></span>       | <span data-ttu-id="2713b-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2713b-113">Return Type</span></span> | <span data-ttu-id="2713b-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="2713b-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2713b-115">Obter calendarPermission</span><span class="sxs-lookup"><span data-stu-id="2713b-115">Get calendarPermission</span></span>](../api/calendarpermission-get.md) | [<span data-ttu-id="2713b-116">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="2713b-116">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="2713b-117">Leia as propriedades e os relacionamentos do objeto calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="2713b-117">Read properties and relationships of calendarPermission object.</span></span> |
| [<span data-ttu-id="2713b-118">Update</span><span class="sxs-lookup"><span data-stu-id="2713b-118">Update</span></span>](../api/calendarpermission-update.md) | [<span data-ttu-id="2713b-119">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="2713b-119">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="2713b-120">Atualize o objeto calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="2713b-120">Update calendarPermission object.</span></span> |
| [<span data-ttu-id="2713b-121">Delete</span><span class="sxs-lookup"><span data-stu-id="2713b-121">Delete</span></span>](../api/calendarpermission-delete.md) | <span data-ttu-id="2713b-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2713b-122">None</span></span> | <span data-ttu-id="2713b-123">Exclua o objeto calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="2713b-123">Delete calendarPermission object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2713b-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2713b-124">Properties</span></span>

| <span data-ttu-id="2713b-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2713b-125">Property</span></span>     | <span data-ttu-id="2713b-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="2713b-126">Type</span></span>        | <span data-ttu-id="2713b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="2713b-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2713b-128">allowedRoles</span><span class="sxs-lookup"><span data-stu-id="2713b-128">allowedRoles</span></span>|<span data-ttu-id="2713b-129">coleção [calendarRoleType](#calendarroletype-values)</span><span class="sxs-lookup"><span data-stu-id="2713b-129">[calendarRoleType](#calendarroletype-values) collection</span></span>| <span data-ttu-id="2713b-130">Lista de níveis de permissão de compartilhamento ou de delegação permitidos para o calendário.</span><span class="sxs-lookup"><span data-stu-id="2713b-130">List of allowed sharing or delegating permission levels for the calendar.</span></span> <span data-ttu-id="2713b-131">Os valores possíveis são: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="2713b-131">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="2713b-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="2713b-132">emailAddress</span></span>|[<span data-ttu-id="2713b-133">emailAddress</span><span class="sxs-lookup"><span data-stu-id="2713b-133">emailAddress</span></span>](emailaddress.md)| <span data-ttu-id="2713b-134">Representa um compartilhamento ou representante que tem acesso ao calendário.</span><span class="sxs-lookup"><span data-stu-id="2713b-134">Represents a sharee or delegate who has access to the calendar.</span></span> <span data-ttu-id="2713b-135">Para o compartilhamento "minha organização", a propriedade **Address** é NULL.</span><span class="sxs-lookup"><span data-stu-id="2713b-135">For the "My Organization" sharee, the **address** property is null.</span></span> <span data-ttu-id="2713b-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2713b-136">Read-only.</span></span> |
|<span data-ttu-id="2713b-137">id</span><span class="sxs-lookup"><span data-stu-id="2713b-137">id</span></span>|<span data-ttu-id="2713b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2713b-138">String</span></span>| <span data-ttu-id="2713b-139">O identificador exclusivo do usuário (compartilhamento ou representante) com o qual o calendário foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="2713b-139">The unique identifier of the user (sharee or delegate) with whom the calendar has been shared.</span></span> <span data-ttu-id="2713b-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2713b-140">Read-only.</span></span>|
|<span data-ttu-id="2713b-141">isInsideOrganization</span><span class="sxs-lookup"><span data-stu-id="2713b-141">isInsideOrganization</span></span>|<span data-ttu-id="2713b-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="2713b-142">Boolean</span></span>| <span data-ttu-id="2713b-143">True se o usuário em contexto (compartilhamento ou representante) estiver dentro da mesma organização que o proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="2713b-143">True if the user in context (sharee or delegate) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="2713b-144">isRemovable</span><span class="sxs-lookup"><span data-stu-id="2713b-144">isRemovable</span></span>|<span data-ttu-id="2713b-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="2713b-145">Boolean</span></span>| <span data-ttu-id="2713b-146">`True` Se o usuário puder ser removido da lista de compartilhamentos ou representantes do calendário especificado, `false` caso contrário.</span><span class="sxs-lookup"><span data-stu-id="2713b-146">`True` if the user can be removed from the list of sharees or delegates for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="2713b-147">O usuário "minha organização" determina as permissões que outras pessoas dentro da sua organização têm para o calendário especificado.</span><span class="sxs-lookup"><span data-stu-id="2713b-147">The "My organization" user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="2713b-148">Não é possível remover "minha organização" como um compartilhamento para um calendário.</span><span class="sxs-lookup"><span data-stu-id="2713b-148">You cannot remove "My organization" as a sharee to a calendar.</span></span>|
|<span data-ttu-id="2713b-149">role</span><span class="sxs-lookup"><span data-stu-id="2713b-149">role</span></span>|[<span data-ttu-id="2713b-150">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="2713b-150">calendarRoleType</span></span>](#calendarroletype-values)| <span data-ttu-id="2713b-151">Nível de permissão atual do compartilhamento ou representante do calendário.</span><span class="sxs-lookup"><span data-stu-id="2713b-151">Current permission level of the calendar sharee or delegate.</span></span> |

### <a name="calendarroletype-values"></a><span data-ttu-id="2713b-152">valores de calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="2713b-152">calendarRoleType values</span></span>

| <span data-ttu-id="2713b-153">Valores</span><span class="sxs-lookup"><span data-stu-id="2713b-153">Values</span></span>        | <span data-ttu-id="2713b-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="2713b-154">Description</span></span> |
|:--------------|:------------|
| <span data-ttu-id="2713b-155">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="2713b-155">none</span></span> | <span data-ttu-id="2713b-156">O calendário não é compartilhado com o usuário.</span><span class="sxs-lookup"><span data-stu-id="2713b-156">Calendar is not shared with the user.</span></span> |
| <span data-ttu-id="2713b-157">freeBusyRead</span><span class="sxs-lookup"><span data-stu-id="2713b-157">freeBusyRead</span></span> | <span data-ttu-id="2713b-158">O usuário é um compartilhamento que pode exibir o status de disponibilidade do proprietário no calendário.</span><span class="sxs-lookup"><span data-stu-id="2713b-158">User is a sharee who can view free/busy status of the owner on the calendar.</span></span> |
| <span data-ttu-id="2713b-159">limitedRead</span><span class="sxs-lookup"><span data-stu-id="2713b-159">limitedRead</span></span> | <span data-ttu-id="2713b-160">O usuário é um compartilhamento que pode exibir o status de disponibilidade e os títulos e locais dos eventos no calendário.</span><span class="sxs-lookup"><span data-stu-id="2713b-160">User is a sharee who can view free/busy status, and titles and locations of the events on the calendar.</span></span> |
| <span data-ttu-id="2713b-161">leitura</span><span class="sxs-lookup"><span data-stu-id="2713b-161">read</span></span> | <span data-ttu-id="2713b-162">O usuário é um compartilhamento que pode exibir todos os detalhes dos eventos no calendário, exceto os eventos privados do proprietário.</span><span class="sxs-lookup"><span data-stu-id="2713b-162">User is a sharee who can view all the details of the events on the calendar, except for the owner's private events.</span></span> |
| <span data-ttu-id="2713b-163">gravação</span><span class="sxs-lookup"><span data-stu-id="2713b-163">write</span></span> | <span data-ttu-id="2713b-164">O usuário é um compartilhamento que pode exibir todos os detalhes (exceto eventos privados) e editar eventos no calendário.</span><span class="sxs-lookup"><span data-stu-id="2713b-164">User is a sharee who can view all the details (except for private events) and edit events on the calendar.</span></span> |
| <span data-ttu-id="2713b-165">delegateWithoutPrivateEventAccess</span><span class="sxs-lookup"><span data-stu-id="2713b-165">delegateWithoutPrivateEventAccess</span></span> | <span data-ttu-id="2713b-166">O usuário é um representante que tem acesso de gravação, mas não pode exibir informações dos eventos privados do proprietário no calendário.</span><span class="sxs-lookup"><span data-stu-id="2713b-166">User is a delegate who has write access but cannot view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="2713b-167">delegateWithPrivateEventAccess</span><span class="sxs-lookup"><span data-stu-id="2713b-167">delegateWithPrivateEventAccess</span></span> | <span data-ttu-id="2713b-168">O usuário é um representante que tem acesso de gravação e pode exibir informações dos eventos privados do proprietário no calendário.</span><span class="sxs-lookup"><span data-stu-id="2713b-168">User is a delegate who has write access and can view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="2713b-169">cliente</span><span class="sxs-lookup"><span data-stu-id="2713b-169">custom</span></span> | <span data-ttu-id="2713b-170">O usuário tem permissões personalizadas para o calendário.</span><span class="sxs-lookup"><span data-stu-id="2713b-170">User has custom permissions to the calendar.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="2713b-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2713b-171">JSON representation</span></span>

<span data-ttu-id="2713b-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2713b-172">The following is a JSON representation of the resource.</span></span>

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

