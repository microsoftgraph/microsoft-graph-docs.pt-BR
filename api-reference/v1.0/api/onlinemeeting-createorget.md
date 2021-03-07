---
title: 'onlineMeeting: createOrGet'
description: Crie uma reunião online com uma ID externa especificada personalizada. Se a ID externa já existir, essa API retornará o **objeto onlineMeeting** com essa ID externa.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 27e68b078b22380638047d9a0827459f90e3c5da
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516161"
---
# <a name="onlinemeeting-createorget"></a><span data-ttu-id="09d94-104">onlineMeeting: createOrGet</span><span class="sxs-lookup"><span data-stu-id="09d94-104">onlineMeeting: createOrGet</span></span>

<span data-ttu-id="09d94-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09d94-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="09d94-106">Crie um [objeto onlineMeeting](../resources/onlinemeeting.md) com uma ID externa especificada personalizada.</span><span class="sxs-lookup"><span data-stu-id="09d94-106">Create an [onlineMeeting](../resources/onlinemeeting.md) object with a custom specified external ID.</span></span> <span data-ttu-id="09d94-107">Se a ID externa já existir, essa API retornará o [objeto onlineMeeting](../resources/onlinemeeting.md) com essa ID externa.</span><span class="sxs-lookup"><span data-stu-id="09d94-107">If the external ID already exists, this API will return the [onlineMeeting](../resources/onlinemeeting.md) object with that external ID.</span></span> 

> <span data-ttu-id="09d94-108">**Observação**: a reunião não é exibida no calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="09d94-108">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="09d94-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="09d94-109">Permissions</span></span>
<span data-ttu-id="09d94-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09d94-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09d94-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09d94-112">Permission type</span></span>                        | <span data-ttu-id="09d94-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09d94-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="09d94-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09d94-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="09d94-115">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09d94-115">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="09d94-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09d94-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09d94-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09d94-117">Not supported.</span></span>                               |
| <span data-ttu-id="09d94-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09d94-118">Application</span></span>                            | <span data-ttu-id="09d94-119">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="09d94-119">OnlineMeetings.ReadWrite.All\*</span></span>                |

> [!IMPORTANT]
> <span data-ttu-id="09d94-120">\*Os administradores [](/graph/concepts/cloud-communication-online-meeting-application-access-policy.md) devem criar uma política de acesso a aplicativos e concedi-la a um usuário, autorizando o aplicativo configurado na política para criar ou obter uma reunião online com a ID externa em nome desse usuário (ID do usuário especificada no caminho da solicitação).</span><span class="sxs-lookup"><span data-stu-id="09d94-120">\* Administrators must create an [application access policy](/graph/concepts/cloud-communication-online-meeting-application-access-policy.md) and grant it to a user, authorizing the app configured in the policy to create or get an online meeting with external ID on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="09d94-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09d94-121">HTTP request</span></span>
<span data-ttu-id="09d94-122">Para chamar a API **createOrGet** com token delegado:</span><span class="sxs-lookup"><span data-stu-id="09d94-122">To call **createOrGet** API with delegated token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/createOrGet
```

<span data-ttu-id="09d94-123">Para chamar a API **createOrGet** com token de aplicativo:</span><span class="sxs-lookup"><span data-stu-id="09d94-123">To call **createOrGet** API with application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/onlineMeetings/createOrGet
```

