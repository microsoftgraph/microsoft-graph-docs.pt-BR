---
title: Obter onlineMeeting
description: Recupere as propriedades e os relacionamentos de um objeto de **reunião online** .
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 704ca0d5dca4b1bbee02ebc779d13503403d2646
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865671"
---
# <a name="get-onlinemeeting"></a><span data-ttu-id="ff135-103">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ff135-103">Get onlineMeeting</span></span>

<span data-ttu-id="ff135-104">Recupere as propriedades e os relacionamentos de um objeto [onlineMeeting](../resources/onlinemeeting.md) .</span><span class="sxs-lookup"><span data-stu-id="ff135-104">Retrieve the properties and relationships of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

> <span data-ttu-id="ff135-105">**Observação:** Atualmente `GET` , o método só tem suporte para uma [ID de conferência VTC](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). Essas IDs são geradas para usuários licenciados de Cloud-Video-Interop e este método é usado para obter os detalhes para ingressar na reunião.</span><span class="sxs-lookup"><span data-stu-id="ff135-105">**Note:** The `GET` method is currently only supported for a [VTC conference id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). These IDs are generated for Cloud-Video-Interop licensed users and this method is used to get the details to join the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff135-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff135-106">Permissions</span></span>

<span data-ttu-id="ff135-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff135-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff135-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff135-109">Permission type</span></span>                        | <span data-ttu-id="ff135-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff135-110">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="ff135-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff135-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ff135-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff135-112">Not Supported.</span></span>                                        |
| <span data-ttu-id="ff135-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff135-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff135-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff135-114">Not Supported.</span></span>                                        |
| <span data-ttu-id="ff135-115">Application</span><span class="sxs-lookup"><span data-stu-id="ff135-115">Application</span></span>                            | <span data-ttu-id="ff135-116">OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff135-116">OnlineMeetings.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff135-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff135-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{id}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff135-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ff135-118">Optional query parameters</span></span>
<span data-ttu-id="ff135-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ff135-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff135-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff135-120">Request headers</span></span>
| <span data-ttu-id="ff135-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ff135-121">Name</span></span>          | <span data-ttu-id="ff135-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff135-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="ff135-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff135-123">Authorization</span></span> | <span data-ttu-id="ff135-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff135-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff135-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff135-126">Request body</span></span>
<span data-ttu-id="ff135-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff135-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff135-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff135-128">Response</span></span>
<span data-ttu-id="ff135-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff135-129">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff135-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ff135-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ff135-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff135-131">Request</span></span>
<span data-ttu-id="ff135-132">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff135-132">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ff135-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff135-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'123456789'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ff135-134">C#</span><span class="sxs-lookup"><span data-stu-id="ff135-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff135-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff135-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ff135-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff135-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ff135-137">Java</span><span class="sxs-lookup"><span data-stu-id="ff135-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onlinemeeting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ff135-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff135-138">Response</span></span>

> <span data-ttu-id="ff135-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff135-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.type": "#microsoft.graph.meetingParticipants",
    "attendees": [
      {
        "@odata.type": "#microsoft.graph.identitySet",
        "identity": {
          "user": {
            "@odata.type": "#microsoft.graph.identity",
            "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8",
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
