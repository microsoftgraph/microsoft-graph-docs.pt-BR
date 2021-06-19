---
title: Listar operações em um chat
description: Recupere operações em um chat.
author: jecha
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fce94d591d6d1bde1e15f78674b18623ba80cb33
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031435"
---
# <a name="list-operations-on-a-chat"></a><span data-ttu-id="8896c-103">Listar operações em um chat</span><span class="sxs-lookup"><span data-stu-id="8896c-103">List operations on a chat</span></span>
<span data-ttu-id="8896c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8896c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8896c-105">Listar [todas Teams assíncronas](../resources/teamsasyncoperation.md) que executam ou estão sendo executados no [chat especificado.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="8896c-105">List all [Teams async operations](../resources/teamsasyncoperation.md) that ran or are running on the specified [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8896c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8896c-106">Permissions</span></span>
<span data-ttu-id="8896c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8896c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8896c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8896c-109">Permission type</span></span>                        | <span data-ttu-id="8896c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8896c-110">Permissions (from least to most privileged)</span></span>|
| :------------------------------------- | :--------------------------------------------------- |
| <span data-ttu-id="8896c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8896c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8896c-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8896c-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span>|
| <span data-ttu-id="8896c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8896c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8896c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8896c-114">Not supported.</span></span> |
| <span data-ttu-id="8896c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8896c-115">Application</span></span>                            | <span data-ttu-id="8896c-116">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8896c-116">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |

> <span data-ttu-id="8896c-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="8896c-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="8896c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8896c-118">HTTP request</span></span>
<!-- { 
    "blockType": "ignored" 
} 
-->
``` http
GET /chats/{chat-id}/operations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8896c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8896c-119">Optional query parameters</span></span>

<span data-ttu-id="8896c-120">Este método dá suporte `$filter` aos `$select` parâmetros de consulta , , e OData para `$top` ajudar a personalizar a `$skip` [](/graph/query-parameters) resposta.</span><span class="sxs-lookup"><span data-stu-id="8896c-120">This method supports the `$filter`, `$select`, `$top`, and `$skip` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8896c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8896c-121">Request headers</span></span>

|<span data-ttu-id="8896c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8896c-122">Name</span></span>|<span data-ttu-id="8896c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8896c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8896c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8896c-124">Authorization</span></span>|<span data-ttu-id="8896c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8896c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8896c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8896c-127">Request body</span></span>

<span data-ttu-id="8896c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8896c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8896c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8896c-129">Response</span></span>

<span data-ttu-id="8896c-130">Se tiver êxito, isso retornará um código de resposta e uma `200 OK` coleção de [objetos teamsAsyncOperation](../resources/teamsasyncoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8896c-130">If successful, this returns a `200 OK` response code and a collection of [teamsAsyncOperation](../resources/teamsasyncoperation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8896c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8896c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8896c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8896c-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_chat_operations"
}
-->
``` http
GET https://graph.microsoft.com/beta/chats/19:c253a29b5f694b55a6baad8e83510af7@thread.v2/operations
```

---

### <a name="response"></a><span data-ttu-id="8896c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8896c-133">Response</span></span>
><span data-ttu-id="8896c-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8896c-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAsyncOperation",
  "isCollection": true
}
-->
``` http
HTTP/1.1 202 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ac253a29b5f694b55a6baad8e83510af7%40thread.v2')/operations",
    "@odata.count": 1,
    "value": [
        {
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
    ]
}
```
