---
title: Tipo de recurso calendarPermission
description: As permissões de um usuário com quem o calendário é compartilhado.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8162220df0ebf6973f1b317c1e4c063dbc98de3e
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176700"
---
# <a name="calendarpermission-resource-type"></a><span data-ttu-id="4943e-103">Tipo de recurso calendarPermission</span><span class="sxs-lookup"><span data-stu-id="4943e-103">calendarPermission resource type</span></span>

<span data-ttu-id="4943e-104">As permissões de um usuário com o qual o calendário foi compartilhado ou delegado em um cliente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="4943e-104">The permissions of a user with whom the calendar has been shared or delegated in an Outlook client.</span></span>

<span data-ttu-id="4943e-105">Obter, atualizar e excluir permissões de calendário é suportado em nome apenas do proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="4943e-105">Get, update, and delete of calendar permissions is supported on behalf of only the calendar owner.</span></span>

<span data-ttu-id="4943e-106">Obter as permissões de calendário de um calendário em nome de um compartilhamento ou representante retorna uma coleção de permissões de calendário vazia.</span><span class="sxs-lookup"><span data-stu-id="4943e-106">Getting the calendar permissions of a calendar on behalf of a sharee or delegate returns an empty calendar permissions collection.</span></span>

<span data-ttu-id="4943e-107">Depois que um compartilhamento ou representante tiver sido [](../api/calendarpermission-update.md) definido  para um calendário, você poderá atualizar apenas a propriedade de função para alterar as permissões de um compartilhamento ou representante.</span><span class="sxs-lookup"><span data-stu-id="4943e-107">Once a sharee or delegate has been set up for a calendar, you can [update](../api/calendarpermission-update.md) only the **role** property to change the permissions of a sharee or delegate.</span></span> <span data-ttu-id="4943e-108">Você não **pode atualizar** a **propriedade allowedRoles**, **emailAddress**, **isInsideOrganization** ou **isRemovable.**</span><span class="sxs-lookup"><span data-stu-id="4943e-108">You cannot **update** the **allowedRoles**, **emailAddress**, **isInsideOrganization**, or **isRemovable** property.</span></span> <span data-ttu-id="4943e-109">Para alterar essas propriedades, você deve [excluir](../api/calendarpermission-delete.md) o objeto **calendarPermission** correspondente e criar outro compartilhamento ou representante em um cliente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="4943e-109">To change these properties, you should [delete](../api/calendarpermission-delete.md) the corresponding **calendarPermission** object and create another sharee or delegate in an Outlook client.</span></span>

## <a name="methods"></a><span data-ttu-id="4943e-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="4943e-110">Methods</span></span>

