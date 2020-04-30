---
title: Criar ReuniãoOnline
description: Crie uma reunião online em nome de um usuário específico no corpo da solicitação.
author: ananmishr
localization_priority: Priority
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 9f85832dc557a2e2242c30cd983cfb9800382176
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2020
ms.locfileid: "43934707"
---
# <a name="create-onlinemeeting"></a><span data-ttu-id="df74a-103">Criar ReuniãoOnline</span><span class="sxs-lookup"><span data-stu-id="df74a-103">Create onlineMeeting</span></span>

<span data-ttu-id="df74a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df74a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df74a-105">Crie uma reunião online em nome de um usuário usando a ID de objeto (OID) no token de usuário.</span><span class="sxs-lookup"><span data-stu-id="df74a-105">Create an online meeting on behalf of a user by using the object ID (OID) in the user token.</span></span>

> <span data-ttu-id="df74a-106">**Observação**: a reunião não é exibida no calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="df74a-106">**Note**: The meeting does not show up on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="df74a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="df74a-107">Permissions</span></span>
<span data-ttu-id="df74a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df74a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df74a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df74a-110">Permission type</span></span>                        | <span data-ttu-id="df74a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df74a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="df74a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df74a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="df74a-113">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="df74a-113">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="df74a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df74a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df74a-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="df74a-115">Not Supported</span></span>                               |
| <span data-ttu-id="df74a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df74a-116">Application</span></span>                            | <span data-ttu-id="df74a-117">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="df74a-117">OnlineMeetings.ReadWrite.All\*</span></span>  |

