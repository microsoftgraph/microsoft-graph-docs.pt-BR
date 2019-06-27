---
title: Obter reunião online
description: Recupere as propriedades e os relacionamentos de um objeto **onlineMeeting** .
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: da94541540989ef8e85c89e5fd64ea4b75867d91
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265895"
---
# <a name="get-online-meeting"></a><span data-ttu-id="57656-103">Obter reunião online</span><span class="sxs-lookup"><span data-stu-id="57656-103">Get Online Meeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57656-104">Recupere as propriedades e os relacionamentos de um objeto **onlineMeeting** .</span><span class="sxs-lookup"><span data-stu-id="57656-104">Retrieve the properties and relationships of an **onlineMeeting** object.</span></span>

> <span data-ttu-id="57656-105">**Observação:** O `GET` método é limitado a uma [ID de conferência do VTC](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). Essas IDs são geradas para usuários licenciados de Cloud-Video-Interop e este método é usado para obter os detalhes para ingressar na reunião.</span><span class="sxs-lookup"><span data-stu-id="57656-105">**Note:** The `GET` method is limited to a [VTC conference id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). These IDs are generated for Cloud-Video-Interop licensed users and this method is used to get the details to join the meeting.</span></span>
> <span data-ttu-id="57656-106">Para fluxos regulares, o bot pode usar o `joinURL` para ingressar em uma reunião e nenhuma pesquisa é necessária.</span><span class="sxs-lookup"><span data-stu-id="57656-106">For regular flows, the bot can use the `joinURL` to join a meeting and no lookup is necessary.</span></span>

## <a name="permissions"></a><span data-ttu-id="57656-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="57656-107">Permissions</span></span>

<span data-ttu-id="57656-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57656-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57656-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57656-110">Permission type</span></span>                        | <span data-ttu-id="57656-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="57656-111">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="57656-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57656-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="57656-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57656-113">Not Supported.</span></span>                                        |
| <span data-ttu-id="57656-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57656-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57656-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57656-115">Not Supported.</span></span>                                        |
| <span data-ttu-id="57656-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57656-116">Application</span></span>                            | <span data-ttu-id="57656-117">OnlineMeetings. Read. All, OnlineMeetings. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="57656-117">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57656-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57656-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/{id}
GET /applications/{id}/onlineMeetings/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="57656-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="57656-119">Optional query parameters</span></span>
<span data-ttu-id="57656-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="57656-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="57656-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57656-121">Request headers</span></span>
| <span data-ttu-id="57656-122">Nome</span><span class="sxs-lookup"><span data-stu-id="57656-122">Name</span></span>          | <span data-ttu-id="57656-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="57656-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="57656-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="57656-124">Authorization</span></span> | <span data-ttu-id="57656-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57656-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="57656-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57656-127">Request body</span></span>
<span data-ttu-id="57656-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57656-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57656-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="57656-129">Response</span></span>
<span data-ttu-id="57656-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57656-130">If successful, this method returns a `200 OK` response code and [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57656-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57656-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="57656-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57656-132">Request</span></span>
<span data-ttu-id="57656-133">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="57656-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```http
GET https://graph.microsoft.com/beta/app/onlineMeetings/{id}
```

##### <a name="response"></a><span data-ttu-id="57656-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="57656-134">Response</span></span>

> <span data-ttu-id="57656-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57656-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "accessLevel": "everyone",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "participantPasscode": "2425999",
    "leaderPasscode": null,
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "canceledDateTime": "2018-03-19T09:46:02Z",
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "creationDateTime": "2018-03-19T09:46:02Z",
  "endDateTime": "2018-03-19T09:46:02Z",
  "entryExitAnnouncement": true,
  "expirationDateTime": "2018-03-19T09:46:02Z",
  "id": "013448345",
  "isCancelled": false,
  "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "meetingType": "scheduled",
  "participants": {
    "attendees": [
      {
        "identity": {
          "user": {
            "id": "550fae72-d251-43ec-868c-373732c2704f",
            "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
            "displayName": "Heidi Steen"
          }
        },
        "upn": "upn-value"
      }
    ],
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
  "startDateTime": "2018-03-19T09:46:02Z",
  "subject": "Quarterly sales numbers"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="57656-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="57656-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="57656-138">C#</span><span class="sxs-lookup"><span data-stu-id="57656-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-onlineMeeting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="57656-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="57656-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-onlineMeeting-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="57656-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="57656-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-onlineMeeting-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/onlinemeeting-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/onlinemeeting-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/onlinemeeting-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
