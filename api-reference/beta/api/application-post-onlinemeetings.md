---
title: Criar a reunião online
description: Cria uma reunião online em nome de um usuário especificado no corpo da solicitação.
author: VinodRavichandran
localization_priority: Priority
ms.openlocfilehash: bd16b6979eed2c7d9386313f2ca07cb9ea2c5c6c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838945"
---
# <a name="create-online-meeting"></a><span data-ttu-id="0a1fc-103">Criar a reunião online</span><span class="sxs-lookup"><span data-stu-id="0a1fc-103">Create online meeting</span></span>

> <span data-ttu-id="0a1fc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0a1fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a1fc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0a1fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0a1fc-106">Cria uma reunião online em nome de um usuário especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a1fc-106">Creates an online meeting on behalf of a user specified in the request body.</span></span>

> <span data-ttu-id="0a1fc-107">**Observação**: A reunião não será mostrado no calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="0a1fc-107">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a1fc-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="0a1fc-108">Permissions</span></span>
<span data-ttu-id="0a1fc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a1fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0a1fc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a1fc-111">Permission type</span></span>                        | <span data-ttu-id="0a1fc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a1fc-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0a1fc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a1fc-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a1fc-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="0a1fc-114">Not Supported</span></span>                               |
| <span data-ttu-id="0a1fc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a1fc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a1fc-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="0a1fc-116">Not Supported</span></span>                               |
| <span data-ttu-id="0a1fc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a1fc-117">Application</span></span>                            | <span data-ttu-id="0a1fc-118">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a1fc-118">OnlineMeetings.ReadWrite.All</span></span>                |

## <a name="http-request"></a><span data-ttu-id="0a1fc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a1fc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
POST /applications/{id}/onlineMeetings
```

## <a name="request-headers"></a><span data-ttu-id="0a1fc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a1fc-120">Request headers</span></span>
| <span data-ttu-id="0a1fc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0a1fc-121">Name</span></span>          | <span data-ttu-id="0a1fc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a1fc-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0a1fc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a1fc-123">Authorization</span></span> | <span data-ttu-id="0a1fc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a1fc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a1fc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a1fc-126">Request body</span></span>
<span data-ttu-id="0a1fc-127">No corpo da solicitação, fornece uma representação JSON de um objeto [onlineMeeting](../resources/onlinemeeting.md) .</span><span class="sxs-lookup"><span data-stu-id="0a1fc-127">In the request body, supply a JSON representation of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0a1fc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a1fc-128">Response</span></span>
<span data-ttu-id="0a1fc-129">Se tiver êxito, este método retornará `201 Created` código de resposta e um objeto [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a1fc-129">If successful, this method returns `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a1fc-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a1fc-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0a1fc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a1fc-131">Request</span></span>
<span data-ttu-id="0a1fc-132">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a1fc-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-onlinemeeting-from-application"
}-->
```http
POST https://graph.microsoft.com/beta/app/onlineMeetings
Content-Type: application/json
Content-Length: 1553

{
  "meetingType": "meetNow",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f"
        }
      }
    }
  },
  "subject": "subject-value"
}
```

<span data-ttu-id="0a1fc-133">No corpo da solicitação, fornece uma representação JSON do objeto [onlineMeeting](../resources/onlinemeeting.md) .</span><span class="sxs-lookup"><span data-stu-id="0a1fc-133">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="0a1fc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a1fc-134">Response</span></span>

><span data-ttu-id="0a1fc-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a1fc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 201 Created
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
  "meetingType": "meetNow",
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
  "startDateTime": "2018-03-19T09:46:02Z",
  "subject": "Quarterly sales numbers"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
