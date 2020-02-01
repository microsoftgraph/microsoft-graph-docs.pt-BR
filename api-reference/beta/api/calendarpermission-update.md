---
title: Atualizar calendarpermission
description: Atualize as propriedades do objeto calendarpermission.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 98deef23a65fd4bfa9fc2ae6f112d97e38cf9bf5
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2020
ms.locfileid: "41651964"
---
# <a name="update-calendarpermission"></a><span data-ttu-id="99ae3-103">Atualizar calendarPermission</span><span class="sxs-lookup"><span data-stu-id="99ae3-103">Update calendarPermission</span></span>

<span data-ttu-id="99ae3-104">Atualize as permissões atribuídas a um compartilhamento ou delegado existente, através do objeto [calendarPermission](../resources/calendarpermission.md) correspondente para um calendário.</span><span class="sxs-lookup"><span data-stu-id="99ae3-104">Update the permissions assigned to an existing sharee or delegate, through the corresponding [calendarPermission](../resources/calendarpermission.md) object for a calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="99ae3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="99ae3-105">Permissions</span></span>

<span data-ttu-id="99ae3-106">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="99ae3-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="99ae3-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99ae3-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="99ae3-108">Calendário</span><span class="sxs-lookup"><span data-stu-id="99ae3-108">Calendar</span></span> | <span data-ttu-id="99ae3-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99ae3-109">Delegated (work or school account)</span></span> | <span data-ttu-id="99ae3-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99ae3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99ae3-111">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99ae3-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="99ae3-112">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="99ae3-112">user calendar</span></span> | <span data-ttu-id="99ae3-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99ae3-113">Calendars.ReadWrite</span></span> | <span data-ttu-id="99ae3-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99ae3-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="99ae3-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99ae3-115">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="99ae3-116">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="99ae3-116">group calendar</span></span> | <span data-ttu-id="99ae3-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99ae3-117">Group.ReadWrite.All</span></span> | <span data-ttu-id="99ae3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99ae3-118">Not supported.</span></span> | <span data-ttu-id="99ae3-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99ae3-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="99ae3-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99ae3-120">HTTP request</span></span>

<span data-ttu-id="99ae3-121">Atualizar as permissões especificadas do calendário de um usuário:</span><span class="sxs-lookup"><span data-stu-id="99ae3-121">Update the specified permissions of a user's calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="99ae3-122">Atualizar as permissões especificadas de um calendário de Grupo:</span><span class="sxs-lookup"><span data-stu-id="99ae3-122">Update the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="99ae3-123">Atualize as permissões especificadas do calendário do usuário que contém o evento identificado:</span><span class="sxs-lookup"><span data-stu-id="99ae3-123">Update the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="99ae3-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99ae3-124">Request headers</span></span>

| <span data-ttu-id="99ae3-125">Nome</span><span class="sxs-lookup"><span data-stu-id="99ae3-125">Name</span></span>       | <span data-ttu-id="99ae3-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="99ae3-126">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="99ae3-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="99ae3-127">Authorization</span></span> | <span data-ttu-id="99ae3-128">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="99ae3-128">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="99ae3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99ae3-129">Request body</span></span>

<span data-ttu-id="99ae3-130">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="99ae3-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="99ae3-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="99ae3-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="99ae3-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="99ae3-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="99ae3-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99ae3-133">Property</span></span>     | <span data-ttu-id="99ae3-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="99ae3-134">Type</span></span>        | <span data-ttu-id="99ae3-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="99ae3-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="99ae3-136">role</span><span class="sxs-lookup"><span data-stu-id="99ae3-136">role</span></span>|[<span data-ttu-id="99ae3-137">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="99ae3-137">calendarRoleType</span></span>](../resources/calendarpermission.md#calendarroletype-values)| <span data-ttu-id="99ae3-138">O nível de permissão a ser alterado para o compartilhamento ou representante do calendário.</span><span class="sxs-lookup"><span data-stu-id="99ae3-138">The permission level to change to for the calendar sharee or delegate.</span></span> |

## <a name="response"></a><span data-ttu-id="99ae3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="99ae3-139">Response</span></span>

<span data-ttu-id="99ae3-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [calendarPermission](../resources/calendarpermission.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99ae3-140">If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="99ae3-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="99ae3-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="99ae3-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99ae3-142">Request</span></span>

<span data-ttu-id="99ae3-143">O exemplo a seguir altera o nível de permissão de Sharee, Adele, `write`para.</span><span class="sxs-lookup"><span data-stu-id="99ae3-143">The following example changes the permission level of the sharee, Adele, to `write`.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="99ae3-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="99ae3-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["RGVmYXVsdA=="],
  "name": "update_calendarpermission"
}-->

```http
PATCH https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/RGVmYXVsdA==
Content-type: application/json

{
  "role": "write"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="99ae3-145">C#</span><span class="sxs-lookup"><span data-stu-id="99ae3-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="99ae3-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99ae3-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="99ae3-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99ae3-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="99ae3-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="99ae3-148">Response</span></span>

<span data-ttu-id="99ae3-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="99ae3-149">The following is an example of the response.</span></span>

> <span data-ttu-id="99ae3-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99ae3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "update_calendarpermission",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "L289RXhlbGVW",
    "isRemovable": true,
    "isInsideOrganization": true,
    "role": "write",
    "allowedRoles": [
        "freeBusyRead",
        "limitedRead",
        "read",
        "write"
    ],
    "emailAddress": {
        "name": "Adele Vance",
        "address": "AdeleV@contoso.OnMicrosoft.com"
    }
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
