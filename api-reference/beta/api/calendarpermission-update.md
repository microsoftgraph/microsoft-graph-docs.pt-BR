---
title: Atualizar calendarpermission
description: Atualize as propriedades do objeto calendarpermission.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d1cd959c4ee083ff6ec26914c5f99ccd3d8c3c8f
ms.sourcegitcommit: 1a3ca53422fc9a8254e78af7c058e876fc9f9ef8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2019
ms.locfileid: "37942633"
---
# <a name="update-calendarpermission"></a><span data-ttu-id="e18e0-103">Atualizar calendarPermission</span><span class="sxs-lookup"><span data-stu-id="e18e0-103">Update calendarPermission</span></span>

<span data-ttu-id="e18e0-104">Atualize as propriedades do objeto calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="e18e0-104">Update the properties of calendarPermission object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e18e0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e18e0-105">Permissions</span></span>

<span data-ttu-id="e18e0-106">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="e18e0-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="e18e0-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e18e0-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e18e0-108">Calendário</span><span class="sxs-lookup"><span data-stu-id="e18e0-108">Calendar</span></span> | <span data-ttu-id="e18e0-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e18e0-109">Delegated (work or school account)</span></span> | <span data-ttu-id="e18e0-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e18e0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e18e0-111">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e18e0-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="e18e0-112">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="e18e0-112">user calendar</span></span> | <span data-ttu-id="e18e0-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e18e0-113">Calendars.ReadWrite</span></span> | <span data-ttu-id="e18e0-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e18e0-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="e18e0-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e18e0-115">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="e18e0-116">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="e18e0-116">group calendar</span></span> | <span data-ttu-id="e18e0-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e18e0-117">Group.ReadWrite.All</span></span> | <span data-ttu-id="e18e0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e18e0-118">Not supported.</span></span> | <span data-ttu-id="e18e0-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e18e0-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e18e0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e18e0-120">HTTP request</span></span>

<span data-ttu-id="e18e0-121">Atualizar as permissões especificadas do calendário principal de um usuário:</span><span class="sxs-lookup"><span data-stu-id="e18e0-121">Update the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="e18e0-122">Atualizar as permissões especificadas de um calendário de Grupo:</span><span class="sxs-lookup"><span data-stu-id="e18e0-122">Update the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="e18e0-123">Atualize as permissões especificadas do calendário do usuário que contém o evento identificado:</span><span class="sxs-lookup"><span data-stu-id="e18e0-123">Update the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e18e0-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e18e0-124">Request headers</span></span>

| <span data-ttu-id="e18e0-125">Nome</span><span class="sxs-lookup"><span data-stu-id="e18e0-125">Name</span></span>       | <span data-ttu-id="e18e0-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e18e0-126">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e18e0-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="e18e0-127">Authorization</span></span> | <span data-ttu-id="e18e0-128">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="e18e0-128">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e18e0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e18e0-129">Request body</span></span>

