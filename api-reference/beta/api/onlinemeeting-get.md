---
title: Obter reunião online
description: Recupere as propriedades e os relacionamentos de um objeto de **reunião online** .
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 9b5d571a73a03f6e313f13912b10262bff7b7041
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006484"
---
# <a name="get-online-meeting"></a><span data-ttu-id="278c9-103">Obter reunião online</span><span class="sxs-lookup"><span data-stu-id="278c9-103">Get Online Meeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="278c9-104">Recupere as propriedades e os relacionamentos de um objeto [onlineMeeting](../resources/onlinemeeting.md) .</span><span class="sxs-lookup"><span data-stu-id="278c9-104">Retrieve the properties and relationships of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

> <span data-ttu-id="278c9-105">**Observação:** Atualmente `GET` , o método só tem suporte para uma [ID de conferência VTC](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). Essas IDs são geradas para usuários licenciados de Cloud-Video-Interop e este método é usado para obter os detalhes para ingressar na reunião.</span><span class="sxs-lookup"><span data-stu-id="278c9-105">**Note:** The `GET` method is currently only supported for a [VTC conference id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). These IDs are generated for Cloud-Video-Interop licensed users and this method is used to get the details to join the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="278c9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="278c9-106">Permissions</span></span>

<span data-ttu-id="278c9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="278c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="278c9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="278c9-109">Permission type</span></span>                        | <span data-ttu-id="278c9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="278c9-110">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="278c9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="278c9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="278c9-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="278c9-112">Not Supported.</span></span>                                        |
| <span data-ttu-id="278c9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="278c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="278c9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="278c9-114">Not Supported.</span></span>                                        |
| <span data-ttu-id="278c9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="278c9-115">Application</span></span>                            | <span data-ttu-id="278c9-116">OnlineMeetings. Read. All, OnlineMeetings. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="278c9-116">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="278c9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="278c9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{id}'
GET /communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{id}'
```
> <span data-ttu-id="278c9-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="278c9-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="278c9-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="278c9-119">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="278c9-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="278c9-120">Optional query parameters</span></span>
<span data-ttu-id="278c9-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="278c9-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="278c9-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="278c9-122">Request headers</span></span>
| <span data-ttu-id="278c9-123">Nome</span><span class="sxs-lookup"><span data-stu-id="278c9-123">Name</span></span>          | <span data-ttu-id="278c9-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="278c9-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="278c9-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="278c9-125">Authorization</span></span> | <span data-ttu-id="278c9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="278c9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="278c9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="278c9-128">Request body</span></span>
<span data-ttu-id="278c9-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="278c9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="278c9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="278c9-130">Response</span></span>
<span data-ttu-id="278c9-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="278c9-131">If successful, this method returns a `200 OK` response code and [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="278c9-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="278c9-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="278c9-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="278c9-133">Request</span></span>
<span data-ttu-id="278c9-134">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="278c9-134">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="278c9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="278c9-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'123456789'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="278c9-136">C#</span><span class="sxs-lookup"><span data-stu-id="278c9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="278c9-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="278c9-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="278c9-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="278c9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="278c9-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="278c9-139">Response</span></span>

> <span data-ttu-id="278c9-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="278c9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "canceledDateTime": "0001-01-01T08:00:00Z",
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
    "messageId": "1533758867081"
  },
  "creationDateTime": "2018-05-30T00:12:19.0726086Z",
  "endDateTime": "2018-05-30T01:00:00Z",
  "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8_19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
  "isCanceled": false,
  "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3a:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context=%7b%22Tid%22%3a%aa67bd4c-8475-432d-bd41-39f255720e0a%22%2c%22Oid%22%3a%22112f7296-5fa4-42ca-bae8-6a692b15d4b8%22%7d",
  "isBroadcast": false,
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