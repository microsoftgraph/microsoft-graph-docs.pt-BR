---
title: Obter teamsAsyncOperation
description: Obter os detalhes de um teamsAsyncOperation.
author: jecha
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9837cd6af69ee9af06ce2a1ab9aa59f93d0963a9
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210260"
---
# <a name="get-teamsasyncoperation"></a><span data-ttu-id="5ee8f-103">Obter teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="5ee8f-103">Get teamsAsyncOperation</span></span>
<span data-ttu-id="5ee8f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ee8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ee8f-105">Obter a operação [Teams assíncrona especificada](../resources/teamsasyncoperation.md) que foi executado ou está sendo executado em um recurso específico.</span><span class="sxs-lookup"><span data-stu-id="5ee8f-105">Get the specified [Teams async operation](../resources/teamsasyncoperation.md) that ran or is running on a specific resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ee8f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ee8f-106">Permissions</span></span>
<span data-ttu-id="5ee8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ee8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5ee8f-109">As seguintes permissões são para obter a operação em um chat:</span><span class="sxs-lookup"><span data-stu-id="5ee8f-109">The following permissions are for getting the operation on a chat:</span></span>

| <span data-ttu-id="5ee8f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ee8f-110">Permission type</span></span>                        | <span data-ttu-id="5ee8f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ee8f-111">Permissions (from least to most privileged)</span></span>|
| :------------------------------------- | :--------------------------------------------------- |
| <span data-ttu-id="5ee8f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ee8f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ee8f-113">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ee8f-113">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span>|
| <span data-ttu-id="5ee8f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ee8f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ee8f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ee8f-115">Not supported.</span></span> |
| <span data-ttu-id="5ee8f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ee8f-116">Application</span></span>                            | <span data-ttu-id="5ee8f-117">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ee8f-117">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |

> <span data-ttu-id="5ee8f-118">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="5ee8f-118">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="5ee8f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee8f-119">HTTP request</span></span>
<!-- { 
    "blockType": "ignored" 
} 
-->
``` http
GET /chats/{chat-id}/operations/{operation-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ee8f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5ee8f-120">Optional query parameters</span></span>

<span data-ttu-id="5ee8f-121">Este método dá suporte ao `$select` [parâmetro de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee8f-121">This method supports the `$select` [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ee8f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee8f-122">Request headers</span></span>

|<span data-ttu-id="5ee8f-123">Nome</span><span class="sxs-lookup"><span data-stu-id="5ee8f-123">Name</span></span>|<span data-ttu-id="5ee8f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ee8f-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5ee8f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ee8f-125">Authorization</span></span>|<span data-ttu-id="5ee8f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ee8f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ee8f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee8f-128">Request body</span></span>

<span data-ttu-id="5ee8f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ee8f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ee8f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee8f-130">Response</span></span>

<span data-ttu-id="5ee8f-131">Se tiver êxito, isso retornará um código `200 OK` de resposta e um objeto [teamsAsyncOperation](../resources/teamsasyncoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee8f-131">If successful, this returns a `200 OK` response code and a [teamsAsyncOperation](../resources/teamsasyncoperation.md) object in the response body.</span></span>

## <a name="example-get-operation-on-chat"></a><span data-ttu-id="5ee8f-132">Exemplo: Obter operação no chat</span><span class="sxs-lookup"><span data-stu-id="5ee8f-132">Example: Get operation on chat</span></span>

### <a name="request"></a><span data-ttu-id="5ee8f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee8f-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5ee8f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee8f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat_operation"
}
-->
``` http
GET https://graph.microsoft.com/beta/chats/19:c253a29b5f694b55a6baad8e83510af7@thread.v2/operations/2432b57b-0abd-43db-aa7b-16eadd115d34-e88ae9aa-887e-4972-ac3e-bd578e38232e-cf58835e-43f0-4fc1-825e-5de55630e7e4
```
# <a name="c"></a>[<span data-ttu-id="5ee8f-135">C#</span><span class="sxs-lookup"><span data-stu-id="5ee8f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-operation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ee8f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ee8f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-operation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ee8f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ee8f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-operation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ee8f-138">Java</span><span class="sxs-lookup"><span data-stu-id="5ee8f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chat-operation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5ee8f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee8f-139">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsAsyncOperation"
}
-->
``` http
HTTP/1.1 202 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ac253a29b5f694b55a6baad8e83510af7%40thread.v2')/operations/$entity",
    "id": "2432b57b-0abd-43db-aa7b-16eadd115d34-e88ae9aa-887e-4972-ac3e-bd578e38232e-cf58835e-43f0-4fc1-825e-5de55630e7e4",
    "operationType": "createChat",
    "createdDateTime": "2021-05-27T21:23:41.9085453Z",
    "status": "succeeded",
    "lastActionDateTime": "2021-05-27T21:23:45.1899277Z",
    "attemptsCount": 1,
    "targetResourceId": "19:c253a29b5f694b55a6baad8e83510af7@thread.v2",
    "targetResourceLocation": "/chats('19:c253a29b5f694b55a6baad8e83510af7@thread.v2')",
    "values": "{\"appIds\":[\"1542629c-01b3-4a6d-8f76-1938b779e48d\"]}",
    "error": null
}
```
