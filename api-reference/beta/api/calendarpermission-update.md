---
title: Atualizar calendarpermission
description: Atualize as propriedades do objeto calendarpermission.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e69a1b4cdc66e9c591d060bed6600c4383e14a63
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936787"
---
# <a name="update-calendarpermission"></a><span data-ttu-id="80edc-103">Atualizar calendarPermission</span><span class="sxs-lookup"><span data-stu-id="80edc-103">Update calendarPermission</span></span>

<span data-ttu-id="80edc-104">Atualize as propriedades do objeto calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="80edc-104">Update the properties of calendarPermission object.</span></span>

## <a name="permissions"></a><span data-ttu-id="80edc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="80edc-105">Permissions</span></span>

<span data-ttu-id="80edc-106">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="80edc-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="80edc-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80edc-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="80edc-108">Calendário</span><span class="sxs-lookup"><span data-stu-id="80edc-108">Calendar</span></span> | <span data-ttu-id="80edc-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80edc-109">Delegated (work or school account)</span></span> | <span data-ttu-id="80edc-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80edc-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80edc-111">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80edc-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="80edc-112">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="80edc-112">user calendar</span></span> | <span data-ttu-id="80edc-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80edc-113">Calendars.ReadWrite</span></span> | <span data-ttu-id="80edc-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80edc-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="80edc-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80edc-115">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="80edc-116">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="80edc-116">group calendar</span></span> | <span data-ttu-id="80edc-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80edc-117">Group.ReadWrite.All</span></span> | <span data-ttu-id="80edc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80edc-118">Not supported.</span></span> | <span data-ttu-id="80edc-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80edc-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="80edc-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80edc-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
PATCH /groups/{id}/calendar/calendarPermissions/{id}
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="80edc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80edc-121">Request headers</span></span>

| <span data-ttu-id="80edc-122">Nome</span><span class="sxs-lookup"><span data-stu-id="80edc-122">Name</span></span>       | <span data-ttu-id="80edc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="80edc-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="80edc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="80edc-124">Authorization</span></span> | <span data-ttu-id="80edc-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="80edc-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="80edc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80edc-126">Request body</span></span>

<span data-ttu-id="80edc-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="80edc-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="80edc-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="80edc-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="80edc-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="80edc-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="80edc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80edc-130">Property</span></span>     | <span data-ttu-id="80edc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="80edc-131">Type</span></span>        | <span data-ttu-id="80edc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="80edc-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="80edc-133">allowedRoles</span><span class="sxs-lookup"><span data-stu-id="80edc-133">allowedRoles</span></span>|<span data-ttu-id="80edc-134">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="80edc-134">string collection</span></span>| <span data-ttu-id="80edc-135">Lista de níveis de permissão de compartilhamento permitidos para o calendário.</span><span class="sxs-lookup"><span data-stu-id="80edc-135">List of allowed sharing permission levels for the calendar.</span></span> <span data-ttu-id="80edc-136">Os valores possíveis são: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="80edc-136">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="80edc-137">emailAddress</span><span class="sxs-lookup"><span data-stu-id="80edc-137">emailAddress</span></span>|[<span data-ttu-id="80edc-138">emailAddress</span><span class="sxs-lookup"><span data-stu-id="80edc-138">emailAddress</span></span>](../resources/email.md)| <span data-ttu-id="80edc-139">Representa um compartilhamento que tem acesso ao calendário.</span><span class="sxs-lookup"><span data-stu-id="80edc-139">Represents a sharee who has access to the calendar.</span></span> <span data-ttu-id="80edc-140">Para o compartilhamento "minha organização", a propriedade **Address** é NULL.</span><span class="sxs-lookup"><span data-stu-id="80edc-140">For the "My Organization" sharee, the **address** property is null.</span></span> |
|<span data-ttu-id="80edc-141">id</span><span class="sxs-lookup"><span data-stu-id="80edc-141">id</span></span>|<span data-ttu-id="80edc-142">String</span><span class="sxs-lookup"><span data-stu-id="80edc-142">String</span></span>| <span data-ttu-id="80edc-143">O identificador exclusivo do usuário (compartilhamento) com o qual o calendário foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="80edc-143">The unique identifier of the user (sharee) with whom the calendar has been shared.</span></span> <span data-ttu-id="80edc-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80edc-144">Read-only.</span></span>|
|<span data-ttu-id="80edc-145">isInsideOrganization</span><span class="sxs-lookup"><span data-stu-id="80edc-145">isInsideOrganization</span></span>|<span data-ttu-id="80edc-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="80edc-146">Boolean</span></span>| <span data-ttu-id="80edc-147">True se o usuário em contexto (compartilhamento) estiver dentro da mesma organização que o proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="80edc-147">True if the user in context (sharee) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="80edc-148">isRemovable</span><span class="sxs-lookup"><span data-stu-id="80edc-148">isRemovable</span></span>|<span data-ttu-id="80edc-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="80edc-149">Boolean</span></span>| <span data-ttu-id="80edc-150">`True`Se o usuário puder ser removido da lista de compartilhamentos do calendário especificado, `false` caso contrário.</span><span class="sxs-lookup"><span data-stu-id="80edc-150">`True` if the user can be removed from the list of sharees for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="80edc-151">O usuário "minha organização" determina as permissões que outras pessoas dentro da sua organização têm para o calendário especificado.</span><span class="sxs-lookup"><span data-stu-id="80edc-151">The “My organization” user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="80edc-152">Não é possível remover "minha organização" como um compartilhamento para um calendário.</span><span class="sxs-lookup"><span data-stu-id="80edc-152">You cannot remove  “My organization” as a sharee to a calendar.</span></span>|
|<span data-ttu-id="80edc-153">role</span><span class="sxs-lookup"><span data-stu-id="80edc-153">role</span></span>|<span data-ttu-id="80edc-154">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="80edc-154">calendarRoleType</span></span>| <span data-ttu-id="80edc-155">Nível de permissão atual do compartilhamento de calendário.</span><span class="sxs-lookup"><span data-stu-id="80edc-155">Current permission level of the calendar sharee.</span></span> <span data-ttu-id="80edc-156">Os valores possíveis são: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="80edc-156">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="80edc-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="80edc-157">Response</span></span>

<span data-ttu-id="80edc-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [calendarPermission](../resources/calendarpermission.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80edc-158">If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="80edc-159">Exemplos</span><span class="sxs-lookup"><span data-stu-id="80edc-159">Examples</span></span>

### <a name="request"></a><span data-ttu-id="80edc-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80edc-160">Request</span></span>

<span data-ttu-id="80edc-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="80edc-161">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="80edc-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="80edc-162">Response</span></span>

<span data-ttu-id="80edc-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="80edc-163">The following is an example of the response.</span></span>

> <span data-ttu-id="80edc-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80edc-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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