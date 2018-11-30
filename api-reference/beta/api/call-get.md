---
title: Fazer chamada
description: Recupere as propriedades e relacionamentos de um objeto de chamada.
ms.openlocfilehash: d161160fbce95e1aa549c8561c0c271b5c641818
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037354"
---
# <a name="get-call"></a><span data-ttu-id="dede1-103">Fazer chamada</span><span class="sxs-lookup"><span data-stu-id="dede1-103">Get call</span></span>

> <span data-ttu-id="dede1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dede1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dede1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dede1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dede1-106">Recupere as propriedades e relacionamentos de um objeto de chamada.</span><span class="sxs-lookup"><span data-stu-id="dede1-106">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dede1-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="dede1-107">Permissions</span></span>
<span data-ttu-id="dede1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dede1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dede1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dede1-110">Permission type</span></span> | <span data-ttu-id="dede1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dede1-111">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="dede1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dede1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="dede1-113">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="dede1-113">Not Supported.</span></span>                         |
| <span data-ttu-id="dede1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dede1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dede1-115">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="dede1-115">Not Supported.</span></span>                         |
| <span data-ttu-id="dede1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dede1-116">Application</span></span>                            | <span data-ttu-id="dede1-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="dede1-117">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="dede1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dede1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}
GET /applications/{id}/calls/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dede1-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dede1-119">Optional query parameters</span></span>
<span data-ttu-id="dede1-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dede1-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dede1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dede1-121">Request headers</span></span>
| <span data-ttu-id="dede1-122">Nome</span><span class="sxs-lookup"><span data-stu-id="dede1-122">Name</span></span>          | <span data-ttu-id="dede1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="dede1-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="dede1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="dede1-124">Authorization</span></span> | <span data-ttu-id="dede1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dede1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dede1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dede1-127">Request body</span></span>
<span data-ttu-id="dede1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dede1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dede1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dede1-129">Response</span></span>
<span data-ttu-id="dede1-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [chamada](../resources/call.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dede1-130">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dede1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dede1-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dede1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dede1-132">Request</span></span>
<span data-ttu-id="dede1-133">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="dede1-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_call"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="dede1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dede1-134">Response</span></span>

> <span data-ttu-id="dede1-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dede1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get call",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
