---
title: Criar ReuniãoOnline
description: Crie uma reunião online em nome de um usuário específico no corpo da solicitação.
author: ananmishr
localization_priority: Priority
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: f3195f55532713ee4bc359623b8fed241b799f3f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441470"
---
# <a name="create-onlinemeeting"></a><span data-ttu-id="491fe-103">Criar ReuniãoOnline</span><span class="sxs-lookup"><span data-stu-id="491fe-103">Create onlineMeeting</span></span>

<span data-ttu-id="491fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="491fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="491fe-105">Crie uma reunião online em nome de um usuário usando a ID de objeto (OID) no token de usuário.</span><span class="sxs-lookup"><span data-stu-id="491fe-105">Create an online meeting on behalf of a user by using the object ID (OID) in the user token.</span></span>

> <span data-ttu-id="491fe-106">**Observação**: a reunião não é exibida no calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="491fe-106">**Note**: The meeting does not show up on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="491fe-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="491fe-107">Permissions</span></span>
<span data-ttu-id="491fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="491fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="491fe-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="491fe-110">Permission type</span></span>                        | <span data-ttu-id="491fe-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="491fe-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="491fe-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="491fe-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="491fe-113">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="491fe-113">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="491fe-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="491fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="491fe-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="491fe-115">Not Supported</span></span>                               |
| <span data-ttu-id="491fe-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="491fe-116">Application</span></span>                            | <span data-ttu-id="491fe-117">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="491fe-117">OnlineMeetings.ReadWrite.All\*</span></span>  |

> <span data-ttu-id="491fe-118">\* **Observação:** as permissões de aplicativo foram preteridas e serão removidas em abril de 2020.</span><span class="sxs-lookup"><span data-stu-id="491fe-118">\* **Note:** Application permissions are deprecated and will be removed in April 2020.</span></span>

## <a name="http-request"></a><span data-ttu-id="491fe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="491fe-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
POST /communications/onlineMeetings
POST /me/onlineMeetings
```
> <span data-ttu-id="491fe-120">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="491fe-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="491fe-121">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="491fe-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="491fe-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="491fe-122">Request headers</span></span>
| <span data-ttu-id="491fe-123">Nome</span><span class="sxs-lookup"><span data-stu-id="491fe-123">Name</span></span>          | <span data-ttu-id="491fe-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="491fe-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="491fe-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="491fe-125">Authorization</span></span> | <span data-ttu-id="491fe-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="491fe-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="491fe-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="491fe-128">Content-type</span></span>  | <span data-ttu-id="491fe-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="491fe-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="491fe-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="491fe-131">Request body</span></span>
<span data-ttu-id="491fe-132">No corpo da solicitação, forneça uma representação JSON de um objeto [onlineMeeting](../resources/onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="491fe-132">In the request body, supply a JSON representation of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="491fe-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="491fe-133">Response</span></span>
<span data-ttu-id="491fe-134">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="491fe-134">If successful, this method returns a `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="491fe-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="491fe-135">Examples</span></span>

### <a name="example-1-create-an-online-meeting-with-application-token"></a><span data-ttu-id="491fe-136">Exemplo 1: criar uma reunião online com o token do aplicativo</span><span class="sxs-lookup"><span data-stu-id="491fe-136">Example 1: Create an online meeting with application token</span></span>

#### <a name="request"></a><span data-ttu-id="491fe-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="491fe-137">Request</span></span>

> [!Note]
> <span data-ttu-id="491fe-138">A criação de reuniões online usando um token de aplicativo foi descontinuada e o suporte será removido em abril de 2020.</span><span class="sxs-lookup"><span data-stu-id="491fe-138">Online meeting creation using an application token is deprecated and support will be removed in April 2020.</span></span> <span data-ttu-id="491fe-139">Use o caminho /me com um token de usuário para criar reuniões online.</span><span class="sxs-lookup"><span data-stu-id="491fe-139">Use the /me path with a user token to create online meetings going forward.</span></span>

# <a name="http"></a>[<span data-ttu-id="491fe-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="491fe-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="491fe-141">C#</span><span class="sxs-lookup"><span data-stu-id="491fe-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onlinemeeting-app-token-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="491fe-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="491fe-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onlinemeeting-app-token-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="491fe-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="491fe-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onlinemeeting-app-token-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="491fe-144">No corpo da solicitação, forneça uma representação JSON do objeto [onlineMeeting](../resources/onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="491fe-144">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="491fe-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="491fe-145">Response</span></span>

><span data-ttu-id="491fe-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="491fe-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-an-online-meeting-with-user-token"></a><span data-ttu-id="491fe-148">Exemplo 2: criar uma reunião online com o token de usuário</span><span class="sxs-lookup"><span data-stu-id="491fe-148">Example 2: Create an online meeting with user token</span></span>

#### <a name="request"></a><span data-ttu-id="491fe-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="491fe-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="491fe-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="491fe-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="491fe-151">C#</span><span class="sxs-lookup"><span data-stu-id="491fe-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onlinemeeting-user-token-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="491fe-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="491fe-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onlinemeeting-user-token-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="491fe-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="491fe-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onlinemeeting-user-token-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="491fe-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="491fe-154">Response</span></span>
><span data-ttu-id="491fe-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="491fe-155">**Note:** The response object shown here might be shortened for readability.</span></span> 

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

### <a name="example-3-create-an-online-meeting-in-a-microsoft-teams-channel-with-a-user-token"></a><span data-ttu-id="491fe-156">Exemplo 3: criar uma reunião online em um Canal do Microsoft Teams com um token de usuário</span><span class="sxs-lookup"><span data-stu-id="491fe-156">Example 3: Create an online meeting in a Microsoft Teams Channel with a user token</span></span>

#### <a name="request"></a><span data-ttu-id="491fe-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="491fe-157">Request</span></span>
><span data-ttu-id="491fe-158">**Observação:**: a ID de objeto do token do usuário aprovada deve ser um membro do canal representado pelo threadid no conteúdo.</span><span class="sxs-lookup"><span data-stu-id="491fe-158">**Note:** The Object ID of the user token passed should be a member of the channel represented by threadid in the payload.</span></span>

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
#### <a name="response"></a><span data-ttu-id="491fe-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="491fe-159">Response</span></span>

><span data-ttu-id="491fe-160">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="491fe-160">**Note:** The response object shown here might be shortened for readability.</span></span>

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
