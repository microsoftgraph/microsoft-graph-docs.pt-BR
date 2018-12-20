---
title: Fazer chamada
description: Recupere as propriedades e relacionamentos de um objeto de chamada.
author: VinodRavichandran
ms.openlocfilehash: df97b69f87a1562e56a96d84de1af740ab0aff65
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380321"
---
# <a name="get-call"></a><span data-ttu-id="90961-103">Fazer chamada</span><span class="sxs-lookup"><span data-stu-id="90961-103">Get call</span></span>

> <span data-ttu-id="90961-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="90961-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90961-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="90961-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90961-106">Recupere as propriedades e relacionamentos de um objeto de chamada.</span><span class="sxs-lookup"><span data-stu-id="90961-106">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="90961-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="90961-107">Permissions</span></span>
<span data-ttu-id="90961-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90961-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90961-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90961-110">Permission type</span></span> | <span data-ttu-id="90961-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90961-111">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="90961-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90961-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="90961-113">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="90961-113">Not Supported.</span></span>                         |
| <span data-ttu-id="90961-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90961-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90961-115">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="90961-115">Not Supported.</span></span>                         |
| <span data-ttu-id="90961-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90961-116">Application</span></span>                            | <span data-ttu-id="90961-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="90961-117">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="90961-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90961-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}
GET /applications/{id}/calls/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="90961-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="90961-119">Optional query parameters</span></span>
<span data-ttu-id="90961-120">Este método oferece suporte para os [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="90961-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="90961-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90961-121">Request headers</span></span>
| <span data-ttu-id="90961-122">Nome</span><span class="sxs-lookup"><span data-stu-id="90961-122">Name</span></span>          | <span data-ttu-id="90961-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="90961-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="90961-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="90961-124">Authorization</span></span> | <span data-ttu-id="90961-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90961-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90961-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90961-127">Request body</span></span>
<span data-ttu-id="90961-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90961-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90961-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="90961-129">Response</span></span>
<span data-ttu-id="90961-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [chamada](../resources/call.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90961-130">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90961-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90961-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="90961-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90961-132">Request</span></span>
<span data-ttu-id="90961-133">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="90961-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-call"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="90961-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="90961-134">Response</span></span>

> <span data-ttu-id="90961-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90961-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get call",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