| <span data-ttu-id="4943e-111">Método</span><span class="sxs-lookup"><span data-stu-id="4943e-111">Method</span></span>       | <span data-ttu-id="4943e-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4943e-112">Return Type</span></span> | <span data-ttu-id="4943e-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="4943e-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4943e-114">Obter calendarPermission</span><span class="sxs-lookup"><span data-stu-id="4943e-114">Get calendarPermission</span></span>](../api/calendarpermission-get.md) | [<span data-ttu-id="4943e-115">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="4943e-115">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="4943e-116">Leia as propriedades e os relacionamentos do objeto calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="4943e-116">Read properties and relationships of calendarPermission object.</span></span> |
| [<span data-ttu-id="4943e-117">Update</span><span class="sxs-lookup"><span data-stu-id="4943e-117">Update</span></span>](../api/calendarpermission-update.md) | [<span data-ttu-id="4943e-118">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="4943e-118">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="4943e-119">Atualize o objeto calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="4943e-119">Update calendarPermission object.</span></span> |
| [<span data-ttu-id="4943e-120">Delete</span><span class="sxs-lookup"><span data-stu-id="4943e-120">Delete</span></span>](../api/calendarpermission-delete.md) | <span data-ttu-id="4943e-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4943e-121">None</span></span> | <span data-ttu-id="4943e-122">Exclua o objeto calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="4943e-122">Delete calendarPermission object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4943e-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4943e-123">Properties</span></span>

| <span data-ttu-id="4943e-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4943e-124">Property</span></span>     | <span data-ttu-id="4943e-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="4943e-125">Type</span></span>        | <span data-ttu-id="4943e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="4943e-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4943e-127">allowedRoles</span><span class="sxs-lookup"><span data-stu-id="4943e-127">allowedRoles</span></span>|<span data-ttu-id="4943e-128">[Coleção calendarRoleType](#calendarroletype-values)</span><span class="sxs-lookup"><span data-stu-id="4943e-128">[calendarRoleType](#calendarroletype-values) collection</span></span>| <span data-ttu-id="4943e-129">Lista de níveis de permissão permitidos de compartilhamento ou de delegação do calendário.</span><span class="sxs-lookup"><span data-stu-id="4943e-129">List of allowed sharing or delegating permission levels for the calendar.</span></span> <span data-ttu-id="4943e-130">Os valores possíveis são: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="4943e-130">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="4943e-131">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4943e-131">emailAddress</span></span>|[<span data-ttu-id="4943e-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4943e-132">emailAddress</span></span>](emailaddress.md)| <span data-ttu-id="4943e-133">Representa um compartilhamento ou representante que tem acesso ao calendário.</span><span class="sxs-lookup"><span data-stu-id="4943e-133">Represents a sharee or delegate who has access to the calendar.</span></span> <span data-ttu-id="4943e-134">Para o compartilhamento "Minha Organização", a propriedade **de** endereço é nula.</span><span class="sxs-lookup"><span data-stu-id="4943e-134">For the "My Organization" sharee, the **address** property is null.</span></span> <span data-ttu-id="4943e-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4943e-135">Read-only.</span></span> |
|<span data-ttu-id="4943e-136">id</span><span class="sxs-lookup"><span data-stu-id="4943e-136">id</span></span>|<span data-ttu-id="4943e-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4943e-137">String</span></span>| <span data-ttu-id="4943e-138">O identificador exclusivo do usuário (compartilhar ou delegar) com quem o calendário foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="4943e-138">The unique identifier of the user (sharee or delegate) with whom the calendar has been shared.</span></span> <span data-ttu-id="4943e-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4943e-139">Read-only.</span></span>|
|<span data-ttu-id="4943e-140">isInsideOrganization</span><span class="sxs-lookup"><span data-stu-id="4943e-140">isInsideOrganization</span></span>|<span data-ttu-id="4943e-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="4943e-141">Boolean</span></span>| <span data-ttu-id="4943e-142">True se o usuário no contexto (compartilhar ou delegar) estiver dentro da mesma organização que o proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="4943e-142">True if the user in context (sharee or delegate) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="4943e-143">isRemovable</span><span class="sxs-lookup"><span data-stu-id="4943e-143">isRemovable</span></span>|<span data-ttu-id="4943e-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="4943e-144">Boolean</span></span>| <span data-ttu-id="4943e-145">`True` se o usuário puder ser removido da lista de compartilhamentos ou representantes do calendário especificado, `false` caso contrário.</span><span class="sxs-lookup"><span data-stu-id="4943e-145">`True` if the user can be removed from the list of sharees or delegates for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="4943e-146">O usuário "Minha organização" determina as permissões que outras pessoas em sua organização têm para o calendário determinado.</span><span class="sxs-lookup"><span data-stu-id="4943e-146">The "My organization" user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="4943e-147">Não é possível remover "Minha organização" como um compartilhamento de um calendário.</span><span class="sxs-lookup"><span data-stu-id="4943e-147">You cannot remove "My organization" as a sharee to a calendar.</span></span>|
|<span data-ttu-id="4943e-148">role</span><span class="sxs-lookup"><span data-stu-id="4943e-148">role</span></span>|[<span data-ttu-id="4943e-149">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="4943e-149">calendarRoleType</span></span>](#calendarroletype-values)| <span data-ttu-id="4943e-150">Nível de permissão atual do compartilhamento de calendário ou representante.</span><span class="sxs-lookup"><span data-stu-id="4943e-150">Current permission level of the calendar sharee or delegate.</span></span> |

### <a name="calendarroletype-values"></a><span data-ttu-id="4943e-151">Valores de calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="4943e-151">calendarRoleType values</span></span>

| <span data-ttu-id="4943e-152">Member</span><span class="sxs-lookup"><span data-stu-id="4943e-152">Member</span></span>        | <span data-ttu-id="4943e-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="4943e-153">Description</span></span> |
|:--------------|:------------|
| <span data-ttu-id="4943e-154">nenhum</span><span class="sxs-lookup"><span data-stu-id="4943e-154">none</span></span> | <span data-ttu-id="4943e-155">O calendário não é compartilhado com o usuário.</span><span class="sxs-lookup"><span data-stu-id="4943e-155">Calendar is not shared with the user.</span></span> |
| <span data-ttu-id="4943e-156">freeBusyRead</span><span class="sxs-lookup"><span data-stu-id="4943e-156">freeBusyRead</span></span> | <span data-ttu-id="4943e-157">O usuário é um compartilhamento que pode exibir o status de livre/ocupado do proprietário no calendário.</span><span class="sxs-lookup"><span data-stu-id="4943e-157">User is a sharee who can view free/busy status of the owner on the calendar.</span></span> |
| <span data-ttu-id="4943e-158">limitedRead</span><span class="sxs-lookup"><span data-stu-id="4943e-158">limitedRead</span></span> | <span data-ttu-id="4943e-159">O usuário é um compartilhamento que pode exibir o status de livre/ocupado e títulos e locais dos eventos no calendário.</span><span class="sxs-lookup"><span data-stu-id="4943e-159">User is a sharee who can view free/busy status, and titles and locations of the events on the calendar.</span></span> |
| <span data-ttu-id="4943e-160">leitura</span><span class="sxs-lookup"><span data-stu-id="4943e-160">read</span></span> | <span data-ttu-id="4943e-161">O usuário é um compartilhamento que pode exibir todos os detalhes dos eventos no calendário, exceto os eventos particulares do proprietário.</span><span class="sxs-lookup"><span data-stu-id="4943e-161">User is a sharee who can view all the details of the events on the calendar, except for the owner's private events.</span></span> |
| <span data-ttu-id="4943e-162">gravação</span><span class="sxs-lookup"><span data-stu-id="4943e-162">write</span></span> | <span data-ttu-id="4943e-163">O usuário é um compartilhamento que pode exibir todos os detalhes (exceto eventos privados) e editar eventos no calendário.</span><span class="sxs-lookup"><span data-stu-id="4943e-163">User is a sharee who can view all the details (except for private events) and edit events on the calendar.</span></span> |
| <span data-ttu-id="4943e-164">delegateWithoutPrivateEventAccess</span><span class="sxs-lookup"><span data-stu-id="4943e-164">delegateWithoutPrivateEventAccess</span></span> | <span data-ttu-id="4943e-165">O usuário é um representante que tem acesso de gravação, mas não pode exibir informações dos eventos particulares do proprietário no calendário.</span><span class="sxs-lookup"><span data-stu-id="4943e-165">User is a delegate who has write access but cannot view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="4943e-166">delegateWithPrivateEventAccess</span><span class="sxs-lookup"><span data-stu-id="4943e-166">delegateWithPrivateEventAccess</span></span> | <span data-ttu-id="4943e-167">O usuário é um representante que tem acesso de gravação e pode exibir informações dos eventos particulares do proprietário no calendário.</span><span class="sxs-lookup"><span data-stu-id="4943e-167">User is a delegate who has write access and can view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="4943e-168">custom</span><span class="sxs-lookup"><span data-stu-id="4943e-168">custom</span></span> | <span data-ttu-id="4943e-169">O usuário tem permissões personalizadas para o calendário.</span><span class="sxs-lookup"><span data-stu-id="4943e-169">User has custom permissions to the calendar.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="4943e-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4943e-170">JSON representation</span></span>

<span data-ttu-id="4943e-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4943e-171">The following is a JSON representation of the resource.</span></span>

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
