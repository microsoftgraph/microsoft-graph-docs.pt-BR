---
title: 'onlineMeeting: createOrGet'
description: Criar uma reunião online com uma ID externa personalizada especificada. Se a ID externa já existir, essa API retornará o objeto onlineMeeting com essa ID externa.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: c66b3ccdf0ddc5e60b68b34c546193b8081d2c69
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/16/2020
ms.locfileid: "47842775"
---
# <a name="onlinemeeting-createorget"></a><span data-ttu-id="f1e0b-104">onlineMeeting: createOrGet</span><span class="sxs-lookup"><span data-stu-id="f1e0b-104">onlineMeeting: createOrGet</span></span>

<span data-ttu-id="f1e0b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1e0b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1e0b-106">Criar um objeto [onlineMeeting](../resources/onlinemeeting.md) com uma ID externa personalizada especificada.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-106">Create an [onlineMeeting](../resources/onlinemeeting.md) object with a custom specified external ID.</span></span> <span data-ttu-id="f1e0b-107">Se a ID externa já existir, essa API retornará o objeto [onlineMeeting](../resources/onlinemeeting.md) com essa ID externa.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-107">If the external ID already exists, this API will return the [onlineMeeting](../resources/onlinemeeting.md) object with that external ID.</span></span> 

> <span data-ttu-id="f1e0b-108">**Observação**: a reunião não é exibida no calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-108">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1e0b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1e0b-109">Permissions</span></span>
<span data-ttu-id="f1e0b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1e0b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f1e0b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1e0b-112">Permission type</span></span>                        | <span data-ttu-id="f1e0b-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1e0b-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f1e0b-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1e0b-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1e0b-115">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1e0b-115">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="f1e0b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1e0b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1e0b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-117">Not Supported.</span></span>                              |
| <span data-ttu-id="f1e0b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1e0b-118">Application</span></span>                            | <span data-ttu-id="f1e0b-119">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="f1e0b-119">OnlineMeetings.ReadWrite.All\*</span></span>                |

> [!IMPORTANT]
> <span data-ttu-id="f1e0b-120">\* Os administradores devem criar uma [política de acesso de aplicativo](/graph/concepts/cloud-communication-online-meeting-application-access-policy.md) e conceder a ele um usuário, autorizando o aplicativo configurado na política para criar ou obter uma reunião online com ID externa em nome desse usuário (ID de usuário especificada no caminho da solicitação).</span><span class="sxs-lookup"><span data-stu-id="f1e0b-120">\* Administrators must create an [application access policy](/graph/concepts/cloud-communication-online-meeting-application-access-policy.md) and grant it to a user, authorizing the app configured in the policy to create or get an online meeting with external ID on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="f1e0b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1e0b-121">HTTP request</span></span>

<span data-ttu-id="f1e0b-122">Solicitação ao usar um token delegado:</span><span class="sxs-lookup"><span data-stu-id="f1e0b-122">Request when using a delegated token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/createOrGet
```

<span data-ttu-id="f1e0b-123">Solicitação ao usar um token de aplicativo:</span><span class="sxs-lookup"><span data-stu-id="f1e0b-123">Request when using an application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/onlineMeetings/createOrGet
```