<span data-ttu-id="e18e0-130">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="e18e0-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e18e0-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="e18e0-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e18e0-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e18e0-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e18e0-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e18e0-133">Property</span></span>     | <span data-ttu-id="e18e0-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="e18e0-134">Type</span></span>        | <span data-ttu-id="e18e0-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="e18e0-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e18e0-136">allowedRoles</span><span class="sxs-lookup"><span data-stu-id="e18e0-136">allowedRoles</span></span>|<span data-ttu-id="e18e0-137">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e18e0-137">string collection</span></span>| <span data-ttu-id="e18e0-138">Lista de níveis de permissão de compartilhamento permitidos para o calendário.</span><span class="sxs-lookup"><span data-stu-id="e18e0-138">List of allowed sharing permission levels for the calendar.</span></span> <span data-ttu-id="e18e0-139">Os valores possíveis são: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="e18e0-139">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="e18e0-140">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e18e0-140">emailAddress</span></span>|[<span data-ttu-id="e18e0-141">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e18e0-141">emailAddress</span></span>](../resources/email.md)| <span data-ttu-id="e18e0-142">Representa um compartilhamento que tem acesso ao calendário.</span><span class="sxs-lookup"><span data-stu-id="e18e0-142">Represents a sharee who has access to the calendar.</span></span> <span data-ttu-id="e18e0-143">Para o compartilhamento "minha organização", a propriedade **Address** é NULL.</span><span class="sxs-lookup"><span data-stu-id="e18e0-143">For the "My Organization" sharee, the **address** property is null.</span></span> |
|<span data-ttu-id="e18e0-144">id</span><span class="sxs-lookup"><span data-stu-id="e18e0-144">id</span></span>|<span data-ttu-id="e18e0-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e18e0-145">String</span></span>| <span data-ttu-id="e18e0-146">O identificador exclusivo do usuário (compartilhamento) com o qual o calendário foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="e18e0-146">The unique identifier of the user (sharee) with whom the calendar has been shared.</span></span> <span data-ttu-id="e18e0-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e18e0-147">Read-only.</span></span>|
|<span data-ttu-id="e18e0-148">isInsideOrganization</span><span class="sxs-lookup"><span data-stu-id="e18e0-148">isInsideOrganization</span></span>|<span data-ttu-id="e18e0-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="e18e0-149">Boolean</span></span>| <span data-ttu-id="e18e0-150">True se o usuário em contexto (compartilhamento) estiver dentro da mesma organização que o proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="e18e0-150">True if the user in context (sharee) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="e18e0-151">isRemovable</span><span class="sxs-lookup"><span data-stu-id="e18e0-151">isRemovable</span></span>|<span data-ttu-id="e18e0-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="e18e0-152">Boolean</span></span>| <span data-ttu-id="e18e0-153">`True`Se o usuário puder ser removido da lista de compartilhamentos do calendário especificado, `false` caso contrário.</span><span class="sxs-lookup"><span data-stu-id="e18e0-153">`True` if the user can be removed from the list of sharees for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="e18e0-154">O usuário "minha organização" determina as permissões que outras pessoas dentro da sua organização têm para o calendário especificado.</span><span class="sxs-lookup"><span data-stu-id="e18e0-154">The “My organization” user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="e18e0-155">Não é possível remover "minha organização" como um compartilhamento para um calendário.</span><span class="sxs-lookup"><span data-stu-id="e18e0-155">You cannot remove  “My organization” as a sharee to a calendar.</span></span>|
|<span data-ttu-id="e18e0-156">role</span><span class="sxs-lookup"><span data-stu-id="e18e0-156">role</span></span>|<span data-ttu-id="e18e0-157">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="e18e0-157">calendarRoleType</span></span>| <span data-ttu-id="e18e0-158">Nível de permissão atual do compartilhamento de calendário.</span><span class="sxs-lookup"><span data-stu-id="e18e0-158">Current permission level of the calendar sharee.</span></span> <span data-ttu-id="e18e0-159">Os valores possíveis são: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="e18e0-159">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="e18e0-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="e18e0-160">Response</span></span>

<span data-ttu-id="e18e0-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [calendarPermission](../resources/calendarpermission.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e18e0-161">If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e18e0-162">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e18e0-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e18e0-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e18e0-163">Request</span></span>

<span data-ttu-id="e18e0-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e18e0-164">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_calendarpermission"
}-->

```http
PATCH https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
Content-type: application/json

{
  "emailAddress": {
    "name": "My Organization",
  },
  "isRemovable": true,
  "isInsideOrganization": true,
  "role": "write",
  "allowedRoles": [
    "none",
    "freeBusyRead",
    "limitedRead",
    "read",
    "write"
  ],
  "id": "RGVmYXVsdA=="
}
```

### <a name="response"></a><span data-ttu-id="e18e0-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="e18e0-165">Response</span></span>

<span data-ttu-id="e18e0-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e18e0-166">The following is an example of the response.</span></span>

> <span data-ttu-id="e18e0-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e18e0-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "emailAddress": {
    "name": "My Organization",
  },
  "isRemovable": true,
  "isInsideOrganization": true,
  "role": "write",
  "allowedRoles": [
    "none",
    "freeBusyRead",
    "limitedRead",
    "read",
    "write"
  ],
  "id": "RGVmYXVsdA=="
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update calendarpermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->