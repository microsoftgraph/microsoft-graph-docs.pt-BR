---
title: Obter chamada
description: Recupere as propriedades e os relacionamentos de um objeto de chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2accad64fabf12b578d1d455db08d6aa0b8539e6
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635789"
---
# <a name="get-call"></a><span data-ttu-id="1f23b-103">Obter chamada</span><span class="sxs-lookup"><span data-stu-id="1f23b-103">Get call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f23b-104">Recupere as propriedades e os relacionamentos de um objeto de chamada.</span><span class="sxs-lookup"><span data-stu-id="1f23b-104">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f23b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f23b-105">Permissions</span></span>
<span data-ttu-id="1f23b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f23b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1f23b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f23b-108">Permission type</span></span> | <span data-ttu-id="1f23b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f23b-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="1f23b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f23b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f23b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f23b-111">Not Supported.</span></span>                         |
| <span data-ttu-id="1f23b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f23b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f23b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f23b-113">Not Supported.</span></span>                         |
| <span data-ttu-id="1f23b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f23b-114">Application</span></span>                            | <span data-ttu-id="1f23b-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1f23b-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="1f23b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f23b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}
GET /applications/{id}/calls/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f23b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1f23b-117">Optional query parameters</span></span>
<span data-ttu-id="1f23b-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1f23b-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f23b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f23b-119">Request headers</span></span>
| <span data-ttu-id="1f23b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1f23b-120">Name</span></span>          | <span data-ttu-id="1f23b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f23b-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1f23b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f23b-122">Authorization</span></span> | <span data-ttu-id="1f23b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f23b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f23b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f23b-125">Request body</span></span>
<span data-ttu-id="1f23b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1f23b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f23b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f23b-127">Response</span></span>
<span data-ttu-id="1f23b-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Call](../resources/call.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f23b-128">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f23b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f23b-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1f23b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f23b-130">Request</span></span>
<span data-ttu-id="1f23b-131">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f23b-131">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-call"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="1f23b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f23b-132">Response</span></span>

> <span data-ttu-id="1f23b-p103">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f23b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2821

{
  "activeModalities": [
    "unknown"
  ],
  "answeredBy": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "callRoutes": [
    {
      "final": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "original": {
        "phone": {
          "id": "+14258828080"
        }
      },
      "routingType": "forwarded"
    }
  ],
  "callbackUri": "callbackUri-value",
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "direction": "incoming",
  "id": "id-value",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  },
  "meetingCapability": {
    "allowAnonymousUsersToDialOut": true,
    "allowAnonymousUsersToStartMeeting": true,
    "autoAdmittedUsers": "everyoneInCompany"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "allowConversationWithoutHost": true
  },
  "myParticipantId": "myParticipantId-value",
  "requestedModalities": [
    "audio", "video"
  ],
  "ringingTimeoutInSeconds": 99,
  "routingPolicies": [
    "none"
  ],
  "source": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "state": "incoming",
  "subject": "subject-value",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "languageId-value",
      "region": "region-value"
    }
  ],
  "tenantId": "tenantId-value",
  "terminationReason": "terminationReason-value",
  "toneInfo": {
    "sequenceId": 99,
    "tone": "tone0"
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1f23b-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="1f23b-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1f23b-136">Basic</span><span class="sxs-lookup"><span data-stu-id="1f23b-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-call-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1f23b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f23b-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-call-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
