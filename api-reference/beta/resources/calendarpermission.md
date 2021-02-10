---
title: Tipo de recurso calendarPermission
description: As permissões de um usuário com quem o calendário é compartilhado.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0c8cf612827819370a43b02dbb7064d03530a5d1
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177092"
---
# <a name="calendarpermission-resource-type"></a><span data-ttu-id="a5a83-103">Tipo de recurso calendarPermission</span><span class="sxs-lookup"><span data-stu-id="a5a83-103">calendarPermission resource type</span></span>

<span data-ttu-id="a5a83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5a83-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a5a83-105">As permissões de um usuário com quem o calendário foi compartilhado ou delegado em um cliente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="a5a83-105">The permissions of a user with whom the calendar has been shared or delegated in an Outlook client.</span></span>

<span data-ttu-id="a5a83-106">Obter, atualizar e excluir permissões de calendário é suportado em nome apenas do proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="a5a83-106">Get, update, and delete of calendar permissions is supported on behalf of only the calendar owner.</span></span>

<span data-ttu-id="a5a83-107">Obter as permissões de calendário de um calendário em nome de um compartilhamento ou representante retorna uma coleção de permissões de calendário vazia.</span><span class="sxs-lookup"><span data-stu-id="a5a83-107">Getting the calendar permissions of a calendar on behalf of a sharee or delegate returns an empty calendar permissions collection.</span></span>

<span data-ttu-id="a5a83-108">Depois que um compartilhamento ou representante tiver sido [](../api/calendarpermission-update.md) definido  para um calendário, você poderá atualizar apenas a propriedade de função para alterar as permissões de um compartilhamento ou representante.</span><span class="sxs-lookup"><span data-stu-id="a5a83-108">Once a sharee or delegate has been set up for a calendar, you can [update](../api/calendarpermission-update.md) only the **role** property to change the permissions of a sharee or delegate.</span></span> <span data-ttu-id="a5a83-109">Você não **pode atualizar** a **propriedade allowedRoles**, **emailAddress**, **isInsideOrganization** ou **isRemovable.**</span><span class="sxs-lookup"><span data-stu-id="a5a83-109">You cannot **update** the **allowedRoles**, **emailAddress**, **isInsideOrganization**, or **isRemovable** property.</span></span> <span data-ttu-id="a5a83-110">Para alterar essas propriedades, você deve [excluir](../api/calendarpermission-delete.md) o objeto **calendarPermission** correspondente e criar outro compartilhamento ou representante em um cliente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="a5a83-110">To change these properties, you should [delete](../api/calendarpermission-delete.md) the corresponding **calendarPermission** object and create another sharee or delegate in an Outlook client.</span></span>

## <a name="methods"></a><span data-ttu-id="a5a83-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="a5a83-111">Methods</span></span>

