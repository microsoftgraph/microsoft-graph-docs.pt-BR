---
title: Criar ReuniãoOnline
description: Crie uma reunião online em nome de um usuário específico no corpo da solicitação.
author: VinodRavichandran
localization_priority: Priority
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 96b52984c199c1f66688752c34ebca4094cd1d39
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868405"
---
# <a name="create-onlinemeeting"></a><span data-ttu-id="1a90d-103">Criar ReuniãoOnline</span><span class="sxs-lookup"><span data-stu-id="1a90d-103">Create onlineMeeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a90d-104">Crie uma reunião online em nome de um usuário usando a ID de objeto (OID) no token de usuário.</span><span class="sxs-lookup"><span data-stu-id="1a90d-104">Create an online meeting on behalf of a user by using the Object Id (oid) in the user token.</span></span>

> <span data-ttu-id="1a90d-105">**Observação**: a reunião não é exibida no calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="1a90d-105">**Note**: The meeting does not show up on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a90d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a90d-106">Permissions</span></span>
<span data-ttu-id="1a90d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a90d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a90d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a90d-109">Permission type</span></span>                        | <span data-ttu-id="1a90d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a90d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1a90d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a90d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a90d-112">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a90d-112">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="1a90d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a90d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a90d-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="1a90d-114">Not Supported</span></span>                               |
| <span data-ttu-id="1a90d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a90d-115">Application</span></span>                            | <span data-ttu-id="1a90d-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="1a90d-116">Not Supported</span></span>                |
## <a name="http-request"></a><span data-ttu-id="1a90d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a90d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
POST /communications/onlineMeetings
POST /me/onlineMeetings
```
> <span data-ttu-id="1a90d-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="1a90d-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="1a90d-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="1a90d-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a90d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a90d-120">Request headers</span></span>
| <span data-ttu-id="1a90d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1a90d-121">Name</span></span>          | <span data-ttu-id="1a90d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a90d-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1a90d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a90d-123">Authorization</span></span> | <span data-ttu-id="1a90d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a90d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1a90d-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="1a90d-126">Content-type</span></span>  | <span data-ttu-id="1a90d-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a90d-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a90d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a90d-129">Request body</span></span>
<span data-ttu-id="1a90d-130">No corpo da solicitação, forneça uma representação JSON de um objeto [onlineMeeting](../resources/onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="1a90d-130">In the request body, supply a JSON representation of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1a90d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a90d-131">Response</span></span>
<span data-ttu-id="1a90d-132">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a90d-132">If successful, this method returns a `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a90d-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1a90d-133">Examples</span></span>

### <a name="example-1-create-an-online-meeting-with-application-token"></a><span data-ttu-id="1a90d-134">Exemplo 1: criar uma reunião online com o token do aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a90d-134">Example 1: Create an online meeting with application token</span></span>

#### <a name="request"></a><span data-ttu-id="1a90d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a90d-135">Request</span></span>

> [!Note]
> <span data-ttu-id="1a90d-136">A criação de uma reunião online usando o token do aplicativo foi preterida.</span><span class="sxs-lookup"><span data-stu-id="1a90d-136">Note: Online meeting creation using the application token is deprecated.</span></span> <span data-ttu-id="1a90d-137">Use o caminho /me com um token de usuário para criar reuniões online.</span><span class="sxs-lookup"><span data-stu-id="1a90d-137">Use the /me path with a user token to create online meetings going forward.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1a90d-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a90d-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-onlinemeeting-app-token"
}-->
```http
POST https://graph.microsoft.com/beta/communications/onlineMeetings
Content-Type: application/json

{
  "startDateTime":"2019-09-09T14:33:30.8546353-07:00",
  "endDateTime":"2019-09-09T15:03:30.8566356-07:00",
  "subject":"Application Token Meeting",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f"
        }
      }
    }
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1a90d-139">C#</span><span class="sxs-lookup"><span data-stu-id="1a90d-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onlinemeeting-app-token-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a90d-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a90d-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onlinemeeting-app-token-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1a90d-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a90d-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onlinemeeting-app-token-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="1a90d-142">No corpo da solicitação, forneça uma representação JSON do objeto [onlineMeeting](../resources/onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="1a90d-142">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="1a90d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a90d-143">Response</span></span>

><span data-ttu-id="1a90d-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1a90d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "autoAdmittedUsers": "everyone",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "2425999",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "id": "550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "upn": "upn-value"
    }
  },
  "subject": "Application Token Meeting"
}
```

