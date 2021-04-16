---
title: Atualizar onlineMeeting
description: Atualize as propriedades de uma reunião online.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 42bc40f6dc1ec6f72996ade9b0a552bc94d0a69f
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51870006"
---
# <a name="update-onlinemeeting"></a><span data-ttu-id="5ee62-103">Atualizar onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="5ee62-103">Update onlineMeeting</span></span>

<span data-ttu-id="5ee62-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ee62-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ee62-105">Atualize as propriedades do objeto [onlineMeeting](../resources/onlinemeeting.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="5ee62-105">Update the properties of the specified [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

<span data-ttu-id="5ee62-106">Consulte [a seção Solicitar corpo](#request-body) para a lista de propriedades que suportam a atualização.</span><span class="sxs-lookup"><span data-stu-id="5ee62-106">Please see [Request body](#request-body) section for the list of properties that support updating.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ee62-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ee62-107">Permissions</span></span>

| <span data-ttu-id="5ee62-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ee62-108">Permission type</span></span>                        | <span data-ttu-id="5ee62-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ee62-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5ee62-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ee62-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ee62-111">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ee62-111">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="5ee62-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ee62-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ee62-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ee62-113">Not Supported.</span></span>                              |
| <span data-ttu-id="5ee62-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ee62-114">Application</span></span>                            | <span data-ttu-id="5ee62-115">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="5ee62-115">OnlineMeetings.ReadWrite.All\*</span></span>               |

> [!IMPORTANT]
> <span data-ttu-id="5ee62-116">\*Os administradores [](/graph/cloud-communication-online-meeting-application-access-policy) devem criar uma política de acesso a aplicativos e concedi-la a um usuário, autorizando o aplicativo configurado na política para atualizar uma reunião online em nome desse usuário (ID do usuário especificada no caminho da solicitação).</span><span class="sxs-lookup"><span data-stu-id="5ee62-116">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to update an online meeting on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="5ee62-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee62-117">HTTP request</span></span>
<span data-ttu-id="5ee62-118">Para atualizar o onlineMeeting especificado por meio da ID de reunião com o token delegado:</span><span class="sxs-lookup"><span data-stu-id="5ee62-118">To update the specified onlineMeeting by meeting ID with delegated token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onlineMeetings/{meetingId}
```

<span data-ttu-id="5ee62-119">Para atualizar o onlineMeeting especificado pela ID de reunião com o token de aplicativo:</span><span class="sxs-lookup"><span data-stu-id="5ee62-119">To update the specified onlineMeeting by meeting ID with application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{userId}/onlineMeetings/{meetingId}
```

> [!NOTE]
> - <span data-ttu-id="5ee62-120">`userId`é a ID do objeto de um usuário no portal de gerenciamento [de usuários do Azure.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="5ee62-120">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="5ee62-121">Para obter mais detalhes, consulte [política de acesso ao aplicativo](/graph/cloud-communication-online-meeting-application-access-policy).</span><span class="sxs-lookup"><span data-stu-id="5ee62-121">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
> - <span data-ttu-id="5ee62-122">`meetingId`é a **id** de um [objeto onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="5ee62-122">`meetingId` is the **id** of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ee62-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee62-123">Request headers</span></span>
| <span data-ttu-id="5ee62-124">Nome</span><span class="sxs-lookup"><span data-stu-id="5ee62-124">Name</span></span>          | <span data-ttu-id="5ee62-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ee62-125">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="5ee62-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ee62-126">Authorization</span></span> | <span data-ttu-id="5ee62-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ee62-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="5ee62-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="5ee62-129">Content-type</span></span>  | <span data-ttu-id="5ee62-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ee62-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ee62-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee62-132">Request body</span></span>
<span data-ttu-id="5ee62-133">A tabela abaixo lista as propriedades que podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="5ee62-133">The table below lists the properties that can be updated.</span></span> <span data-ttu-id="5ee62-134">No corpo da solicitação, inclua apenas as propriedades que precisam ser atualizadas, com as seguintes exceções:</span><span class="sxs-lookup"><span data-stu-id="5ee62-134">In the request body, include only the properties that need updating, with the following exceptions:</span></span>

- <span data-ttu-id="5ee62-135">Ajustar a data/hora inicial ou final de uma reunião online sempre requer as propriedades **startDateTime** e **endDateTime** no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ee62-135">Adjusting the start or end date/time of an online meeting always requires both **startDateTime** and **endDateTime** properties in the request body.</span></span>
- <span data-ttu-id="5ee62-136">Ajustar o **campo de** participantes  da propriedade participantes, como adicionar ou remover um participante à reunião, sempre requer a lista completa de participantes no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ee62-136">Adjusting the **attendees** field of the **participants** property, such as adding or removing an attendee to the meeting, always requires the full list of attendees in the request body.</span></span>

| <span data-ttu-id="5ee62-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ee62-137">Property</span></span>             | <span data-ttu-id="5ee62-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ee62-138">Type</span></span>                                                         | <span data-ttu-id="5ee62-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ee62-139">Description</span></span>                                                                                                                                    |
|----------------------|--------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5ee62-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5ee62-140">startDateTime</span></span>        | <span data-ttu-id="5ee62-141">DateTime</span><span class="sxs-lookup"><span data-stu-id="5ee62-141">DateTime</span></span>                                                     | <span data-ttu-id="5ee62-142">O horário de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="5ee62-142">The meeting start time in UTC.</span></span>                                                                                                                 |
| <span data-ttu-id="5ee62-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="5ee62-143">endDateTime</span></span>          | <span data-ttu-id="5ee62-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="5ee62-144">DateTime</span></span>                                                     | <span data-ttu-id="5ee62-145">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="5ee62-145">The meeting end time in UTC.</span></span>                                                                                                                   |
| <span data-ttu-id="5ee62-146">assunto</span><span class="sxs-lookup"><span data-stu-id="5ee62-146">subject</span></span>              | <span data-ttu-id="5ee62-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ee62-147">String</span></span>                                                       | <span data-ttu-id="5ee62-148">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="5ee62-148">The subject of the online meeting.</span></span>                                                                                                             |
| <span data-ttu-id="5ee62-149">participants</span><span class="sxs-lookup"><span data-stu-id="5ee62-149">participants</span></span>         | [<span data-ttu-id="5ee62-150">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="5ee62-150">meetingParticipants</span></span>](../resources/meetingparticipants.md)   | <span data-ttu-id="5ee62-151">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="5ee62-151">The participants associated with the online meeting.</span></span> <span data-ttu-id="5ee62-152">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="5ee62-152">This includes the organizer and the attendees.</span></span>                                            |
| <span data-ttu-id="5ee62-153">isEntryExitAnnounced</span><span class="sxs-lookup"><span data-stu-id="5ee62-153">isEntryExitAnnounced</span></span> | <span data-ttu-id="5ee62-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ee62-154">Boolean</span></span>                                                      | <span data-ttu-id="5ee62-155">Se os chamadores ingressarão ou sairão.</span><span class="sxs-lookup"><span data-stu-id="5ee62-155">Whether or not to announce when callers join or leave.</span></span>                                                                                         |
| <span data-ttu-id="5ee62-156">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="5ee62-156">lobbyBypassSettings</span></span>  | [<span data-ttu-id="5ee62-157">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="5ee62-157">lobbyBypassSettings</span></span>](../resources/lobbyBypassSettings.md)   | <span data-ttu-id="5ee62-158">Especifica quais participantes podem ignorar o lobby da reunião.</span><span class="sxs-lookup"><span data-stu-id="5ee62-158">Specifies which participants can bypass the meeting lobby.</span></span>                                                                                     |
| <span data-ttu-id="5ee62-159">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="5ee62-159">allowedPresenters</span></span>    | <span data-ttu-id="5ee62-160">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="5ee62-160">onlineMeetingPresenters</span></span>                                      | <span data-ttu-id="5ee62-161">Especifica quem pode ser um apresentador em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="5ee62-161">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="5ee62-162">Os valores possíveis são todos, organização, roleIsPresenter, organizador e unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="5ee62-162">Possible values are everyone, organization, roleIsPresenter, organizer, and unknownFutureValue.</span></span> |

## <a name="response"></a><span data-ttu-id="5ee62-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee62-163">Response</span></span>
<span data-ttu-id="5ee62-164">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee62-164">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5ee62-165">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5ee62-165">Examples</span></span>

### <a name="example-1-update-the-startdatetime-enddatetime-and-subject"></a><span data-ttu-id="5ee62-166">Exemplo 1: atualizar o startDateTime, endDateTime e assunto</span><span class="sxs-lookup"><span data-stu-id="5ee62-166">Example 1: Update the startDateTime, endDateTime and subject</span></span>

#### <a name="request"></a><span data-ttu-id="5ee62-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee62-167">Request</span></span>

> <span data-ttu-id="5ee62-168">**Observação:** A ID da reunião foi truncada para capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="5ee62-168">**Note:** The meeting ID has been truncated for readability.</span></span>


# <a name="http"></a>[<span data-ttu-id="5ee62-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee62-169">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5ee62-170">C#</span><span class="sxs-lookup"><span data-stu-id="5ee62-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-start-end-subject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ee62-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ee62-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-start-end-subject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ee62-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ee62-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-start-end-subject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ee62-173">Java</span><span class="sxs-lookup"><span data-stu-id="5ee62-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-start-end-subject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5ee62-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee62-174">Response</span></span>

> <span data-ttu-id="5ee62-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ee62-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

#### <a name="example-2-update-the-lobbybypasssettings"></a><span data-ttu-id="5ee62-177">Exemplo 2: atualizar o lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="5ee62-177">Example 2: Update the lobbyBypassSettings</span></span>
> <span data-ttu-id="5ee62-178">**Observação:** A ID da reunião foi truncada para capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="5ee62-178">**Note:** The meeting ID has been truncated for readability.</span></span>


# <a name="http"></a>[<span data-ttu-id="5ee62-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee62-179">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5ee62-180">C#</span><span class="sxs-lookup"><span data-stu-id="5ee62-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-lobbybypasssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ee62-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ee62-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-lobbybypasssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ee62-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ee62-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-lobbybypasssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ee62-183">Java</span><span class="sxs-lookup"><span data-stu-id="5ee62-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-lobbybypasssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5ee62-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee62-184">Response</span></span>

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


