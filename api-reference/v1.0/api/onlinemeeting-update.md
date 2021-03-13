---
title: Atualizar onlineMeeting
description: Atualize as propriedades de uma reunião online.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 934a54b83b85c7096cc8b1a62f35a53fcfbbc169
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773491"
---
# <a name="update-onlinemeeting"></a><span data-ttu-id="5987f-103">Atualizar onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="5987f-103">Update onlineMeeting</span></span>

<span data-ttu-id="5987f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5987f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5987f-105">Atualize as propriedades do objeto [onlineMeeting](../resources/onlinemeeting.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="5987f-105">Update the properties of the specified [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

<span data-ttu-id="5987f-106">Consulte [a seção Solicitar corpo](#request-body) para a lista de propriedades que suportam a atualização.</span><span class="sxs-lookup"><span data-stu-id="5987f-106">Please see [Request body](#request-body) section for the list of properties that support updating.</span></span>

## <a name="permissions"></a><span data-ttu-id="5987f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5987f-107">Permissions</span></span>

| <span data-ttu-id="5987f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5987f-108">Permission type</span></span>                        | <span data-ttu-id="5987f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5987f-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5987f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5987f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5987f-111">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5987f-111">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="5987f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5987f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5987f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5987f-113">Not Supported.</span></span>                              |
| <span data-ttu-id="5987f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5987f-114">Application</span></span>                            | <span data-ttu-id="5987f-115">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="5987f-115">OnlineMeetings.ReadWrite.All\*</span></span>               |

> [!IMPORTANT]
> <span data-ttu-id="5987f-116">\*Os administradores [](/graph/cloud-communication-online-meeting-application-access-policy) devem criar uma política de acesso a aplicativos e concedi-la a um usuário, autorizando o aplicativo configurado na política para atualizar uma reunião online em nome desse usuário (ID do usuário especificada no caminho da solicitação).</span><span class="sxs-lookup"><span data-stu-id="5987f-116">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to update an online meeting on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="5987f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5987f-117">HTTP request</span></span>
<span data-ttu-id="5987f-118">Para atualizar o onlineMeeting especificado por meio da ID de reunião com o token delegado:</span><span class="sxs-lookup"><span data-stu-id="5987f-118">To update the specified onlineMeeting by meeting ID with delegated token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onlineMeetings/{meetingId}
```

<span data-ttu-id="5987f-119">Para atualizar o onlineMeeting especificado pela ID de reunião com o token de aplicativo:</span><span class="sxs-lookup"><span data-stu-id="5987f-119">To update the specified onlineMeeting by meeting ID with application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{userId}/onlineMeetings/{meetingId}
```

> <span data-ttu-id="5987f-120">**Observações:**</span><span class="sxs-lookup"><span data-stu-id="5987f-120">**Notes:**</span></span>
> - <span data-ttu-id="5987f-121">`userId`é a ID do objeto de um usuário no portal de gerenciamento [de usuários do Azure.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="5987f-121">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="5987f-122">Para obter mais detalhes, consulte [política de acesso ao aplicativo](/graph/cloud-communication-online-meeting-application-access-policy).</span><span class="sxs-lookup"><span data-stu-id="5987f-122">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
> - <span data-ttu-id="5987f-123">`meetingId`é a **id** de um [objeto onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="5987f-123">`meetingId` is the **id** of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5987f-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5987f-124">Request headers</span></span>
| <span data-ttu-id="5987f-125">Nome</span><span class="sxs-lookup"><span data-stu-id="5987f-125">Name</span></span>          | <span data-ttu-id="5987f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="5987f-126">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="5987f-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="5987f-127">Authorization</span></span> | <span data-ttu-id="5987f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5987f-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="5987f-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="5987f-130">Content-type</span></span>  | <span data-ttu-id="5987f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5987f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5987f-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5987f-133">Request body</span></span>
<span data-ttu-id="5987f-134">A tabela abaixo lista as propriedades que podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="5987f-134">The table below lists the properties that can be updated.</span></span> <span data-ttu-id="5987f-135">No corpo da solicitação, inclua apenas as propriedades que precisam ser atualizadas, com as seguintes exceções:</span><span class="sxs-lookup"><span data-stu-id="5987f-135">In the request body, include only the properties that need updating, with the following exceptions:</span></span>

- <span data-ttu-id="5987f-136">Ajustar a data/hora inicial ou final de uma reunião online sempre requer as propriedades **startDateTime** e **endDateTime** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5987f-136">Adjusting the start or end date/time of an online meeting always requires both **startDateTime** and **endDateTime** properties in the request body.</span></span>
- <span data-ttu-id="5987f-137">Ajustar o **campo de** participantes  da propriedade participantes, como adicionar ou remover um participante à reunião, sempre requer a lista completa de participantes no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5987f-137">Adjusting the **attendees** field of the **participants** property, such as adding or removing an attendee to the meeting, always requires the full list of attendees in the request body.</span></span>

| <span data-ttu-id="5987f-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5987f-138">Property</span></span>             | <span data-ttu-id="5987f-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="5987f-139">Type</span></span>                                                         | <span data-ttu-id="5987f-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="5987f-140">Description</span></span>                                                                                                                                    |
|----------------------|--------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5987f-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5987f-141">startDateTime</span></span>        | <span data-ttu-id="5987f-142">DateTime</span><span class="sxs-lookup"><span data-stu-id="5987f-142">DateTime</span></span>                                                     | <span data-ttu-id="5987f-143">O horário de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="5987f-143">The meeting start time in UTC.</span></span>                                                                                                                 |
| <span data-ttu-id="5987f-144">endDateTime</span><span class="sxs-lookup"><span data-stu-id="5987f-144">endDateTime</span></span>          | <span data-ttu-id="5987f-145">DateTime</span><span class="sxs-lookup"><span data-stu-id="5987f-145">DateTime</span></span>                                                     | <span data-ttu-id="5987f-146">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="5987f-146">The meeting end time in UTC.</span></span>                                                                                                                   |
| <span data-ttu-id="5987f-147">assunto</span><span class="sxs-lookup"><span data-stu-id="5987f-147">subject</span></span>              | <span data-ttu-id="5987f-148">String</span><span class="sxs-lookup"><span data-stu-id="5987f-148">String</span></span>                                                       | <span data-ttu-id="5987f-149">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="5987f-149">The subject of the online meeting.</span></span>                                                                                                             |
| <span data-ttu-id="5987f-150">participants</span><span class="sxs-lookup"><span data-stu-id="5987f-150">participants</span></span>         | [<span data-ttu-id="5987f-151">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="5987f-151">meetingParticipants</span></span>](../resources/meetingparticipants.md)   | <span data-ttu-id="5987f-152">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="5987f-152">The participants associated with the online meeting.</span></span> <span data-ttu-id="5987f-153">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="5987f-153">This includes the organizer and the attendees.</span></span>                                            |
| <span data-ttu-id="5987f-154">isEntryExitAnnounced</span><span class="sxs-lookup"><span data-stu-id="5987f-154">isEntryExitAnnounced</span></span> | <span data-ttu-id="5987f-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="5987f-155">Boolean</span></span>                                                      | <span data-ttu-id="5987f-156">Se os chamadores ingressarão ou sairão.</span><span class="sxs-lookup"><span data-stu-id="5987f-156">Whether or not to announce when callers join or leave.</span></span>                                                                                         |
| <span data-ttu-id="5987f-157">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="5987f-157">lobbyBypassSettings</span></span>  | [<span data-ttu-id="5987f-158">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="5987f-158">lobbyBypassSettings</span></span>](../resources/lobbyBypassSettings.md)   | <span data-ttu-id="5987f-159">Especifica quais participantes podem ignorar o lobby da reunião.</span><span class="sxs-lookup"><span data-stu-id="5987f-159">Specifies which participants can bypass the meeting lobby.</span></span>                                                                                     |
| <span data-ttu-id="5987f-160">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="5987f-160">allowedPresenters</span></span>    | <span data-ttu-id="5987f-161">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="5987f-161">onlineMeetingPresenters</span></span>                                      | <span data-ttu-id="5987f-162">Especifica quem pode ser um apresentador em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="5987f-162">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="5987f-163">Os valores possíveis são todos, organização, roleIsPresenter, organizador e unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="5987f-163">Possible values are everyone, organization, roleIsPresenter, organizer, and unknownFutureValue.</span></span> |

## <a name="response"></a><span data-ttu-id="5987f-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="5987f-164">Response</span></span>
<span data-ttu-id="5987f-165">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5987f-165">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5987f-166">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5987f-166">Examples</span></span>

### <a name="example-1-update-the-startdatetime-enddatetime-and-subject"></a><span data-ttu-id="5987f-167">Exemplo 1: atualizar o startDateTime, endDateTime e assunto</span><span class="sxs-lookup"><span data-stu-id="5987f-167">Example 1: Update the startDateTime, endDateTime and subject</span></span>

#### <a name="request"></a><span data-ttu-id="5987f-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5987f-168">Request</span></span>

> <span data-ttu-id="5987f-169">**Observação:** A ID da reunião foi truncada para capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="5987f-169">**Note:** The meeting ID has been truncated for readability.</span></span>


# <a name="http"></a>[<span data-ttu-id="5987f-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="5987f-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_start_end_subject"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "startDateTime": "2020-09-09T14:33:30.8546353-07:00",
  "endDateTime": "2020-09-09T15:03:30.8566356-07:00",
  "subject": "Patch Meeting Subject"
}
```
# <a name="c"></a>[<span data-ttu-id="5987f-171">C#</span><span class="sxs-lookup"><span data-stu-id="5987f-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-start-end-subject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5987f-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5987f-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-start-end-subject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5987f-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5987f-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-start-end-subject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5987f-174">Java</span><span class="sxs-lookup"><span data-stu-id="5987f-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-start-end-subject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5987f-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="5987f-175">Response</span></span>

> <span data-ttu-id="5987f-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5987f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "id":"MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi",
   "creationDateTime":"2020-07-03T00:23:39.444642Z",
   "startDateTime":"2020-09-09T21:33:30.8546353Z",
   "endDateTime":"2020-09-09T22:03:30.8566356Z",
   "joinWebUrl":"url",
   "subject":"Patch Meeting Subject",
   "isBroadcast":false,
   "autoAdmittedUsers":"EveryoneInCompany",
   "outerMeetingAutoAdmittedUsers":null,
   "participants":{
      "organizer":{
         "upn":"upn",
         "role": "presenter",
         "identity":{
            "azureApplicationInstance":null,
            "applicationInstance":null,
            "application":null,
            "device":null,
            "user":{
               "id":"8716745d-77a9-4be3-afff-009e4b81658e",
               "displayName":null,
               "tenantId":"0823831b-1f1b-424b-b90a-1caa345a742a",
               "identityProvider":"AAD"
            }
         }
      }
   },
   "audioConferencing":{
      "conferenceId":"id",
      "tollNumber":"+1-900-555-0100",
      "tollFreeNumber":"+1-800-555-0100",
      "dialinUrl":"url"
   }
}
```

#### <a name="example-2-update-the-lobbybypasssettings"></a><span data-ttu-id="5987f-178">Exemplo 2: atualizar o lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="5987f-178">Example 2: Update the lobbyBypassSettings</span></span>
> <span data-ttu-id="5987f-179">**Observação:** A ID da reunião foi truncada para capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="5987f-179">**Note:** The meeting ID has been truncated for readability.</span></span>


# <a name="http"></a>[<span data-ttu-id="5987f-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="5987f-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_lobbyBypassSettings"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "lobbyBypassSettings": {
      "isDialInBypassEnabled": true
  }
}
```
# <a name="c"></a>[<span data-ttu-id="5987f-181">C#</span><span class="sxs-lookup"><span data-stu-id="5987f-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-lobbybypasssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5987f-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5987f-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-lobbybypasssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5987f-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5987f-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-lobbybypasssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5987f-184">Java</span><span class="sxs-lookup"><span data-stu-id="5987f-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-lobbybypasssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5987f-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="5987f-185">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi",
    "creationDateTime":"2020-07-03T00:23:39.444642Z",
    "startDateTime":"2020-09-09T21:33:30.8546353Z",
    "endDateTime":"2020-09-09T22:03:30.8566356Z",
    "joinWebUrl":"(redacted)",
    "subject":"Patch Meeting Subject",
    "autoAdmittedUsers": "EveryoneInCompany",
    "isEntryExitAnnounced": true,
    "allowedPresenters": "everyone",
    "videoTeleconferenceId": "(redacted)",
    "participants": {
        "organizer": {
            "upn": "(redacted)",
            "role": "presenter",
            "identity": {
                "user": {
                    "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4622",
                    "displayName": null,
                    "tenantId": "909c6581-5130-43e9-88f3-fcb3582cde38",
                    "identityProvider": "AAD"
                }
            }
        },
        "attendees": [],
    },
    "lobbyBypassSettings": {
        "scope": "organization",
        "isDialInBypassEnabled": true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-7-16 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch online meeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