> <span data-ttu-id="f1e0b-124">**Observação:** `userId` é a ID de objeto de um usuário no [portal de gerenciamento do usuário do Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span><span class="sxs-lookup"><span data-stu-id="f1e0b-124">**Note:** `userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="f1e0b-125">Veja mais detalhes na [política de acesso de aplicativo](/graph/concepts/cloud-communication-online-meeting-application-access-policy.md).</span><span class="sxs-lookup"><span data-stu-id="f1e0b-125">See more details in [application access policy](/graph/concepts/cloud-communication-online-meeting-application-access-policy.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1e0b-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1e0b-126">Request headers</span></span>
| <span data-ttu-id="f1e0b-127">Nome</span><span class="sxs-lookup"><span data-stu-id="f1e0b-127">Name</span></span>          | <span data-ttu-id="f1e0b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1e0b-128">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="f1e0b-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1e0b-129">Authorization</span></span> | <span data-ttu-id="f1e0b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="f1e0b-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="f1e0b-132">Content-type</span></span>  | <span data-ttu-id="f1e0b-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1e0b-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1e0b-135">Request body</span></span>
<span data-ttu-id="f1e0b-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f1e0b-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f1e0b-137">Parameter</span></span>     | <span data-ttu-id="f1e0b-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1e0b-138">Type</span></span>                                                       | <span data-ttu-id="f1e0b-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1e0b-139">Description</span></span>                                                                                          |
| :------------ | :--------------------------------------------------------- | :--------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f1e0b-140">chatInfo</span><span class="sxs-lookup"><span data-stu-id="f1e0b-140">chatInfo</span></span>      | [<span data-ttu-id="f1e0b-141">chatInfo</span><span class="sxs-lookup"><span data-stu-id="f1e0b-141">chatInfo</span></span>](../resources/chatinfo.md)                       | <span data-ttu-id="f1e0b-142">As informações de chat associadas a esta reunião online.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-142">The chat information associated with this online meeting.</span></span>                                            |
| <span data-ttu-id="f1e0b-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f1e0b-143">endDateTime</span></span>   | <span data-ttu-id="f1e0b-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="f1e0b-144">DateTime</span></span>                                                   | <span data-ttu-id="f1e0b-145">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-145">The meeting end time in UTC.</span></span>                                                                         |
| <span data-ttu-id="f1e0b-146">externalId</span><span class="sxs-lookup"><span data-stu-id="f1e0b-146">externalId</span></span>    | <span data-ttu-id="f1e0b-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1e0b-147">String</span></span>                                                     | <span data-ttu-id="f1e0b-148">A ID externa.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-148">The external ID.</span></span> <span data-ttu-id="f1e0b-149">Uma ID personalizada.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-149">A custom ID.</span></span> <span data-ttu-id="f1e0b-150">Precisam</span><span class="sxs-lookup"><span data-stu-id="f1e0b-150">(Required)</span></span>                                                             |
| <span data-ttu-id="f1e0b-151">participants</span><span class="sxs-lookup"><span data-stu-id="f1e0b-151">participants</span></span>  | [<span data-ttu-id="f1e0b-152">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="f1e0b-152">meetingParticipants</span></span>](../resources/meetingparticipants.md) | <span data-ttu-id="f1e0b-153">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-153">The participants associated with the online meeting.</span></span>  <span data-ttu-id="f1e0b-154">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-154">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="f1e0b-155">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f1e0b-155">startDateTime</span></span> | <span data-ttu-id="f1e0b-156">DateTime</span><span class="sxs-lookup"><span data-stu-id="f1e0b-156">DateTime</span></span>                                                   | <span data-ttu-id="f1e0b-157">A hora de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-157">The meeting start time in UTC.</span></span>                                                                       |
| <span data-ttu-id="f1e0b-158">assunto</span><span class="sxs-lookup"><span data-stu-id="f1e0b-158">subject</span></span>       | <span data-ttu-id="f1e0b-159">String</span><span class="sxs-lookup"><span data-stu-id="f1e0b-159">String</span></span>                                                     | <span data-ttu-id="f1e0b-160">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-160">The subject of the online meeting.</span></span>                                                                   |

> <span data-ttu-id="f1e0b-161">**Observações:**</span><span class="sxs-lookup"><span data-stu-id="f1e0b-161">**Notes:**</span></span>
>
> - <span data-ttu-id="f1e0b-162">Se o **StartDateTime** e **EndDateTime** não forem fornecidos, o **StartDateTime** será o padrão para o valor dateTime **atual e o valor EndDateTime será** igual a **StartDateTime** + 1 hora.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-162">If the **startDateTime** and **endDateTime** are not provided, the **startDateTime** will default to the current dateTime value and **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="f1e0b-163">Se **StartDateTime** for fornecido, mas **EndDateTime** não for, o valor **EndDateTime** será igual a **StartDateTime** + 1 hora.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-163">If the **startDateTime** is provided, but **endDateTime** is not, the **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="f1e0b-164">Um erro será gerado se **EndDateTime** for fornecido sem o **StartDateTime** ou se **EndDateTime** for anterior ao **StartDateTime**.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-164">An error will be thrown if the **endDateTime** is provided without the **startDateTime** or if the **endDateTime** is earlier than the **startDateTime**.</span></span>
>
> - <span data-ttu-id="f1e0b-165">Atualmente, o **chatInfo** só tem suporte na versão beta.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-165">Currently **chatInfo** is only supported in beta.</span></span>

## <a name="response"></a><span data-ttu-id="f1e0b-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1e0b-166">Response</span></span>
<span data-ttu-id="f1e0b-167">Se tiver êxito, este método retornará um `201 Created` código de resposta se uma nova reunião for criada ou um `200 OK` código de resposta se uma reunião existente for recuperada.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-167">If successful, this method returns a `201 Created` response code if a new meeting is created, or a `200 OK` response code if an existing meeting is retrieved.</span></span> <span data-ttu-id="f1e0b-168">Em ambos os casos, um objeto [onlineMeeting](../resources/onlinemeeting.md) é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-168">In both cases, an [onlineMeeting](../resources/onlinemeeting.md) object is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f1e0b-169">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f1e0b-169">Examples</span></span>

### <a name="example-1-create-or-get-an-online-meeting-with-an-external-id"></a><span data-ttu-id="f1e0b-170">Exemplo 1: criar ou obter uma reunião online com uma ID externa</span><span class="sxs-lookup"><span data-stu-id="f1e0b-170">Example 1: Create or get an online meeting with an external ID</span></span>

#### <a name="request"></a><span data-ttu-id="f1e0b-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1e0b-171">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f1e0b-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1e0b-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-or-get-onlinemeeting"
}-->

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/createOrGet
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
# <a name="c"></a>[<span data-ttu-id="f1e0b-173">C#</span><span class="sxs-lookup"><span data-stu-id="f1e0b-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-or-get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1e0b-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1e0b-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-or-get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1e0b-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1e0b-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-or-get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f1e0b-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1e0b-176">Response</span></span>

><span data-ttu-id="f1e0b-177">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-177">**Note:** The response object shown here might be shortened for readability.</span></span> 

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


### <a name="example-2-create-or-get-an-online-meeting-in-a-microsoft-teams-channel-with-an-external-id"></a><span data-ttu-id="f1e0b-178">Exemplo 2: criar ou obter uma reunião online em um canal do Microsoft Teams com uma ID externa</span><span class="sxs-lookup"><span data-stu-id="f1e0b-178">Example 2: Create or get an online meeting in a Microsoft Teams channel with an external ID</span></span>

#### <a name="request"></a><span data-ttu-id="f1e0b-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1e0b-179">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create-or-get-onlinemeeting"
}-->
```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/createOrGet
Content-Type: application/json

{
    "chatInfo": {
        "threadId": "19:7ebda77322dd4505ac4dedb5b67df076@thread.tacv2"
    },
    "startDateTime": "2020-02-06T01:49:21.3524945+00:00",
    "endDateTime": "2020-02-06T02:19:21.3524945+00:00",
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
    },
    "subject": "Create a meeting with customId provided"
}
```

#### <a name="response"></a><span data-ttu-id="f1e0b-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1e0b-180">Response</span></span>

><span data-ttu-id="f1e0b-181">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f1e0b-181">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
        "messageId": "1599805818399",
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
