---
title: 'presença: clearPresence'
description: Desmarcar as informações de presença para a sessão de presença do aplicativo do usuário.
author: jsandoval-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 02140f99accf36bfac156996e83bd75de2bb3b19
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107790"
---
# <a name="presence-clearpresence"></a><span data-ttu-id="f156e-103">presença: clearPresence</span><span class="sxs-lookup"><span data-stu-id="f156e-103">presence: clearPresence</span></span>

<span data-ttu-id="f156e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f156e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f156e-105">Desmarcar a sessão de presença do aplicativo para um usuário.</span><span class="sxs-lookup"><span data-stu-id="f156e-105">Clear the application's presence session for a user.</span></span> <span data-ttu-id="f156e-106">Se for a única sessão de presença do usuário, a presença do usuário mudará para `Offline/Offline` .</span><span class="sxs-lookup"><span data-stu-id="f156e-106">If it is the user's only presence session, the user's presence will change to `Offline/Offline`.</span></span>

<span data-ttu-id="f156e-107">Para obter detalhes sobre sessões de presença, [consulte presence: setPresence](presence-setpresence.md#presence-sessions).</span><span class="sxs-lookup"><span data-stu-id="f156e-107">For details about presences sessions, see [presence: setPresence](presence-setpresence.md#presence-sessions).</span></span>

## <a name="permissions"></a><span data-ttu-id="f156e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f156e-108">Permissions</span></span>
<span data-ttu-id="f156e-109">A permissão a seguir é necessária para chamar a API.</span><span class="sxs-lookup"><span data-stu-id="f156e-109">The following permission is required to call the API.</span></span> <span data-ttu-id="f156e-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f156e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f156e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f156e-111">Permission type</span></span>                        | <span data-ttu-id="f156e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f156e-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f156e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f156e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f156e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f156e-114">Not Supported.</span></span>                              |
| <span data-ttu-id="f156e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f156e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f156e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f156e-116">Not Supported.</span></span>                              |
| <span data-ttu-id="f156e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f156e-117">Application</span></span>                            | <span data-ttu-id="f156e-118">Presence.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f156e-118">Presence.ReadWrite.All</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="f156e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f156e-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/presence/clearPresence
```

## <a name="request-headers"></a><span data-ttu-id="f156e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f156e-120">Request headers</span></span>
| <span data-ttu-id="f156e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f156e-121">Name</span></span>          | <span data-ttu-id="f156e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f156e-122">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="f156e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f156e-123">Authorization</span></span> | <span data-ttu-id="f156e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f156e-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="f156e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f156e-126">Content-Type</span></span>  | <span data-ttu-id="f156e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f156e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f156e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f156e-129">Request body</span></span>

<span data-ttu-id="f156e-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f156e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f156e-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f156e-131">Parameter</span></span> | <span data-ttu-id="f156e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f156e-132">Type</span></span>   | <span data-ttu-id="f156e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f156e-133">Description</span></span>                                   |
| :-------- | :----- | :-------------------------------------------- |
| <span data-ttu-id="f156e-134">sessionId</span><span class="sxs-lookup"><span data-stu-id="f156e-134">sessionId</span></span> | <span data-ttu-id="f156e-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f156e-135">string</span></span> | <span data-ttu-id="f156e-136">A ID da sessão de presença do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f156e-136">The ID of the application's presence session.</span></span> |


> [!IMPORTANT]
> 
> <span data-ttu-id="f156e-137">Forneça a ID do aplicativo como `sessionId` na solicitação.</span><span class="sxs-lookup"><span data-stu-id="f156e-137">Provide the ID of the application as `sessionId` in the request.</span></span>

## <a name="response"></a><span data-ttu-id="f156e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f156e-138">Response</span></span>
<span data-ttu-id="f156e-139">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="f156e-139">If successful, this method returns a `200 OK` response code.</span></span>

<span data-ttu-id="f156e-140">Se a sessão de presença não existir, este método retornará um `404 NotFound` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="f156e-140">If the presence session doesn't exist, this method returns a `404 NotFound` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f156e-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f156e-141">Examples</span></span>
<span data-ttu-id="f156e-142">A solicitação a seguir mostra o aplicativo com ID `22553876-f5ab-4529-bffb-cfe50aa89f87` que limpa sua sessão de presença para o usuário `fa8bf3dc-eca7-46b7-bad1-db199b62afc3` .</span><span class="sxs-lookup"><span data-stu-id="f156e-142">The following request shows the application with ID `22553876-f5ab-4529-bffb-cfe50aa89f87` that clears its presence session for user `fa8bf3dc-eca7-46b7-bad1-db199b62afc3`.</span></span>

### <a name="request"></a><span data-ttu-id="f156e-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f156e-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "clear--presence"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/clearPresence
Content-Type: application/json

{
  "sessionId": "22553876-f5ab-4529-bffb-cfe50aa89f87"
}
```

### <a name="response"></a><span data-ttu-id="f156e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f156e-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