### <a name="example-2-create-an-online-meeting-with-user-token"></a><span data-ttu-id="1a90d-146">Exemplo 2: criar uma reunião online com o token de usuário</span><span class="sxs-lookup"><span data-stu-id="1a90d-146">Example 2: Create an online meeting with user token</span></span>

#### <a name="request"></a><span data-ttu-id="1a90d-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a90d-147">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1a90d-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a90d-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-onlinemeeting-user-token"
}-->
```http
POST https://graph.microsoft.com/beta/me/onlineMeetings
Content-Type: application/json

{
  "startDateTime":"2019-07-12T14:30:34.2444915-07:00",
  "endDateTime":"2019-07-12T15:00:34.2464912-07:00",
  "subject":"User Token Meeting"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1a90d-149">C#</span><span class="sxs-lookup"><span data-stu-id="1a90d-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onlinemeeting-user-token-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a90d-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a90d-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onlinemeeting-user-token-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1a90d-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a90d-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onlinemeeting-user-token-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1a90d-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a90d-152">Response</span></span>
><span data-ttu-id="1a90d-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1a90d-153">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('f4053f86-17cc-42e7-85f4-f0389ac980d6')/onlineMeetings/$entity",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "2425999",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "id": "550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "upn": "upn-value"
    }
  },
  "subject": "User Token Meeting"
}
```

### <a name="example-3-create-an-online-meeting-in-a-microsoft-teams-channel-with-a-user-token"></a><span data-ttu-id="1a90d-154">Exemplo 3: criar uma reunião online em um Canal do Microsoft Teams com um token de usuário</span><span class="sxs-lookup"><span data-stu-id="1a90d-154">Example 3: Create an online meeting in a Microsoft Teams Channel with a user token</span></span>

#### <a name="request"></a><span data-ttu-id="1a90d-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a90d-155">Request</span></span>
><span data-ttu-id="1a90d-156">**Observação:**: a ID de objeto do token do usuário aprovada deve ser um membro do canal representado pelo threadid no conteúdo.</span><span class="sxs-lookup"><span data-stu-id="1a90d-156">**Note:** The Object ID of the user token passed should be a member of the channel represented by threadid in the payload.</span></span>

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings
Content-Type: application/json

{
  "startDateTime":"2019-07-12T14:30:34.2444915-07:00",
  "endDateTime":"2019-07-12T15:00:34.2464912-07:00",
  "subject":"User meeting in Microsoft Teams channel.",
  "chatInfo": {
    "threadId":"19%3A3b52398f3c524556894b776357c1dd79%40thread.skype"
  }
}
```
#### <a name="response"></a><span data-ttu-id="1a90d-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a90d-157">Response</span></span>

><span data-ttu-id="1a90d-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1a90d-158">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "example",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('f4053f86-17cc-42e7-85f4-f0389ac980d6')/onlineMeetings/$entity",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "2425999",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "chatInfo": {
    "threadId": "19%3A3b52398f3c524556894b776357c1dd79%40thread.skype",
    "messageId": "1563302249053",
    "replyChainMessageId": null
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "id": "550fae72-d251-43ec-868c-373732c2704f_19%3A3b52398f3c524556894b776357c1dd79%40thread.skype",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "upn": "upn-value"
    }
  },
  "subject": "User meeting in Microsoft Teams channel."
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
