---
title: 'onlineMeeting: createOrGet'
description: Criar uma reunião online com uma ID externa personalizada especificada. Se a ID externa já existir, essa API retornará o objeto **onlineMeeting** com essa ID externa.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: dfb4d697df9d49f177510097ffa5dddfe255f12a
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 09/16/2020
ms.locfileid: "47842817"
---
# <a name="onlinemeeting-createorget"></a><span data-ttu-id="c084b-104">onlineMeeting: createOrGet</span><span class="sxs-lookup"><span data-stu-id="c084b-104">onlineMeeting: createOrGet</span></span>

<span data-ttu-id="c084b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c084b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c084b-106">Criar um objeto [onlineMeeting](../resources/onlinemeeting.md) com uma ID externa personalizada especificada.</span><span class="sxs-lookup"><span data-stu-id="c084b-106">Create an [onlineMeeting](../resources/onlinemeeting.md) object with a custom specified external ID.</span></span> <span data-ttu-id="c084b-107">Se a ID externa já existir, essa API retornará o objeto [onlineMeeting](../resources/onlinemeeting.md) com essa ID externa.</span><span class="sxs-lookup"><span data-stu-id="c084b-107">If the external ID already exists, this API will return the [onlineMeeting](../resources/onlinemeeting.md) object with that external ID.</span></span> 

> <span data-ttu-id="c084b-108">**Observação**: a reunião não é exibida no calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="c084b-108">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="c084b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c084b-109">Permissions</span></span>
<span data-ttu-id="c084b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c084b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c084b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c084b-112">Permission type</span></span>                        | <span data-ttu-id="c084b-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c084b-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c084b-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c084b-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c084b-115">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c084b-115">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="c084b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c084b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c084b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c084b-117">Not supported.</span></span>                               |
| <span data-ttu-id="c084b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c084b-118">Application</span></span>                            | <span data-ttu-id="c084b-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c084b-119">Not supported.</span></span>                |

## <a name="http-request"></a><span data-ttu-id="c084b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c084b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/createOrGet
```

## <a name="request-headers"></a><span data-ttu-id="c084b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c084b-121">Request headers</span></span>
| <span data-ttu-id="c084b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c084b-122">Name</span></span>          | <span data-ttu-id="c084b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c084b-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c084b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c084b-124">Authorization</span></span> | <span data-ttu-id="c084b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c084b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c084b-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="c084b-127">Content-type</span></span>  | <span data-ttu-id="c084b-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c084b-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c084b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c084b-130">Request body</span></span>
<span data-ttu-id="c084b-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c084b-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c084b-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c084b-132">Parameter</span></span>        | <span data-ttu-id="c084b-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c084b-133">Type</span></span>                                     |<span data-ttu-id="c084b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c084b-134">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:--------------------------------------------------------------------------|
| <span data-ttu-id="c084b-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c084b-135">endDateTime</span></span>      | <span data-ttu-id="c084b-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="c084b-136">DateTime</span></span>                                 | <span data-ttu-id="c084b-137">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="c084b-137">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="c084b-138">externalId</span><span class="sxs-lookup"><span data-stu-id="c084b-138">externalId</span></span>       | <span data-ttu-id="c084b-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c084b-139">String</span></span>                                   | <span data-ttu-id="c084b-140">A ID externa.</span><span class="sxs-lookup"><span data-stu-id="c084b-140">The external ID.</span></span> <span data-ttu-id="c084b-141">Uma ID personalizada.</span><span class="sxs-lookup"><span data-stu-id="c084b-141">A custom ID.</span></span> <span data-ttu-id="c084b-142">Precisam</span><span class="sxs-lookup"><span data-stu-id="c084b-142">(Required)</span></span> |
| <span data-ttu-id="c084b-143">participants</span><span class="sxs-lookup"><span data-stu-id="c084b-143">participants</span></span>     | [<span data-ttu-id="c084b-144">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="c084b-144">meetingParticipants</span></span>](../resources/meetingparticipants.md)          | <span data-ttu-id="c084b-145">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="c084b-145">The participants associated with the online meeting.</span></span>  <span data-ttu-id="c084b-146">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="c084b-146">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="c084b-147">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c084b-147">startDateTime</span></span>    | <span data-ttu-id="c084b-148">DateTime</span><span class="sxs-lookup"><span data-stu-id="c084b-148">DateTime</span></span>                                 | <span data-ttu-id="c084b-149">A hora de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="c084b-149">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="c084b-150">assunto</span><span class="sxs-lookup"><span data-stu-id="c084b-150">subject</span></span>          | <span data-ttu-id="c084b-151">String</span><span class="sxs-lookup"><span data-stu-id="c084b-151">String</span></span>                                   | <span data-ttu-id="c084b-152">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="c084b-152">The subject of the online meeting.</span></span> |

> <span data-ttu-id="c084b-153">**Observações:**</span><span class="sxs-lookup"><span data-stu-id="c084b-153">**Notes:**</span></span>
>
> - <span data-ttu-id="c084b-154">Se o **StartDateTime** e **EndDateTime** não forem fornecidos, o **StartDateTime** será o padrão para o valor dateTime **atual e o valor EndDateTime será** igual a **StartDateTime** + 1 hora.</span><span class="sxs-lookup"><span data-stu-id="c084b-154">If the **startDateTime** and **endDateTime** are not provided, the **startDateTime** will default to the current dateTime value and **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="c084b-155">Se **StartDateTime** for fornecido, mas **EndDateTime** não for, o valor **EndDateTime** será igual a **StartDateTime** + 1 hora.</span><span class="sxs-lookup"><span data-stu-id="c084b-155">If the **startDateTime** is provided, but **endDateTime** is not, the **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="c084b-156">Um erro será gerado se **EndDateTime** for fornecido sem o **StartDateTime** ou se **EndDateTime** for anterior ao **StartDateTime**.</span><span class="sxs-lookup"><span data-stu-id="c084b-156">An error will be thrown if the **endDateTime** is provided without the **startDateTime** or if the **endDateTime** is earlier than the **startDateTime**.</span></span>

## <a name="response"></a><span data-ttu-id="c084b-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="c084b-157">Response</span></span>
<span data-ttu-id="c084b-158">Se tiver êxito, este método retornará um `201 Created` código de resposta se uma nova reunião for criada ou um `200 OK` código de resposta se uma reunião existente for recuperada.</span><span class="sxs-lookup"><span data-stu-id="c084b-158">If successful, this method returns a `201 Created` response code if a new meeting is created, or a `200 OK` response code if an existing meeting is retrieved.</span></span> <span data-ttu-id="c084b-159">Em ambos os casos, um objeto [onlineMeeting](../resources/onlinemeeting.md) é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c084b-159">In both cases, an [onlineMeeting](../resources/onlinemeeting.md) object is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c084b-160">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c084b-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c084b-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c084b-161">Request</span></span>

<span data-ttu-id="c084b-162">O exemplo a seguir mostra como criar ou obter uma reunião online com uma ID externa.</span><span class="sxs-lookup"><span data-stu-id="c084b-162">The following example shows how to create or get an online meeting with an external ID.</span></span>


# <a name="http"></a>[<span data-ttu-id="c084b-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="c084b-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c084b-164">C#</span><span class="sxs-lookup"><span data-stu-id="c084b-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-or-get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c084b-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c084b-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-or-get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c084b-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c084b-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-or-get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c084b-167">Java</span><span class="sxs-lookup"><span data-stu-id="c084b-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-or-get-onlinemeeting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c084b-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="c084b-168">Response</span></span>

><span data-ttu-id="c084b-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c084b-169">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
