---
title: Obter calendarPermission
description: Obtenha as propriedades e os relacionamentos do objeto calendarpermission.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d319d45ce3ee50f113e711729bc9c0ae71081e6a
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229079"
---
# <a name="get-calendarpermission"></a><span data-ttu-id="1b842-103">Obter calendarPermission</span><span class="sxs-lookup"><span data-stu-id="1b842-103">Get calendarPermission</span></span>

<span data-ttu-id="1b842-104">Obter o objeto Permissions especificado de um usuário ou grupo calendário que foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="1b842-104">Get the specified permissions object of a user or group calendar that has been shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b842-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b842-105">Permissions</span></span>

<span data-ttu-id="1b842-106">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="1b842-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="1b842-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b842-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1b842-108">Calendário</span><span class="sxs-lookup"><span data-stu-id="1b842-108">Calendar</span></span> | <span data-ttu-id="1b842-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b842-109">Delegated (work or school account)</span></span> | <span data-ttu-id="1b842-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b842-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b842-111">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b842-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="1b842-112">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="1b842-112">user calendar</span></span> | <span data-ttu-id="1b842-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b842-113">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="1b842-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b842-114">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="1b842-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b842-115">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="1b842-116">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="1b842-116">group calendar</span></span> | <span data-ttu-id="1b842-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b842-117">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="1b842-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b842-118">Not supported.</span></span> | <span data-ttu-id="1b842-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b842-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b842-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b842-120">HTTP request</span></span>

<span data-ttu-id="1b842-121">Obter as permissões especificadas do calendário principal de um usuário:</span><span class="sxs-lookup"><span data-stu-id="1b842-121">Get the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="1b842-122">Obter as permissões especificadas de um calendário de Grupo:</span><span class="sxs-lookup"><span data-stu-id="1b842-122">Get the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="1b842-123">Obtenha as permissões especificadas do calendário do usuário que contém o evento identificado:</span><span class="sxs-lookup"><span data-stu-id="1b842-123">Get the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1b842-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1b842-124">Optional query parameters</span></span>

<span data-ttu-id="1b842-125">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1b842-125">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1b842-126">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1b842-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b842-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b842-127">Request headers</span></span>

| <span data-ttu-id="1b842-128">Nome</span><span class="sxs-lookup"><span data-stu-id="1b842-128">Name</span></span>      |<span data-ttu-id="1b842-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b842-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1b842-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b842-130">Authorization</span></span> | <span data-ttu-id="1b842-131">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="1b842-131">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b842-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b842-132">Request body</span></span>

<span data-ttu-id="1b842-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1b842-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b842-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b842-134">Response</span></span>

<span data-ttu-id="1b842-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [calendarPermission](../resources/calendarpermission.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b842-135">If successful, this method returns a `200 OK` response code and the requested [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b842-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1b842-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1b842-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b842-137">Request</span></span>

<span data-ttu-id="1b842-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b842-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendarpermission"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/calendar/calendarPermissions/{id}
```

### <a name="response"></a><span data-ttu-id="1b842-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b842-139">Response</span></span>

<span data-ttu-id="1b842-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1b842-140">The following is an example of the response.</span></span>

> <span data-ttu-id="1b842-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b842-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
