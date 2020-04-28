---
title: 'onlineMeeting: createOrGet'
description: Criar uma reunião online com uma ID externa personalizada especificada. Se a ID externa já existir, essa API retornará o objeto [onlineMeeting](../resources/onlinemeeting.md) com essa ID externa.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6ad76e9362643f29ae93dd2daa03e739ba763e03
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916918"
---
# <a name="onlinemeeting-createorget"></a><span data-ttu-id="bdf8d-104">onlineMeeting: createOrGet</span><span class="sxs-lookup"><span data-stu-id="bdf8d-104">onlineMeeting: createOrGet</span></span>

<span data-ttu-id="bdf8d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdf8d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdf8d-106">Criar um objeto [onlineMeeting](../resources/onlinemeeting.md) com uma ID externa personalizada especificada.</span><span class="sxs-lookup"><span data-stu-id="bdf8d-106">Create an [onlineMeeting](../resources/onlinemeeting.md) object with a custom specified external ID.</span></span> <span data-ttu-id="bdf8d-107">Se a ID externa já existir, essa API retornará o objeto [onlineMeeting](../resources/onlinemeeting.md) com essa ID externa.</span><span class="sxs-lookup"><span data-stu-id="bdf8d-107">If the external ID already exists, this API will return the [onlineMeeting](../resources/onlinemeeting.md) object with that external ID.</span></span> 

> <span data-ttu-id="bdf8d-108">**Observação**: a reunião não é exibida no calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="bdf8d-108">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdf8d-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="bdf8d-109">Permissions</span></span>
<span data-ttu-id="bdf8d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdf8d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bdf8d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdf8d-112">Permission type</span></span>                        | <span data-ttu-id="bdf8d-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bdf8d-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bdf8d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdf8d-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="bdf8d-115">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdf8d-115">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="bdf8d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdf8d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdf8d-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="bdf8d-117">Not Supported</span></span>                               |
| <span data-ttu-id="bdf8d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdf8d-118">Application</span></span>                            | <span data-ttu-id="bdf8d-119">Não suportado</span><span class="sxs-lookup"><span data-stu-id="bdf8d-119">Not Supported</span></span>                |

## <a name="http-request"></a><span data-ttu-id="bdf8d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdf8d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/createOrGet
```

## <a name="request-headers"></a><span data-ttu-id="bdf8d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdf8d-121">Request headers</span></span>
| <span data-ttu-id="bdf8d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="bdf8d-122">Name</span></span>          | <span data-ttu-id="bdf8d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdf8d-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="bdf8d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdf8d-124">Authorization</span></span> | <span data-ttu-id="bdf8d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdf8d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bdf8d-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="bdf8d-127">Content-type</span></span>  | <span data-ttu-id="bdf8d-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdf8d-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdf8d-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdf8d-130">Request body</span></span>
<span data-ttu-id="bdf8d-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdf8d-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bdf8d-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bdf8d-132">Parameter</span></span>        | <span data-ttu-id="bdf8d-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdf8d-133">Type</span></span>                                     |<span data-ttu-id="bdf8d-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdf8d-134">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:--------------------------------------------------------------------------|
| <span data-ttu-id="bdf8d-135">chatInfo</span><span class="sxs-lookup"><span data-stu-id="bdf8d-135">chatInfo</span></span>         |[<span data-ttu-id="bdf8d-136">chatInfo</span><span class="sxs-lookup"><span data-stu-id="bdf8d-136">chatInfo</span></span>](../resources/chatinfo.md)                   |<span data-ttu-id="bdf8d-137">As informações de chat associadas a esta reunião online.</span><span class="sxs-lookup"><span data-stu-id="bdf8d-137">The chat information associated with this online meeting.</span></span>|
| <span data-ttu-id="bdf8d-138">endDateTime</span><span class="sxs-lookup"><span data-stu-id="bdf8d-138">endDateTime</span></span>      | <span data-ttu-id="bdf8d-139">DateTime</span><span class="sxs-lookup"><span data-stu-id="bdf8d-139">DateTime</span></span>                                 | <span data-ttu-id="bdf8d-140">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="bdf8d-140">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="bdf8d-141">externalId</span><span class="sxs-lookup"><span data-stu-id="bdf8d-141">externalId</span></span>       | <span data-ttu-id="bdf8d-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdf8d-142">String</span></span>                                   | <span data-ttu-id="bdf8d-143">A ID externa.</span><span class="sxs-lookup"><span data-stu-id="bdf8d-143">The external ID.</span></span> <span data-ttu-id="bdf8d-144">Uma ID personalizada.</span><span class="sxs-lookup"><span data-stu-id="bdf8d-144">A custom ID.</span></span> <span data-ttu-id="bdf8d-145">Precisam</span><span class="sxs-lookup"><span data-stu-id="bdf8d-145">(Required)</span></span> |
| <span data-ttu-id="bdf8d-146">participants</span><span class="sxs-lookup"><span data-stu-id="bdf8d-146">participants</span></span>     | [<span data-ttu-id="bdf8d-147">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="bdf8d-147">meetingParticipants</span></span>](../resources/meetingparticipants.md)          | <span data-ttu-id="bdf8d-148">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="bdf8d-148">The participants associated with the online meeting.</span></span>  <span data-ttu-id="bdf8d-149">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="bdf8d-149">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="bdf8d-150">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bdf8d-150">startDateTime</span></span>    | <span data-ttu-id="bdf8d-151">DateTime</span><span class="sxs-lookup"><span data-stu-id="bdf8d-151">DateTime</span></span>                                 | <span data-ttu-id="bdf8d-152">A hora de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="bdf8d-152">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="bdf8d-153">assunto</span><span class="sxs-lookup"><span data-stu-id="bdf8d-153">subject</span></span>          | <span data-ttu-id="bdf8d-154">String</span><span class="sxs-lookup"><span data-stu-id="bdf8d-154">String</span></span>                                   | <span data-ttu-id="bdf8d-155">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="bdf8d-155">The subject of the online meeting.</span></span> |

><span data-ttu-id="bdf8d-156">**Observação:** Se o ' startDatetime ' e ' EndDateTime ' não forem fornecidos, os valores padrão serão o valor de DateTime padrão para o sistema.</span><span class="sxs-lookup"><span data-stu-id="bdf8d-156">**Note:** If the 'startDateTime' and 'endDateTime' are not provided, the values will default to the datetime value that is default to the system.</span></span> <span data-ttu-id="bdf8d-157">Em C#, esse valor é "01/01/0001"</span><span class="sxs-lookup"><span data-stu-id="bdf8d-157">In C#, that value is  "01/01/0001"</span></span>

## <a name="response"></a><span data-ttu-id="bdf8d-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdf8d-158">Response</span></span>
<span data-ttu-id="bdf8d-159">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdf8d-159">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bdf8d-160">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bdf8d-160">Examples</span></span>

<span data-ttu-id="bdf8d-161">O exemplo a seguir mostra como criar ou obter uma reunião online com uma ID externa.</span><span class="sxs-lookup"><span data-stu-id="bdf8d-161">The following example shows how to create or get an online meeting with an external ID.</span></span>

### <a name="request"></a><span data-ttu-id="bdf8d-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdf8d-162">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bdf8d-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="bdf8d-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-or-get-onlinemeeting"
}-->

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/createOrGet
Content-Type: application/json

{
  "chatInfo": {
    "threadId":"19%3A3b52398f3c524556894b776357c1dd79%40thread.skype"
  },
  "startDateTime": "2020-02-06T01:49:21.3524945+00:00",
  "endDateTime": "2020-02-06T02:19:21.3524945+00:00",
  "externalId": "7eb8263f-d0e0-4149-bb1c-1f0476083c56",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "d4a060b5-a8fc-450c-837b-750b2c280000",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd0110000"
        }
      },
      "upn": "test1@contoso.com"
    },
    "attendees": [
      {
        "identity": {
          "user": {
            "id": "1f35f2e6-9cab-44ad-8d5a-b74c14720000",
            "identityProvider": "MSA"
          }
        },
        "upn": "test@contoso.com"
      }
    ]
  },
  "subject":"Create a meeting with customId provided"
}
```
# <a name="c"></a>[<span data-ttu-id="bdf8d-164">C#</span><span class="sxs-lookup"><span data-stu-id="bdf8d-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-or-get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bdf8d-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bdf8d-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-or-get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bdf8d-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bdf8d-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-or-get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bdf8d-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdf8d-167">Response</span></span>

