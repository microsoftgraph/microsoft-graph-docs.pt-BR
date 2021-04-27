---
title: Atualizar calendarpermission
description: Atualize as propriedades do objeto calendarpermission.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 116352b351d66bdc2c413eb1aad9357407d25631
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047676"
---
# <a name="update-calendarpermission"></a><span data-ttu-id="0cc45-103">Atualizar calendarPermission</span><span class="sxs-lookup"><span data-stu-id="0cc45-103">Update calendarPermission</span></span>

<span data-ttu-id="0cc45-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cc45-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0cc45-105">Atualize as permissões atribuídas a um compartilhamento ou representante existente, por meio do [objeto calendarPermission](../resources/calendarpermission.md) correspondente para um calendário.</span><span class="sxs-lookup"><span data-stu-id="0cc45-105">Update the permissions assigned to an existing sharee or delegate, through the corresponding [calendarPermission](../resources/calendarpermission.md) object for a calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cc45-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0cc45-106">Permissions</span></span>

<span data-ttu-id="0cc45-107">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="0cc45-107">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="0cc45-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cc45-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0cc45-109">Calendário</span><span class="sxs-lookup"><span data-stu-id="0cc45-109">Calendar</span></span> | <span data-ttu-id="0cc45-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cc45-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0cc45-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cc45-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cc45-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cc45-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="0cc45-113">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="0cc45-113">user calendar</span></span> | <span data-ttu-id="0cc45-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0cc45-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="0cc45-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0cc45-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="0cc45-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0cc45-116">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="0cc45-117">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="0cc45-117">group calendar</span></span> | <span data-ttu-id="0cc45-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cc45-118">Group.ReadWrite.All</span></span> | <span data-ttu-id="0cc45-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cc45-119">Not supported.</span></span> | <span data-ttu-id="0cc45-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cc45-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cc45-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cc45-121">HTTP request</span></span>

<span data-ttu-id="0cc45-122">Atualize as permissões especificadas do calendário de um usuário:</span><span class="sxs-lookup"><span data-stu-id="0cc45-122">Update the specified permissions of a user's calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="0cc45-123">Atualize as permissões especificadas de um calendário de grupo:</span><span class="sxs-lookup"><span data-stu-id="0cc45-123">Update the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="0cc45-124">Atualize as permissões especificadas do calendário do usuário que contém o evento identificado:</span><span class="sxs-lookup"><span data-stu-id="0cc45-124">Update the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0cc45-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0cc45-125">Request headers</span></span>

| <span data-ttu-id="0cc45-126">Nome</span><span class="sxs-lookup"><span data-stu-id="0cc45-126">Name</span></span>       | <span data-ttu-id="0cc45-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cc45-127">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0cc45-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="0cc45-128">Authorization</span></span> | <span data-ttu-id="0cc45-129">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="0cc45-129">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0cc45-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0cc45-130">Request body</span></span>

<span data-ttu-id="0cc45-131">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="0cc45-131">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0cc45-132">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="0cc45-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0cc45-133">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0cc45-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0cc45-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0cc45-134">Property</span></span>     | <span data-ttu-id="0cc45-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cc45-135">Type</span></span>        | <span data-ttu-id="0cc45-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cc45-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0cc45-137">role</span><span class="sxs-lookup"><span data-stu-id="0cc45-137">role</span></span>|[<span data-ttu-id="0cc45-138">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="0cc45-138">calendarRoleType</span></span>](../resources/calendarpermission.md#calendarroletype-values)| <span data-ttu-id="0cc45-139">O nível de permissão a ser alterado para o compartilhamento de calendário ou representante.</span><span class="sxs-lookup"><span data-stu-id="0cc45-139">The permission level to change to for the calendar sharee or delegate.</span></span> |

## <a name="response"></a><span data-ttu-id="0cc45-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cc45-140">Response</span></span>

<span data-ttu-id="0cc45-141">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [calendarPermission](../resources/calendarpermission.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cc45-141">If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0cc45-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0cc45-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0cc45-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cc45-143">Request</span></span>

<span data-ttu-id="0cc45-144">O exemplo a seguir altera o nível de permissão do compartilhamento, Adele, para `write` .</span><span class="sxs-lookup"><span data-stu-id="0cc45-144">The following example changes the permission level of the sharee, Adele, to `write`.</span></span>

# <a name="http"></a>[<span data-ttu-id="0cc45-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cc45-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0cc45-146">C#</span><span class="sxs-lookup"><span data-stu-id="0cc45-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cc45-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cc45-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cc45-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cc45-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0cc45-149">Java</span><span class="sxs-lookup"><span data-stu-id="0cc45-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendarpermission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0cc45-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cc45-150">Response</span></span>

<span data-ttu-id="0cc45-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0cc45-151">The following is an example of the response.</span></span>

> <span data-ttu-id="0cc45-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0cc45-152">**Note:** The response object shown here might be shortened for readability.</span></span>

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


