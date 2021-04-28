---
title: Atualizar calendarpermission
description: Atualize as propriedades do objeto calendarpermission.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a91c174a9830494d6e44463aaaea8217c57849a8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051610"
---
# <a name="update-calendarpermission"></a><span data-ttu-id="0d140-103">Atualizar calendarPermission</span><span class="sxs-lookup"><span data-stu-id="0d140-103">Update calendarPermission</span></span>

<span data-ttu-id="0d140-104">Atualize as permissões atribuídas a um compartilhamento ou representante existente, por meio do [objeto calendarPermission](../resources/calendarpermission.md) correspondente para um calendário.</span><span class="sxs-lookup"><span data-stu-id="0d140-104">Update the permissions assigned to an existing sharee or delegate, through the corresponding [calendarPermission](../resources/calendarpermission.md) object for a calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d140-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d140-105">Permissions</span></span>

<span data-ttu-id="0d140-106">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="0d140-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="0d140-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d140-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d140-108">Calendário</span><span class="sxs-lookup"><span data-stu-id="0d140-108">Calendar</span></span> | <span data-ttu-id="0d140-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d140-109">Delegated (work or school account)</span></span> | <span data-ttu-id="0d140-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d140-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d140-111">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d140-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="0d140-112">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="0d140-112">user calendar</span></span> | <span data-ttu-id="0d140-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d140-113">Calendars.ReadWrite</span></span> | <span data-ttu-id="0d140-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d140-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="0d140-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d140-115">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="0d140-116">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="0d140-116">group calendar</span></span> | <span data-ttu-id="0d140-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d140-117">Group.ReadWrite.All</span></span> | <span data-ttu-id="0d140-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d140-118">Not supported.</span></span> | <span data-ttu-id="0d140-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d140-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d140-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d140-120">HTTP request</span></span>

<span data-ttu-id="0d140-121">Atualize as permissões especificadas do calendário de um usuário:</span><span class="sxs-lookup"><span data-stu-id="0d140-121">Update the specified permissions of a user's calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="0d140-122">Atualize as permissões especificadas de um calendário de grupo:</span><span class="sxs-lookup"><span data-stu-id="0d140-122">Update the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="0d140-123">Atualize as permissões especificadas do calendário do usuário que contém o evento identificado:</span><span class="sxs-lookup"><span data-stu-id="0d140-123">Update the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0d140-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d140-124">Request headers</span></span>

| <span data-ttu-id="0d140-125">Nome</span><span class="sxs-lookup"><span data-stu-id="0d140-125">Name</span></span>       | <span data-ttu-id="0d140-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d140-126">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0d140-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d140-127">Authorization</span></span> | <span data-ttu-id="0d140-128">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="0d140-128">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d140-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d140-129">Request body</span></span>

<span data-ttu-id="0d140-130">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="0d140-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0d140-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="0d140-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0d140-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0d140-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0d140-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d140-133">Property</span></span>     | <span data-ttu-id="0d140-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d140-134">Type</span></span>        | <span data-ttu-id="0d140-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d140-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0d140-136">role</span><span class="sxs-lookup"><span data-stu-id="0d140-136">role</span></span>|[<span data-ttu-id="0d140-137">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="0d140-137">calendarRoleType</span></span>](../resources/calendarpermission.md#calendarroletype-values)| <span data-ttu-id="0d140-138">O nível de permissão a ser alterado para o compartilhamento de calendário ou representante.</span><span class="sxs-lookup"><span data-stu-id="0d140-138">The permission level to change to for the calendar sharee or delegate.</span></span> |

## <a name="response"></a><span data-ttu-id="0d140-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d140-139">Response</span></span>

<span data-ttu-id="0d140-140">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [calendarPermission](../resources/calendarpermission.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d140-140">If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d140-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0d140-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0d140-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d140-142">Request</span></span>

<span data-ttu-id="0d140-143">O exemplo a seguir altera o nível de permissão do compartilhamento, Adele, para `write` .</span><span class="sxs-lookup"><span data-stu-id="0d140-143">The following example changes the permission level of the sharee, Adele, to `write`.</span></span>


# <a name="http"></a>[<span data-ttu-id="0d140-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d140-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["RGVmYXVsdA=="],
  "name": "update_calendarpermission"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/users/{id}/calendar/calendarPermissions/RGVmYXVsdA==
Content-type: application/json

{
  "role": "write"
}
```
# <a name="c"></a>[<span data-ttu-id="0d140-145">C#</span><span class="sxs-lookup"><span data-stu-id="0d140-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d140-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d140-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d140-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d140-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d140-148">Java</span><span class="sxs-lookup"><span data-stu-id="0d140-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendarpermission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0d140-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d140-149">Response</span></span>

<span data-ttu-id="0d140-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0d140-150">The following is an example of the response.</span></span>

> <span data-ttu-id="0d140-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0d140-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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