><span data-ttu-id="bdf8d-168">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bdf8d-168">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "creationDateTime": "2020-02-06T01:50:10.7396692+00:00",
  "startDateTime": "2020-02-06T01:49:21.3524945+00:00",
  "endDateTime": "2020-02-06T02:19:21.3524945+00:00",
 "joinWebUrl": "https://devspaces.skype.com/l/meetup-join/19%3ameeting_MWE2Y2U2NGYtMjk4Ni00NjYyLWEyMjItYjk3MGU4YzFh0000%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22d4a060b5-a8fc-450c-837b-750b2c2869b5%22%7d",
  "subject": "Create a meeting with customId provided",
  "participants": {
    "@odata.type": "#microsoft.graph.meetingParticipants",
    "organizer": {
      "@odata.type": "#microsoft.graph.meetingParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "d4a060b5-a8fc-450c-837b-750b2c280000",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd0110000",
          "displayName": "Tyler Stein",
          "identityProvider": "AAD"
        }
      },
      "upn": "test1@contoso.com"
    },
    "attendees": [
      {
        "@odata.type": "#microsoft.graph.meetingParticipantInfo",
        "identity": {
          "@odata.type": "#microsoft.graph.identitySet",
          "user": {
            "@odata.type": "#microsoft.graph.identity",
            "id": "1f35f2e6-9cab-44ad-8d5a-b74c14720000",
            "displayName": "Jasmine Miller",
            "identityProvider": "MSA"
          }
        },
        "upn": "test@contoso.com"
      }
    ],
    "producers": [],
    "contributors": []
  },
  "isBroadcast": false,
  "autoAdmittedUsers": "everyone",
  "capabilities": [],
  "audioConferencing": {
    "@odata.type": "#microsoft.graph.audioConferencing",
    "conferenceId": "804980000",
    "tollNumber": "555-749-0000",
    "dialinUrl": "https://dialin.teams.microsoft.com/8bf6e654-57eb-4b85-aeaf-36c84429b2fe?id=804980000"
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:meeting_MWE2Y2U2NGYtMjk4Ni00NjYyLWEyMjItYjk3MGU4YzFh0000@thread.v2",
    "messageId": "0"
  },
  "videoTeleconferenceId": "5556440000",
  "externalId": "7eb8263f-d0e0-4149-bb1c-1f0476083c56",
  "id": "d4a060b5-a8fc-450c-837b-750b2c2869b5_19:meeting_MWE2Y2U2NGYtMjk4Ni00NjYyLWEyMjItYjk3MGU4YzFh0000@thread.v2",
  "@odata.context": "http://localhost/$metadata#onlineMeetings/$entity",
  "outerMeetingAutoAdmittedUsers": null,
  "meetingInfo": null
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
