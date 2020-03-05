---
title: Obter calendarPermission
description: Obtenha as propriedades e os relacionamentos do objeto calendarpermission.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8481cecf256d9cd85f9c444f0550ea7c43d37d0b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440896"
---
# <a name="get-calendarpermission"></a><span data-ttu-id="41282-103">Obter calendarPermission</span><span class="sxs-lookup"><span data-stu-id="41282-103">Get calendarPermission</span></span>

<span data-ttu-id="41282-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="41282-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41282-105">Obter o objeto Permissions especificado de um usuário ou grupo calendário que foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="41282-105">Get the specified permissions object of a user or group calendar that has been shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="41282-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="41282-106">Permissions</span></span>

<span data-ttu-id="41282-107">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="41282-107">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="41282-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41282-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41282-109">Calendário</span><span class="sxs-lookup"><span data-stu-id="41282-109">Calendar</span></span> | <span data-ttu-id="41282-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41282-110">Delegated (work or school account)</span></span> | <span data-ttu-id="41282-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41282-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41282-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41282-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="41282-113">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="41282-113">user calendar</span></span> | <span data-ttu-id="41282-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41282-114">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="41282-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41282-115">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="41282-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41282-116">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="41282-117">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="41282-117">group calendar</span></span> | <span data-ttu-id="41282-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41282-118">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="41282-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41282-119">Not supported.</span></span> | <span data-ttu-id="41282-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41282-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="41282-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41282-121">HTTP request</span></span>

<span data-ttu-id="41282-122">Obter as permissões especificadas do calendário principal de um usuário:</span><span class="sxs-lookup"><span data-stu-id="41282-122">Get the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="41282-123">Obter as permissões especificadas de um calendário de Grupo:</span><span class="sxs-lookup"><span data-stu-id="41282-123">Get the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="41282-124">Obtenha as permissões especificadas do calendário do usuário que contém o evento identificado:</span><span class="sxs-lookup"><span data-stu-id="41282-124">Get the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41282-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="41282-125">Optional query parameters</span></span>

<span data-ttu-id="41282-126">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="41282-126">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="41282-127">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="41282-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="41282-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41282-128">Request headers</span></span>

| <span data-ttu-id="41282-129">Nome</span><span class="sxs-lookup"><span data-stu-id="41282-129">Name</span></span>      |<span data-ttu-id="41282-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="41282-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="41282-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="41282-131">Authorization</span></span> | <span data-ttu-id="41282-132">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="41282-132">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="41282-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41282-133">Request body</span></span>

<span data-ttu-id="41282-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41282-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41282-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="41282-135">Response</span></span>

<span data-ttu-id="41282-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [calendarPermission](../resources/calendarpermission.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41282-136">If successful, this method returns a `200 OK` response code and the requested [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="41282-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="41282-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="41282-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41282-138">Request</span></span>

<span data-ttu-id="41282-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="41282-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="41282-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="41282-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarpermission"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
```
# <a name="c"></a>[<span data-ttu-id="41282-141">C#</span><span class="sxs-lookup"><span data-stu-id="41282-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41282-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41282-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41282-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41282-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="41282-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="41282-144">Response</span></span>

<span data-ttu-id="41282-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41282-145">The following is an example of the response.</span></span>

> <span data-ttu-id="41282-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41282-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
