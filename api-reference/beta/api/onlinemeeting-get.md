---
title: Obter onlineMeeting
description: Recupere as propriedades e os relacionamentos de um objeto de **reunião online** .
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 58c995a9ca6be7029b1a5510023160c97cadb735
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456500"
---
# <a name="get-onlinemeeting"></a><span data-ttu-id="2edb6-103">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="2edb6-103">Get onlineMeeting</span></span>

<span data-ttu-id="2edb6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2edb6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2edb6-105">Recupere as propriedades e os relacionamentos de um objeto [onlineMeeting](../resources/onlinemeeting.md) .</span><span class="sxs-lookup"><span data-stu-id="2edb6-105">Retrieve the properties and relationships of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

> <span data-ttu-id="2edb6-106">**Observação:** Atualmente `GET` , o método só tem suporte para uma [ID de conferência VTC](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). Essas IDs são geradas para usuários licenciados de Cloud-Video-Interop e este método é usado para obter os detalhes para ingressar na reunião.</span><span class="sxs-lookup"><span data-stu-id="2edb6-106">**Note:** The `GET` method is currently only supported for a [VTC conference id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). These IDs are generated for Cloud-Video-Interop licensed users and this method is used to get the details to join the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="2edb6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2edb6-107">Permissions</span></span>

<span data-ttu-id="2edb6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2edb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2edb6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2edb6-110">Permission type</span></span>                        | <span data-ttu-id="2edb6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2edb6-111">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="2edb6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2edb6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2edb6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2edb6-113">Not Supported.</span></span>                                        |
| <span data-ttu-id="2edb6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2edb6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2edb6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2edb6-115">Not Supported.</span></span>                                        |
| <span data-ttu-id="2edb6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2edb6-116">Application</span></span>                            | <span data-ttu-id="2edb6-117">OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="2edb6-117">OnlineMeetings.Read.All</span></span>                               |

## <a name="http-request"></a><span data-ttu-id="2edb6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2edb6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{id}'
GET /communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{id}'
```
> <span data-ttu-id="2edb6-119">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="2edb6-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="2edb6-120">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="2edb6-120">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="2edb6-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2edb6-121">Optional query parameters</span></span>
<span data-ttu-id="2edb6-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2edb6-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2edb6-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2edb6-123">Request headers</span></span>
| <span data-ttu-id="2edb6-124">Nome</span><span class="sxs-lookup"><span data-stu-id="2edb6-124">Name</span></span>          | <span data-ttu-id="2edb6-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="2edb6-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2edb6-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="2edb6-126">Authorization</span></span> | <span data-ttu-id="2edb6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2edb6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2edb6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2edb6-129">Request body</span></span>
<span data-ttu-id="2edb6-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2edb6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2edb6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2edb6-131">Response</span></span>
<span data-ttu-id="2edb6-132">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2edb6-132">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2edb6-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2edb6-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2edb6-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2edb6-134">Request</span></span>
<span data-ttu-id="2edb6-135">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="2edb6-135">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2edb6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2edb6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'123456789'
```
# <a name="c"></a>[<span data-ttu-id="2edb6-137">C#</span><span class="sxs-lookup"><span data-stu-id="2edb6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2edb6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2edb6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2edb6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2edb6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2edb6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2edb6-140">Response</span></span>

> <span data-ttu-id="2edb6-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2edb6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "autoAdmittedUsers": "everyone",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "9999999",
    "dialinUrl": "https://dialin.teams.microsoft.com/6787A136-B9B8-4D39-846C-C0F1FF937F10?id=xxxxxxx"
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
    "messageId": "1533758867081"
  },
  "creationDateTime": "2018-05-30T00:12:19.0726086Z",
  "endDateTime": "2018-05-30T01:00:00Z",
  "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8_19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3a:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context=%7b%22Tid%22%3a%aa67bd4c-8475-432d-bd41-39f255720e0a%22%2c%22Oid%22%3a%22112f7296-5fa4-42ca-bae8-6a692b15d4b8%22%7d",
  "participants": {
    "attendees": [
      {
        "@odata.type": "#microsoft.graph.identitySet",
        "identity": {
          "user": {
            "@odata.type": "#microsoft.graph.identity",
            "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8",
            "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
            "displayName": "John"
          }
        },
        "upn": "upn-value"
      }
    ],
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "identity": {
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
          "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
          "displayName": "Bob"
        }
      },
      "upn": "upn-value"
    }
  },
  "startDateTime": "2018-05-30T00:30:00Z",
  "subject": "Test Meeting.",
  "videoTeleconferenceId": "123456789"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
