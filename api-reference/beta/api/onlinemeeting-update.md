---
title: Atualizar onlineMeeting
description: Atualize as propriedades de uma reunião online.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8c6023f8893ced851ee7c79b3ed63314a4a9c510
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038217"
---
# <a name="update-onlinemeeting"></a><span data-ttu-id="5b63d-103">Atualizar onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="5b63d-103">Update onlineMeeting</span></span>

<span data-ttu-id="5b63d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b63d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b63d-105">Atualize as propriedades do objeto [onlineMeeting](../resources/onlinemeeting.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="5b63d-105">Update the properties of the specified [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

<span data-ttu-id="5b63d-106">Consulte [a seção Solicitar corpo](#request-body) para a lista de propriedades que suportam a atualização.</span><span class="sxs-lookup"><span data-stu-id="5b63d-106">Please see [Request body](#request-body) section for the list of properties that support updating.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b63d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b63d-107">Permissions</span></span>

| <span data-ttu-id="5b63d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b63d-108">Permission type</span></span>                        | <span data-ttu-id="5b63d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b63d-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5b63d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b63d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b63d-111">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b63d-111">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="5b63d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b63d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b63d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b63d-113">Not Supported.</span></span>                              |
| <span data-ttu-id="5b63d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b63d-114">Application</span></span>                            | <span data-ttu-id="5b63d-115">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="5b63d-115">OnlineMeetings.ReadWrite.All\*</span></span>                |

> [!IMPORTANT]
> <span data-ttu-id="5b63d-116">\*Os administradores [](/graph/cloud-communication-online-meeting-application-access-policy) devem criar uma política de acesso a aplicativos e concedi-la a um usuário, autorizando o aplicativo configurado na política para atualizar uma reunião online em nome desse usuário (ID do usuário especificada no caminho da solicitação).</span><span class="sxs-lookup"><span data-stu-id="5b63d-116">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to update an online meeting on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="5b63d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b63d-117">HTTP request</span></span>
<span data-ttu-id="5b63d-118">Para atualizar o onlineMeeting especificado por meio da ID de reunião com o token delegado:</span><span class="sxs-lookup"><span data-stu-id="5b63d-118">To update the specified onlineMeeting by meeting ID with delegated token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onlineMeetings/{meetingId}
```

<span data-ttu-id="5b63d-119">Para atualizar o onlineMeeting especificado pela ID de reunião com o token de aplicativo:</span><span class="sxs-lookup"><span data-stu-id="5b63d-119">To update the specified onlineMeeting by meeting ID with application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{userId}/onlineMeetings/{meetingId}
```

> [!NOTE]
> - <span data-ttu-id="5b63d-120">`userId` é a ID de objeto de um usuário no [Portal de gerenciamento de usuário do Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span><span class="sxs-lookup"><span data-stu-id="5b63d-120">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="5b63d-121">Para obter mais detalhes, consulte [política de acesso ao aplicativo](/graph/cloud-communication-online-meeting-application-access-policy).</span><span class="sxs-lookup"><span data-stu-id="5b63d-121">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
> - <span data-ttu-id="5b63d-122">`meetingId`é a **id** de um [objeto onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="5b63d-122">`meetingId` is the **id** of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b63d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b63d-123">Request headers</span></span>
| <span data-ttu-id="5b63d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="5b63d-124">Name</span></span>          | <span data-ttu-id="5b63d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b63d-125">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="5b63d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b63d-126">Authorization</span></span> | <span data-ttu-id="5b63d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b63d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="5b63d-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="5b63d-129">Content-type</span></span>  | <span data-ttu-id="5b63d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b63d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b63d-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b63d-132">Request body</span></span>
<span data-ttu-id="5b63d-133">A tabela abaixo lista as propriedades que podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="5b63d-133">The table below lists the properties that can be updated.</span></span> <span data-ttu-id="5b63d-134">No corpo da solicitação, inclua apenas as propriedades que precisam ser atualizadas, com as seguintes exceções:</span><span class="sxs-lookup"><span data-stu-id="5b63d-134">In the request body, include only the properties that need updating, with the following exceptions:</span></span>

- <span data-ttu-id="5b63d-135">Ajustar a data/hora inicial ou final de uma reunião online sempre requer as propriedades **startDateTime** e **endDateTime** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b63d-135">Adjusting the start or end date/time of an online meeting always requires both **startDateTime** and **endDateTime** properties in the request body.</span></span>
- <span data-ttu-id="5b63d-136">Ajustar o **campo de** participantes  da propriedade participantes, como adicionar ou remover um participante à reunião, sempre requer a lista completa de participantes no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b63d-136">Adjusting the **attendees** field of the **participants** property, such as adding or removing an attendee to the meeting, always requires the full list of attendees in the request body.</span></span>

| <span data-ttu-id="5b63d-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b63d-137">Property</span></span>             | <span data-ttu-id="5b63d-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b63d-138">Type</span></span>                                                         | <span data-ttu-id="5b63d-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b63d-139">Description</span></span>                                                                                                                                    |
|----------------------|--------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5b63d-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5b63d-140">startDateTime</span></span>        | <span data-ttu-id="5b63d-141">DateTime</span><span class="sxs-lookup"><span data-stu-id="5b63d-141">DateTime</span></span>                                                     | <span data-ttu-id="5b63d-142">O horário de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="5b63d-142">The meeting start time in UTC.</span></span>                                                                                                                 |
| <span data-ttu-id="5b63d-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="5b63d-143">endDateTime</span></span>          | <span data-ttu-id="5b63d-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="5b63d-144">DateTime</span></span>                                                     | <span data-ttu-id="5b63d-145">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="5b63d-145">The meeting end time in UTC.</span></span>                                                                                                                   |
| <span data-ttu-id="5b63d-146">assunto</span><span class="sxs-lookup"><span data-stu-id="5b63d-146">subject</span></span>              | <span data-ttu-id="5b63d-147">String</span><span class="sxs-lookup"><span data-stu-id="5b63d-147">String</span></span>                                                       | <span data-ttu-id="5b63d-148">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="5b63d-148">The subject of the online meeting.</span></span>                                                                                                             |
| <span data-ttu-id="5b63d-149">participants</span><span class="sxs-lookup"><span data-stu-id="5b63d-149">participants</span></span>         | [<span data-ttu-id="5b63d-150">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="5b63d-150">meetingParticipants</span></span>](../resources/meetingparticipants.md)   | <span data-ttu-id="5b63d-151">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="5b63d-151">The participants associated with the online meeting.</span></span> <span data-ttu-id="5b63d-152">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="5b63d-152">This includes the organizer and the attendees.</span></span>                                            |
| <span data-ttu-id="5b63d-153">isEntryExitAnnounced</span><span class="sxs-lookup"><span data-stu-id="5b63d-153">isEntryExitAnnounced</span></span> | <span data-ttu-id="5b63d-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b63d-154">Boolean</span></span>                                                      | <span data-ttu-id="5b63d-155">Se os chamadores ingressarão ou sairão.</span><span class="sxs-lookup"><span data-stu-id="5b63d-155">Whether or not to announce when callers join or leave.</span></span>                                                                                         |
| <span data-ttu-id="5b63d-156">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="5b63d-156">lobbyBypassSettings</span></span>  | [<span data-ttu-id="5b63d-157">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="5b63d-157">lobbyBypassSettings</span></span>](../resources/lobbyBypassSettings.md)   | <span data-ttu-id="5b63d-158">Especifica quais participantes podem ignorar o lobby da reunião.</span><span class="sxs-lookup"><span data-stu-id="5b63d-158">Specifies which participants can bypass the meeting lobby.</span></span>                                                                                     |
| <span data-ttu-id="5b63d-159">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="5b63d-159">allowedPresenters</span></span>    | <span data-ttu-id="5b63d-160">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="5b63d-160">onlineMeetingPresenters</span></span>                                      | <span data-ttu-id="5b63d-161">Especifica quem pode ser um apresentador em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="5b63d-161">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="5b63d-162">Os valores possíveis são todos, organização, roleIsPresenter, organizador e unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="5b63d-162">Possible values are everyone, organization, roleIsPresenter, organizer, and unknownFutureValue.</span></span> |

## <a name="response"></a><span data-ttu-id="5b63d-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b63d-163">Response</span></span>
<span data-ttu-id="5b63d-164">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b63d-164">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5b63d-165">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5b63d-165">Examples</span></span>

### <a name="example-1-update-the-startdatetime-enddatetime-and-subject"></a><span data-ttu-id="5b63d-166">Exemplo 1: atualizar o startDateTime, endDateTime e assunto</span><span class="sxs-lookup"><span data-stu-id="5b63d-166">Example 1: Update the startDateTime, endDateTime and subject</span></span>

#### <a name="request"></a><span data-ttu-id="5b63d-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b63d-167">Request</span></span>

> <span data-ttu-id="5b63d-168">**Observação:** A ID da reunião foi truncada para capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="5b63d-168">**Note:** The meeting ID has been truncated for readability.</span></span>


# <a name="http"></a>[<span data-ttu-id="5b63d-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b63d-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_start_end_subject"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "startDateTime": "2020-09-09T14:33:30.8546353-07:00",
  "endDateTime": "2020-09-09T15:03:30.8566356-07:00",
  "subject": "Patch Meeting Subject"
}
```
# <a name="c"></a>[<span data-ttu-id="5b63d-170">C#</span><span class="sxs-lookup"><span data-stu-id="5b63d-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-start-end-subject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b63d-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b63d-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-start-end-subject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b63d-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b63d-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-start-end-subject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5b63d-173">Java</span><span class="sxs-lookup"><span data-stu-id="5b63d-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-start-end-subject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5b63d-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b63d-174">Response</span></span>

> <span data-ttu-id="5b63d-175">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5b63d-175">**Note:** The response object shown here might be shortened for readability.</span></span>

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

#### <a name="example-2-update-the-lobbybypasssettings"></a><span data-ttu-id="5b63d-176">Exemplo 2: atualizar o lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="5b63d-176">Example 2: Update the lobbyBypassSettings</span></span>
> <span data-ttu-id="5b63d-177">**Observação:** A ID da reunião foi truncada para capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="5b63d-177">**Note:** The meeting ID has been truncated for readability.</span></span>


# <a name="http"></a>[<span data-ttu-id="5b63d-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b63d-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_lobbyBypassSettings"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "lobbyBypassSettings": {
      "isDialInBypassEnabled": true
  }
}
```
# <a name="c"></a>[<span data-ttu-id="5b63d-179">C#</span><span class="sxs-lookup"><span data-stu-id="5b63d-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-lobbybypasssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b63d-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b63d-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-lobbybypasssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b63d-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b63d-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-lobbybypasssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5b63d-182">Java</span><span class="sxs-lookup"><span data-stu-id="5b63d-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-lobbybypasssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5b63d-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b63d-183">Response</span></span>

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


