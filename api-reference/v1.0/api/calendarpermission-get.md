---
title: Obter calendarPermission
description: Obtenha as propriedades e os relacionamentos do objeto calendarpermission.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ab5fefbb2b88511d6b40aaf80772f582975eec02
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070300"
---
# <a name="get-calendarpermission"></a><span data-ttu-id="14f71-103">Obter calendarPermission</span><span class="sxs-lookup"><span data-stu-id="14f71-103">Get calendarPermission</span></span>

<span data-ttu-id="14f71-104">Obter o objeto Permissions especificado de um usuário ou grupo calendário que foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="14f71-104">Get the specified permissions object of a user or group calendar that has been shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="14f71-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="14f71-105">Permissions</span></span>

<span data-ttu-id="14f71-106">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="14f71-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="14f71-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14f71-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14f71-108">Calendário</span><span class="sxs-lookup"><span data-stu-id="14f71-108">Calendar</span></span> | <span data-ttu-id="14f71-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14f71-109">Delegated (work or school account)</span></span> | <span data-ttu-id="14f71-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14f71-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14f71-111">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14f71-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="14f71-112">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="14f71-112">user calendar</span></span> | <span data-ttu-id="14f71-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14f71-113">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="14f71-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14f71-114">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="14f71-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14f71-115">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="14f71-116">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="14f71-116">group calendar</span></span> | <span data-ttu-id="14f71-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14f71-117">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="14f71-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14f71-118">Not supported.</span></span> | <span data-ttu-id="14f71-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14f71-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="14f71-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14f71-120">HTTP request</span></span>

<span data-ttu-id="14f71-121">Obter as permissões especificadas do calendário principal de um usuário:</span><span class="sxs-lookup"><span data-stu-id="14f71-121">Get the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="14f71-122">Obter as permissões especificadas de um calendário de Grupo:</span><span class="sxs-lookup"><span data-stu-id="14f71-122">Get the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="14f71-123">Obtenha as permissões especificadas do calendário do usuário que contém o evento identificado:</span><span class="sxs-lookup"><span data-stu-id="14f71-123">Get the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14f71-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="14f71-124">Optional query parameters</span></span>

<span data-ttu-id="14f71-125">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="14f71-125">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="14f71-126">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="14f71-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="14f71-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14f71-127">Request headers</span></span>

| <span data-ttu-id="14f71-128">Nome</span><span class="sxs-lookup"><span data-stu-id="14f71-128">Name</span></span>      |<span data-ttu-id="14f71-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="14f71-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="14f71-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="14f71-130">Authorization</span></span> | <span data-ttu-id="14f71-131">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="14f71-131">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="14f71-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14f71-132">Request body</span></span>

<span data-ttu-id="14f71-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14f71-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14f71-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="14f71-134">Response</span></span>

<span data-ttu-id="14f71-135">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [calendarPermission](../resources/calendarpermission.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14f71-135">If successful, this method returns a `200 OK` response code and the requested [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="14f71-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="14f71-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="14f71-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14f71-137">Request</span></span>

<span data-ttu-id="14f71-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14f71-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="14f71-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="14f71-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarpermission"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/calendar/calendarPermissions/{id}
```
# <a name="c"></a>[<span data-ttu-id="14f71-140">C#</span><span class="sxs-lookup"><span data-stu-id="14f71-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14f71-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14f71-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14f71-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14f71-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14f71-143">Java</span><span class="sxs-lookup"><span data-stu-id="14f71-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarpermission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="14f71-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="14f71-144">Response</span></span>

<span data-ttu-id="14f71-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14f71-145">The following is an example of the response.</span></span>

> <span data-ttu-id="14f71-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14f71-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