> <span data-ttu-id="09d94-124">**Observação:** `userId` é a ID de objeto de um usuário no [portal de gerenciamento de usuário do Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span><span class="sxs-lookup"><span data-stu-id="09d94-124">**Note:** `userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="09d94-125">Veja mais detalhes na [política](/graph/cloud-communication-online-meeting-application-access-policy) de acesso aos aplicativos.</span><span class="sxs-lookup"><span data-stu-id="09d94-125">See more details in [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>

## <a name="request-headers"></a><span data-ttu-id="09d94-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09d94-126">Request headers</span></span>
| <span data-ttu-id="09d94-127">Nome</span><span class="sxs-lookup"><span data-stu-id="09d94-127">Name</span></span>          | <span data-ttu-id="09d94-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="09d94-128">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="09d94-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="09d94-129">Authorization</span></span> | <span data-ttu-id="09d94-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09d94-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="09d94-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="09d94-132">Content-type</span></span>  | <span data-ttu-id="09d94-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09d94-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09d94-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09d94-135">Request body</span></span>
<span data-ttu-id="09d94-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09d94-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="09d94-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="09d94-137">Parameter</span></span>        | <span data-ttu-id="09d94-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="09d94-138">Type</span></span>                                     |<span data-ttu-id="09d94-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="09d94-139">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:--------------------------------------------------------------------------|
| <span data-ttu-id="09d94-140">endDateTime</span><span class="sxs-lookup"><span data-stu-id="09d94-140">endDateTime</span></span>      | <span data-ttu-id="09d94-141">DateTime</span><span class="sxs-lookup"><span data-stu-id="09d94-141">DateTime</span></span>                                 | <span data-ttu-id="09d94-142">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="09d94-142">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="09d94-143">externalId</span><span class="sxs-lookup"><span data-stu-id="09d94-143">externalId</span></span>       | <span data-ttu-id="09d94-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09d94-144">String</span></span>                                   | <span data-ttu-id="09d94-145">A ID externa.</span><span class="sxs-lookup"><span data-stu-id="09d94-145">The external ID.</span></span> <span data-ttu-id="09d94-146">Uma ID personalizada.</span><span class="sxs-lookup"><span data-stu-id="09d94-146">A custom ID.</span></span> <span data-ttu-id="09d94-147">(Obrigatório)</span><span class="sxs-lookup"><span data-stu-id="09d94-147">(Required)</span></span> |
| <span data-ttu-id="09d94-148">participants</span><span class="sxs-lookup"><span data-stu-id="09d94-148">participants</span></span>     | [<span data-ttu-id="09d94-149">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="09d94-149">meetingParticipants</span></span>](../resources/meetingparticipants.md)          | <span data-ttu-id="09d94-150">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="09d94-150">The participants associated with the online meeting.</span></span>  <span data-ttu-id="09d94-151">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="09d94-151">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="09d94-152">startDateTime</span><span class="sxs-lookup"><span data-stu-id="09d94-152">startDateTime</span></span>    | <span data-ttu-id="09d94-153">DateTime</span><span class="sxs-lookup"><span data-stu-id="09d94-153">DateTime</span></span>                                 | <span data-ttu-id="09d94-154">O horário de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="09d94-154">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="09d94-155">assunto</span><span class="sxs-lookup"><span data-stu-id="09d94-155">subject</span></span>          | <span data-ttu-id="09d94-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09d94-156">String</span></span>                                   | <span data-ttu-id="09d94-157">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="09d94-157">The subject of the online meeting.</span></span> |

> <span data-ttu-id="09d94-158">**Observações:**</span><span class="sxs-lookup"><span data-stu-id="09d94-158">**Notes:**</span></span>
>
> - <span data-ttu-id="09d94-159">Se **o startDateTime** e **endDateTime** não são fornecidos, o **startDateTime** será padrão para o valor dateTime atual e o valor **endDateTime** será igual ao **startDateTime** + 1 hora.</span><span class="sxs-lookup"><span data-stu-id="09d94-159">If the **startDateTime** and **endDateTime** are not provided, the **startDateTime** will default to the current dateTime value and **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="09d94-160">Se o **startDateTime** for fornecido, mas **endDateTime** não for, o valor **endDateTime** será igual ao **startDateTime** + 1 hora.</span><span class="sxs-lookup"><span data-stu-id="09d94-160">If the **startDateTime** is provided, but **endDateTime** is not, the **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="09d94-161">Um erro será lançado se **endDateTime** for fornecido sem **o startDateTime** ou se **endDateTime** for anterior ao **startDateTime**.</span><span class="sxs-lookup"><span data-stu-id="09d94-161">An error will be thrown if the **endDateTime** is provided without the **startDateTime** or if the **endDateTime** is earlier than the **startDateTime**.</span></span>

## <a name="response"></a><span data-ttu-id="09d94-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="09d94-162">Response</span></span>
<span data-ttu-id="09d94-163">Se tiver êxito, este método retornará um código de resposta se uma nova reunião for criada ou um código de resposta se uma reunião existente `201 Created` `200 OK` for recuperada.</span><span class="sxs-lookup"><span data-stu-id="09d94-163">If successful, this method returns a `201 Created` response code if a new meeting is created, or a `200 OK` response code if an existing meeting is retrieved.</span></span> <span data-ttu-id="09d94-164">Em ambos os casos, um [objeto onlineMeeting](../resources/onlinemeeting.md) é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09d94-164">In both cases, an [onlineMeeting](../resources/onlinemeeting.md) object is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="09d94-165">Exemplos</span><span class="sxs-lookup"><span data-stu-id="09d94-165">Examples</span></span>

### <a name="request"></a><span data-ttu-id="09d94-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09d94-166">Request</span></span>

<span data-ttu-id="09d94-167">O exemplo a seguir mostra como criar ou obter uma reunião online com uma ID externa.</span><span class="sxs-lookup"><span data-stu-id="09d94-167">The following example shows how to create or get an online meeting with an external ID.</span></span>


# <a name="http"></a>[<span data-ttu-id="09d94-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="09d94-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-or-get-onlinemeeting"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/onlineMeetings/createOrGet
Content-Type: application/json

{
    "startDateTime": "2020-02-06T01:49:21.3524945+00:00",
    "endDateTime": "2020-02-06T02:19:21.3524945+00:00",
    "subject": "Create a meeting with customId provided",
    "externalId": "7eb8263f-d0e0-4149-bb1c-1f0476083c56",
    "participants": {
        "attendees": [
            {
                "identity": {
                    "user": {
                        "id": "1f35f2e6-9cab-44ad-8d5a-b74c14720000"
                    }
                },
                "upn": "test1@contoso.com"
            }
        ]
    }
}
```
# <a name="c"></a>[<span data-ttu-id="09d94-169">C#</span><span class="sxs-lookup"><span data-stu-id="09d94-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-or-get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09d94-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09d94-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-or-get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09d94-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09d94-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-or-get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="09d94-172">Java</span><span class="sxs-lookup"><span data-stu-id="09d94-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-or-get-onlinemeeting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="09d94-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="09d94-173">Response</span></span>

><span data-ttu-id="09d94-174">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="09d94-174">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "(redacted)",
    "creationDateTime": "2020-09-11T06:30:18.1909168Z",
    "startDateTime": "2020-09-11T06:30:18.0615989Z",
    "endDateTime": "2020-09-11T07:30:18.0615989Z",
    "joinWebUrl": "(redacted)",
    "subject": "Create a meeting with customId provided",
    "isBroadcast": false,
    "autoAdmittedUsers": "EveryoneInCompany",
    "isEntryExitAnnounced": true,
    "allowedPresenters": "everyone",
    "videoTeleconferenceId": "(redacted)",
    "externalId": "7eb8263f-d0e0-4149-bb1c-1f0476083c56",
    "participants": {
        "organizer": {
            "upn": "(redacted)",
            "role": "presenter",
            "identity": {
                "user": {
                    "id": "(redacted)",
                }
            }
        },
        "attendees": [
            {
                "upn": "test1@contoso.com",
                "role": null,
                "identity": {
                    "user": {
                        "id": "1f35f2e6-9cab-44ad-8d5a-b74c14720000",
                    }
                }
            }
        ],
        "producers": [],
        "contributors": []
    },
    "lobbyBypassSettings": {
        "scope": "organization",
        "isDialInBypassEnabled": false
    },
    "audioConferencing": {
        "conferenceId": "(redacted)",
        "tollNumber": "+1 206-485-3005",
        "tollFreeNumber": null,
        "dialinUrl": "https://dialin.teams.microsoft.com/0e73a853-1cc2-436c-b18c-9f53e0a97c24?id=(redacted)"
    },
    "chatInfo": {
        "threadId": "19:7ebda77322dd4505ac4dedb5b67df076@thread.tacv2",
        "messageId": "0",
        "replyChainMessageId": null
    },
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