| <span data-ttu-id="a5a83-112">Método</span><span class="sxs-lookup"><span data-stu-id="a5a83-112">Method</span></span>       | <span data-ttu-id="a5a83-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a5a83-113">Return Type</span></span> | <span data-ttu-id="a5a83-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5a83-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a5a83-115">Obter calendarPermission</span><span class="sxs-lookup"><span data-stu-id="a5a83-115">Get calendarPermission</span></span>](../api/calendarpermission-get.md) | [<span data-ttu-id="a5a83-116">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="a5a83-116">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="a5a83-117">Leia as propriedades e os relacionamentos do objeto calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="a5a83-117">Read properties and relationships of calendarPermission object.</span></span> |
| [<span data-ttu-id="a5a83-118">Update</span><span class="sxs-lookup"><span data-stu-id="a5a83-118">Update</span></span>](../api/calendarpermission-update.md) | [<span data-ttu-id="a5a83-119">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="a5a83-119">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="a5a83-120">Atualize o objeto calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="a5a83-120">Update calendarPermission object.</span></span> |
| [<span data-ttu-id="a5a83-121">Delete</span><span class="sxs-lookup"><span data-stu-id="a5a83-121">Delete</span></span>](../api/calendarpermission-delete.md) | <span data-ttu-id="a5a83-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a5a83-122">None</span></span> | <span data-ttu-id="a5a83-123">Exclua o objeto calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="a5a83-123">Delete calendarPermission object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a5a83-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5a83-124">Properties</span></span>

| <span data-ttu-id="a5a83-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5a83-125">Property</span></span>     | <span data-ttu-id="a5a83-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5a83-126">Type</span></span>        | <span data-ttu-id="a5a83-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5a83-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a5a83-128">allowedRoles</span><span class="sxs-lookup"><span data-stu-id="a5a83-128">allowedRoles</span></span>|<span data-ttu-id="a5a83-129">[Coleção calendarRoleType](#calendarroletype-values)</span><span class="sxs-lookup"><span data-stu-id="a5a83-129">[calendarRoleType](#calendarroletype-values) collection</span></span>| <span data-ttu-id="a5a83-130">Lista de níveis de permissão de compartilhamento ou delegação permitidos para o calendário.</span><span class="sxs-lookup"><span data-stu-id="a5a83-130">List of allowed sharing or delegating permission levels for the calendar.</span></span> <span data-ttu-id="a5a83-131">Os valores possíveis são: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="a5a83-131">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="a5a83-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a5a83-132">emailAddress</span></span>|[<span data-ttu-id="a5a83-133">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a5a83-133">emailAddress</span></span>](emailaddress.md)| <span data-ttu-id="a5a83-134">Representa um compartilhamento ou representante que tem acesso ao calendário.</span><span class="sxs-lookup"><span data-stu-id="a5a83-134">Represents a sharee or delegate who has access to the calendar.</span></span> <span data-ttu-id="a5a83-135">Para o compartilhamento "Minha Organização", a propriedade **de** endereço é nula.</span><span class="sxs-lookup"><span data-stu-id="a5a83-135">For the "My Organization" sharee, the **address** property is null.</span></span> <span data-ttu-id="a5a83-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a5a83-136">Read-only.</span></span> |
|<span data-ttu-id="a5a83-137">id</span><span class="sxs-lookup"><span data-stu-id="a5a83-137">id</span></span>|<span data-ttu-id="a5a83-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5a83-138">String</span></span>| <span data-ttu-id="a5a83-139">O identificador exclusivo do usuário (compartilhar ou delegar) com quem o calendário foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="a5a83-139">The unique identifier of the user (sharee or delegate) with whom the calendar has been shared.</span></span> <span data-ttu-id="a5a83-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a5a83-140">Read-only.</span></span>|
|<span data-ttu-id="a5a83-141">isInsideOrganization</span><span class="sxs-lookup"><span data-stu-id="a5a83-141">isInsideOrganization</span></span>|<span data-ttu-id="a5a83-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5a83-142">Boolean</span></span>| <span data-ttu-id="a5a83-143">True se o usuário no contexto (compartilhar ou delegar) estiver dentro da mesma organização que o proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="a5a83-143">True if the user in context (sharee or delegate) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="a5a83-144">isRemovable</span><span class="sxs-lookup"><span data-stu-id="a5a83-144">isRemovable</span></span>|<span data-ttu-id="a5a83-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5a83-145">Boolean</span></span>| <span data-ttu-id="a5a83-146">`True` se o usuário puder ser removido da lista de compartilhamentos ou representantes do calendário especificado, `false` caso contrário.</span><span class="sxs-lookup"><span data-stu-id="a5a83-146">`True` if the user can be removed from the list of sharees or delegates for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="a5a83-147">O usuário "Minha organização" determina as permissões que outras pessoas em sua organização têm para o calendário determinado.</span><span class="sxs-lookup"><span data-stu-id="a5a83-147">The "My organization" user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="a5a83-148">Não é possível remover "Minha organização" como um compartilhamento de um calendário.</span><span class="sxs-lookup"><span data-stu-id="a5a83-148">You cannot remove "My organization" as a sharee to a calendar.</span></span>|
|<span data-ttu-id="a5a83-149">role</span><span class="sxs-lookup"><span data-stu-id="a5a83-149">role</span></span>|[<span data-ttu-id="a5a83-150">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="a5a83-150">calendarRoleType</span></span>](#calendarroletype-values)| <span data-ttu-id="a5a83-151">Nível de permissão atual do compartilhamento de calendário ou representante.</span><span class="sxs-lookup"><span data-stu-id="a5a83-151">Current permission level of the calendar sharee or delegate.</span></span> |

### <a name="calendarroletype-values"></a><span data-ttu-id="a5a83-152">Valores de calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="a5a83-152">calendarRoleType values</span></span>

| <span data-ttu-id="a5a83-153">Member</span><span class="sxs-lookup"><span data-stu-id="a5a83-153">Member</span></span>        | <span data-ttu-id="a5a83-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5a83-154">Description</span></span> |
|:--------------|:------------|
| <span data-ttu-id="a5a83-155">nenhum</span><span class="sxs-lookup"><span data-stu-id="a5a83-155">none</span></span> | <span data-ttu-id="a5a83-156">O calendário não é compartilhado com o usuário.</span><span class="sxs-lookup"><span data-stu-id="a5a83-156">Calendar is not shared with the user.</span></span> |
| <span data-ttu-id="a5a83-157">freeBusyRead</span><span class="sxs-lookup"><span data-stu-id="a5a83-157">freeBusyRead</span></span> | <span data-ttu-id="a5a83-158">O usuário é um compartilhamento que pode exibir o status de livre/ocupado do proprietário no calendário.</span><span class="sxs-lookup"><span data-stu-id="a5a83-158">User is a sharee who can view free/busy status of the owner on the calendar.</span></span> |
| <span data-ttu-id="a5a83-159">limitedRead</span><span class="sxs-lookup"><span data-stu-id="a5a83-159">limitedRead</span></span> | <span data-ttu-id="a5a83-160">O usuário é um compartilhamento que pode exibir o status de livre/ocupado e títulos e locais dos eventos no calendário.</span><span class="sxs-lookup"><span data-stu-id="a5a83-160">User is a sharee who can view free/busy status, and titles and locations of the events on the calendar.</span></span> |
| <span data-ttu-id="a5a83-161">leitura</span><span class="sxs-lookup"><span data-stu-id="a5a83-161">read</span></span> | <span data-ttu-id="a5a83-162">O usuário é um compartilhamento que pode exibir todos os detalhes dos eventos no calendário, exceto os eventos particulares do proprietário.</span><span class="sxs-lookup"><span data-stu-id="a5a83-162">User is a sharee who can view all the details of the events on the calendar, except for the owner's private events.</span></span> |
| <span data-ttu-id="a5a83-163">gravação</span><span class="sxs-lookup"><span data-stu-id="a5a83-163">write</span></span> | <span data-ttu-id="a5a83-164">O usuário é um compartilhamento que pode exibir todos os detalhes (exceto eventos privados) e editar eventos no calendário.</span><span class="sxs-lookup"><span data-stu-id="a5a83-164">User is a sharee who can view all the details (except for private events) and edit events on the calendar.</span></span> |
| <span data-ttu-id="a5a83-165">delegateWithoutPrivateEventAccess</span><span class="sxs-lookup"><span data-stu-id="a5a83-165">delegateWithoutPrivateEventAccess</span></span> | <span data-ttu-id="a5a83-166">O usuário é um representante que tem acesso de gravação, mas não pode exibir informações dos eventos particulares do proprietário no calendário.</span><span class="sxs-lookup"><span data-stu-id="a5a83-166">User is a delegate who has write access but cannot view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="a5a83-167">delegateWithPrivateEventAccess</span><span class="sxs-lookup"><span data-stu-id="a5a83-167">delegateWithPrivateEventAccess</span></span> | <span data-ttu-id="a5a83-168">O usuário é um representante que tem acesso de gravação e pode exibir informações dos eventos particulares do proprietário no calendário.</span><span class="sxs-lookup"><span data-stu-id="a5a83-168">User is a delegate who has write access and can view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="a5a83-169">custom</span><span class="sxs-lookup"><span data-stu-id="a5a83-169">custom</span></span> | <span data-ttu-id="a5a83-170">O usuário tem permissões personalizadas para o calendário.</span><span class="sxs-lookup"><span data-stu-id="a5a83-170">User has custom permissions to the calendar.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="a5a83-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5a83-171">JSON representation</span></span>

<span data-ttu-id="a5a83-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a5a83-172">The following is a JSON representation of the resource.</span></span>

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

