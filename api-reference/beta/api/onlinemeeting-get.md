---
title: Get de Reunião Online
description: Recupere as propriedades e relacionamentos de um objeto **onlineMeeting** .
author: VinodRavichandran
ms.openlocfilehash: bfae4273aba0583e6c10a7e10f9c67865326bacf
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380377"
---
# <a name="get-online-meeting"></a><span data-ttu-id="ddfc7-103">Get de Reunião Online</span><span class="sxs-lookup"><span data-stu-id="ddfc7-103">Get Online Meeting</span></span>

> <span data-ttu-id="ddfc7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ddfc7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ddfc7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ddfc7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ddfc7-106">Recupere as propriedades e relacionamentos de um objeto **onlineMeeting** .</span><span class="sxs-lookup"><span data-stu-id="ddfc7-106">Retrieve the properties and relationships of an **onlineMeeting** object.</span></span>

> <span data-ttu-id="ddfc7-107">**Observação:** O `GET` método está limitado a uma [id de conferência VTC](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). Essas IDs são geradas para interoperabilidade de vídeo de nuvem licenciados usuários e este método é usado para obter os detalhes para ingressar na reunião.</span><span class="sxs-lookup"><span data-stu-id="ddfc7-107">**Note:** The `GET` method is limited to a [VTC conference id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). These IDs are generated for Cloud-Video-Interop licensed users and this method is used to get the details to join the meeting.</span></span>
> <span data-ttu-id="ddfc7-108">Para fluxos de regulares, o bot pode usar o `joinURL` ingressar em uma reunião e nenhuma pesquisa é necessária.</span><span class="sxs-lookup"><span data-stu-id="ddfc7-108">For regular flows, the bot can use the `joinURL` to join a meeting and no lookup is necessary.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddfc7-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="ddfc7-109">Permissions</span></span>

<span data-ttu-id="ddfc7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddfc7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ddfc7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddfc7-112">Permission type</span></span>                        | <span data-ttu-id="ddfc7-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ddfc7-113">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="ddfc7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddfc7-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="ddfc7-115">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="ddfc7-115">Not Supported.</span></span>                                        |
| <span data-ttu-id="ddfc7-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddfc7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddfc7-117">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="ddfc7-117">Not Supported.</span></span>                                        |
| <span data-ttu-id="ddfc7-118">Application</span><span class="sxs-lookup"><span data-stu-id="ddfc7-118">Application</span></span>                            | <span data-ttu-id="ddfc7-119">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddfc7-119">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddfc7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddfc7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/{id}
GET /applications/{id}/onlineMeetings/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ddfc7-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ddfc7-121">Optional query parameters</span></span>
<span data-ttu-id="ddfc7-122">Este método oferece suporte para os [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ddfc7-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddfc7-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddfc7-123">Request headers</span></span>
| <span data-ttu-id="ddfc7-124">Nome</span><span class="sxs-lookup"><span data-stu-id="ddfc7-124">Name</span></span>          | <span data-ttu-id="ddfc7-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddfc7-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="ddfc7-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddfc7-126">Authorization</span></span> | <span data-ttu-id="ddfc7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddfc7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddfc7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddfc7-129">Request body</span></span>
<span data-ttu-id="ddfc7-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ddfc7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddfc7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddfc7-131">Response</span></span>
<span data-ttu-id="ddfc7-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddfc7-132">If successful, this method returns a `200 OK` response code and [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddfc7-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ddfc7-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ddfc7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddfc7-134">Request</span></span>
<span data-ttu-id="ddfc7-135">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddfc7-135">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```http
GET https://graph.microsoft.com/beta/app/onlineMeetings/{id}
```

##### <a name="response"></a><span data-ttu-id="ddfc7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddfc7-136">Response</span></span>

> <span data-ttu-id="ddfc7-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddfc7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