> <span data-ttu-id="df74a-118">\* **Observação:** as permissões de aplicativo foram preteridas e serão removidas em julho de 2020.</span><span class="sxs-lookup"><span data-stu-id="df74a-118">\* **Note:** Application permissions are deprecated and will be removed in July 2020.</span></span> <span data-ttu-id="df74a-119">Para criar um evento do Outlook, usando permissões de aplicativo, confira [Criar evento](user-post-events.md).</span><span class="sxs-lookup"><span data-stu-id="df74a-119">To create an Outlook event instead, using application permissions, see [Create event](user-post-events.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="df74a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df74a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
POST /communications/onlineMeetings
POST /me/onlineMeetings
```
> <span data-ttu-id="df74a-121">**Observação:** O `/app` ou`/communications` caminho com um token de aplicativo está obsoleto.</span><span class="sxs-lookup"><span data-stu-id="df74a-121">**Note:** The `/app` or `/communications` path with an application token is deprecated.</span></span> <span data-ttu-id="df74a-122">No futuro, use o/meu caminho com um token de usuário para criar reuniões on-line.</span><span class="sxs-lookup"><span data-stu-id="df74a-122">Going forward, use the /me path with a user token to create online meetings.</span></span>

## <a name="request-headers"></a><span data-ttu-id="df74a-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df74a-123">Request headers</span></span>
| <span data-ttu-id="df74a-124">Nome</span><span class="sxs-lookup"><span data-stu-id="df74a-124">Name</span></span>          | <span data-ttu-id="df74a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="df74a-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="df74a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="df74a-126">Authorization</span></span> | <span data-ttu-id="df74a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df74a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="df74a-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="df74a-129">Content-type</span></span>  | <span data-ttu-id="df74a-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df74a-p105">application/json. Required.</span></span> |
| <span data-ttu-id="df74a-132">Accept-Language</span><span class="sxs-lookup"><span data-stu-id="df74a-132">Accept-Language</span></span>  | <span data-ttu-id="df74a-133">Idioma.</span><span class="sxs-lookup"><span data-stu-id="df74a-133">Language.</span></span> <span data-ttu-id="df74a-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="df74a-134">Optional.</span></span> |

<span data-ttu-id="df74a-135">Se a solicitação contiver um `Accept-Language`cabeçalho HTTP, o `content` de `joinInformation` estará na variante de idioma e código de idioma especificada `Accept-Language` no cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="df74a-135">If the request contains an `Accept-Language` HTTP header, the `content` of `joinInformation` will be in the language and locale variant specified in the `Accept-Language` header.</span></span> <span data-ttu-id="df74a-136">O conteúdo padrão será em inglês.</span><span class="sxs-lookup"><span data-stu-id="df74a-136">The default content will be in English.</span></span>

## <a name="request-body"></a><span data-ttu-id="df74a-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df74a-137">Request body</span></span>
<span data-ttu-id="df74a-138">No corpo da solicitação, forneça uma representação JSON de um objeto [onlineMeeting](../resources/onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="df74a-138">In the request body, supply a JSON representation of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="df74a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="df74a-139">Response</span></span>
<span data-ttu-id="df74a-140">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df74a-140">If successful, this method returns a `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df74a-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="df74a-141">Examples</span></span>

### <a name="example-1-create-an-online-meeting-with-application-token"></a><span data-ttu-id="df74a-142">Exemplo 1: criar uma reunião online com o token do aplicativo</span><span class="sxs-lookup"><span data-stu-id="df74a-142">Example 1: Create an online meeting with application token</span></span>

#### <a name="request"></a><span data-ttu-id="df74a-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df74a-143">Request</span></span>

> [!Note]
> <span data-ttu-id="df74a-144">A criação de reuniões online usando um token de aplicativo foi preterida e o suporte será removido em julho de 2020.</span><span class="sxs-lookup"><span data-stu-id="df74a-144">Online meeting creation using an application token is deprecated and support will be removed in July 2020.</span></span> <span data-ttu-id="df74a-145">Use o caminho /me com um token de usuário para criar reuniões online.</span><span class="sxs-lookup"><span data-stu-id="df74a-145">Use the /me path with a user token to create online meetings going forward.</span></span>

# <a name="http"></a>[<span data-ttu-id="df74a-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="df74a-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="df74a-147">C#</span><span class="sxs-lookup"><span data-stu-id="df74a-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onlinemeeting-app-token-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df74a-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df74a-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onlinemeeting-app-token-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df74a-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df74a-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onlinemeeting-app-token-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="df74a-150">No corpo da solicitação, forneça uma representação JSON do objeto [onlineMeeting](../resources/onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="df74a-150">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="df74a-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="df74a-151">Response</span></span>

><span data-ttu-id="df74a-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df74a-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-an-online-meeting-with-user-token"></a><span data-ttu-id="df74a-154">Exemplo 2: criar uma reunião online com o token de usuário</span><span class="sxs-lookup"><span data-stu-id="df74a-154">Example 2: Create an online meeting with user token</span></span>

#### <a name="request"></a><span data-ttu-id="df74a-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df74a-155">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="df74a-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="df74a-156">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="df74a-157">C#</span><span class="sxs-lookup"><span data-stu-id="df74a-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onlinemeeting-user-token-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df74a-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df74a-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onlinemeeting-user-token-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df74a-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df74a-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onlinemeeting-user-token-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="df74a-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="df74a-160">Response</span></span>
><span data-ttu-id="df74a-161">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="df74a-161">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
><span data-ttu-id="df74a-162">**Observação:** Se 'Accept-Language: ja' for especificado para indicar japonês, por exemplo, a resposta incluirá o seguinte.</span><span class="sxs-lookup"><span data-stu-id="df74a-162">**Note:** If 'Accept-Language: ja' is specified to indicate Japanese, for example, the response will include the following.</span></span>

```json
    "joinInformation": {
        "content": "data%3Atext%2Fhtml%2C%0A++%3Cdiv+style%3D%22width%3A100%25%3Bheight%3A+20px%3B%22%3E%0A%09%09%3Cspan+style%3D%22white-space%3Anowrap%3Bcolor%3Agray%3Bopacity%3A.36%3B%22%3E________________________________________________________________________________%3C%2Fspan%3E%0A%09+%3C%2Fdiv%3E%0A++++%3Cdiv+class%3D%22me-email-text%22+style%3D%22color%3A%23252424%3Bfont-family%3A'Segoe+UI'%2C'Helvetica+Neue'%2CHelvetica%2CArial%2Csans-serif%3B%22%3E%0A+++%3Cdiv+style%3D%22margin-top%3A+24px%3B+margin-bottom%3A+10px%3B%22%3E%0A++++++++%3Ca+class%3D%22me-email-headline%22%0A++++++++++++++style%3D%22font-size%3A+18px%3Bfont-family%3A'Segoe+UI+Semibold'%2C'Segoe+UI'%2C'Helvetica+Neue'%2CHelvetica%2CArial%2Csans-serif%3Btext-decoration%3A+underline%3Bcolor%3A+%236264a7%3B%22%0A++++++++++++++href%3D%22https%3A%2F%2Fteams.microsoft.com%2Fl%2Fmeetup-join%2F19%253ameeting_NDRiZjRiMmUtODI5OC00MzRlLTk1ZWEtMGY1000000000000%2540thread.v2%2F0%3Fcontext%3D%257b%2522Tid%2522%253a%252279a788bf-86f1-41af-91ab-000000000000%2522%252c%2522Oid%2522%253a%2522d4a060b5-a8fc-450c-837b-000000000000%2522%257d%22%0A++++++++++++++target%3D%22_blank%22+rel%3D%22noreferrer+noopener%22%3EMicrosoft+Teams+%E4%BC%9A%E8%AD%B0%E3%81%AB%E5%8F%82%E5%8A%A0%3C%2Fa%3E%0A++++++%3C%2Fdiv%3E%0A%09+%3Cdiv%3E%0A++++%0A++++++%3Cdiv%3E%0A++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+14px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22%0A++++++++++href%3D%22tel%3A%2B16477490000%2C%2C11160000%26%2335%3B+%22+target%3D%22_blank%22+rel%3D%22noreferrer+noopener%22%3E%2B16477490000%3C%2Fa%3E%0A++++++%3Cspan+style%3D%22font-size%3A+12px%3B%22%3E%26nbsp%3B++(%E6%9C%89%E6%96%99)+%3C%2Fspan%3E%0A++++++%3C%2Fdiv%3E%0A++++%0A++%3C%2Fdiv%3E%0A%0A%09+%0A++++++%3Cdiv+style%3D%22margin-top%3A+10px%3B+margin-bottom%3A+20px%3B%22%3E%0A++++++++%3Cspan+style%3D%22font-size%3A+12px%3B%22%3E%0A++++++++++%E4%BC%9A%E8%AD%B0+ID%3A%0A++++++++%3C%2Fspan%3E%0A++++++%3Cspan+style%3D%22font-size%3A+14px%3B%22%3E%0A++++++++111+000+00%23%0A++++++%3C%2Fspan%3E%0A++++%3C%2Fdiv%3E%0A++++%0A%09+%0A++++++++%3Cdiv+style%3D%22margin-bottom%3A+24px%3B%22%3E%0A++++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fdialin.teams.microsoft.com%2F8bf6e654-57eb-4b85-aeaf-36c84429b2fe%3Fid%3D11160000%22+rel%3D%22noreferrer+noopener%22%3E%E6%9C%80%E5%AF%84%E3%82%8A%E3%81%AE%E5%9B%BD%E3%81%AE%E9%9B%BB%E8%A9%B1%E7%95%AA%E5%8F%B7%E3%82%92%E6%A4%9C%E7%B4%A2%3C%2Fa%3E%0A+++++++++%7C%0A++++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fmysettings.lync.com%2Fpstnconferencing%22+rel%3D%22noreferrer+noopener%22%3E%0A++++++++PIN+%E3%82%92%E3%83%AA%E3%82%BB%E3%83%83%E3%83%88%3C%2Fa%3E%0A+++++++++%7C+%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Faka.ms%2FJoinTeamsMeeting%22+rel%3D%22noreferrer+noopener%22%3ETeams+%E3%81%AE%E8%A9%B3%E7%B4%B0%E3%82%92%E8%A1%A8%E7%A4%BA%3C%2Fa%3E%0A+++++%7C+%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fteams.microsoft.com%2FmeetingOptions%2F%3ForganizerId%3Dd4a060b5-a8fc-450c-837b-000000000000%26tenantId%3D79a788bf-86f1-41af-91ab-000000000000%26threadId%3D19_meeting_NDRiZjRiMmUtODI5OC00MzRlLTk1ZWEtMGY1000000000000%40thread.v2%26messageId%3D0%26language%3Dja%22+rel%3D%22noreferrer+noopener%22%3E%E4%BC%9A%E8%AD%B0%E3%81%AE%E3%82%AA%E3%83%97%E3%82%B7%E3%83%A7%E3%83%B3%3C%2Fa%3E%0A++++%0A++++++++%3C%2Fdiv%3E%0A++++%0A+++++%0A++++++++%3Cdiv+style%3D%22font-size%3A+14px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++++++%E3%83%93%E3%83%87%E3%82%AA%E4%BC%9A%E8%AD%B0%E3%83%87%E3%83%90%E3%82%A4%E3%82%B9%E3%81%A7%E5%8F%82%E5%8A%A0%0A++++++++%3C%2Fdiv%3E%0A%0A++++++++%3Cdiv+style%3D%22font-size%3A12px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22text-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+href%3D%22%22%3E000000000%40t.abcd.vc%3C%2Fa%3E+VTC+%E4%BC%9A%E8%AD%B0+ID%3A+0180300000%0A++++++++%3C%2Fdiv%3E%0A%0A++++++++%3Cdiv+style%3D%22font-size%3A+12px%3B+margin-bottom%3A+20px%3B%22%3E%0A++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22text-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+href%3D%22https%3A%2F%2Fdialin.abcd.vc%2Fteams%2F%3Fkey%3D000000000%26conf%3D0180308922%22%3E%E4%BB%A3%E6%9B%BF+VTC+%E3%81%AE%E3%83%80%E3%82%A4%E3%83%A4%E3%83%AB%E6%96%B9%E6%B3%95%3C%2Fa%3E%0A++++++++%3C%2Fdiv%3E%0A++++%0A+++++%0A++++++%3Cdiv+style%3D%22font-size%3A+14px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++%0A++++++%3C%2Fdiv%3E%0A++++++%3Cdiv+style%3D%22font-size%3A+12px%3B%22%3E%0A++++++%0A++++++%3C%2Fdiv%3E%0A++++%0A+++++%3C%2Fdiv%3E%0A%09+%3Cdiv+style%3D%22width%3A100%25%3Bheight%3A+20px%3B%22%3E%0A%09%09%3Cspan+style%3D%22white-space%3Anowrap%3Bcolor%3Agray%3Bopacity%3A.36%3B%22%3E________________________________________________________________________________%3C%2Fspan%3E%0A++%3C%2Fdiv%3E%22%2C%0A",
        "contentType": "Html"
    }  
```


### <a name="example-3-create-an-online-meeting-in-a-microsoft-teams-channel-with-a-user-token"></a><span data-ttu-id="df74a-163">Exemplo 3: criar uma reunião online em um Canal do Microsoft Teams com um token de usuário</span><span class="sxs-lookup"><span data-stu-id="df74a-163">Example 3: Create an online meeting in a Microsoft Teams Channel with a user token</span></span>

#### <a name="request"></a><span data-ttu-id="df74a-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df74a-164">Request</span></span>
><span data-ttu-id="df74a-165">**Observação:**: a ID de objeto do token do usuário aprovada deve ser um membro do canal representado pelo threadid no conteúdo.</span><span class="sxs-lookup"><span data-stu-id="df74a-165">**Note:** The Object ID of the user token passed should be a member of the channel represented by threadid in the payload.</span></span>

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
#### <a name="response"></a><span data-ttu-id="df74a-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="df74a-166">Response</span></span>

><span data-ttu-id="df74a-167">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="df74a-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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
