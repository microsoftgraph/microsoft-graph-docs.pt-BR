---
title: Obter calendarPermission
description: Obter as propriedades e as relações do objeto calendarpermission.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e6286ec91e3ef75cf9ae5d35992a8794392d2ede
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047683"
---
# <a name="get-calendarpermission"></a><span data-ttu-id="1978b-103">Obter calendarPermission</span><span class="sxs-lookup"><span data-stu-id="1978b-103">Get calendarPermission</span></span>

<span data-ttu-id="1978b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1978b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1978b-105">Obter o objeto de permissões especificado de um usuário ou calendário de grupo que foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="1978b-105">Get the specified permissions object of a user or group calendar that has been shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="1978b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1978b-106">Permissions</span></span>

<span data-ttu-id="1978b-107">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="1978b-107">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="1978b-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1978b-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1978b-109">Calendário</span><span class="sxs-lookup"><span data-stu-id="1978b-109">Calendar</span></span> | <span data-ttu-id="1978b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1978b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1978b-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1978b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1978b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1978b-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="1978b-113">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="1978b-113">user calendar</span></span> | <span data-ttu-id="1978b-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1978b-114">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="1978b-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1978b-115">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="1978b-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1978b-116">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="1978b-117">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="1978b-117">group calendar</span></span> | <span data-ttu-id="1978b-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1978b-118">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="1978b-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1978b-119">Not supported.</span></span> | <span data-ttu-id="1978b-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1978b-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1978b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1978b-121">HTTP request</span></span>

<span data-ttu-id="1978b-122">Obter as permissões especificadas do calendário principal de um usuário:</span><span class="sxs-lookup"><span data-stu-id="1978b-122">Get the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="1978b-123">Obter as permissões especificadas de um calendário de grupo:</span><span class="sxs-lookup"><span data-stu-id="1978b-123">Get the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="1978b-124">Obter as permissões especificadas do calendário do usuário que contém o evento identificado:</span><span class="sxs-lookup"><span data-stu-id="1978b-124">Get the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1978b-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1978b-125">Optional query parameters</span></span>

<span data-ttu-id="1978b-126">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1978b-126">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1978b-127">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1978b-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1978b-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1978b-128">Request headers</span></span>

| <span data-ttu-id="1978b-129">Nome</span><span class="sxs-lookup"><span data-stu-id="1978b-129">Name</span></span>      |<span data-ttu-id="1978b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1978b-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1978b-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="1978b-131">Authorization</span></span> | <span data-ttu-id="1978b-132">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="1978b-132">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1978b-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1978b-133">Request body</span></span>

<span data-ttu-id="1978b-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1978b-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1978b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1978b-135">Response</span></span>

<span data-ttu-id="1978b-136">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [calendarPermission](../resources/calendarpermission.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1978b-136">If successful, this method returns a `200 OK` response code and the requested [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1978b-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1978b-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1978b-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1978b-138">Request</span></span>

<span data-ttu-id="1978b-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1978b-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1978b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="1978b-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarpermission"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
```
# <a name="c"></a>[<span data-ttu-id="1978b-141">C#</span><span class="sxs-lookup"><span data-stu-id="1978b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1978b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1978b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1978b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1978b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1978b-144">Java</span><span class="sxs-lookup"><span data-stu-id="1978b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarpermission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1978b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1978b-145">Response</span></span>

<span data-ttu-id="1978b-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1978b-146">The following is an example of the response.</span></span>

> <span data-ttu-id="1978b-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1978b-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "description": "Get calendarPermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


