---
title: Obter onlineMeeting
description: Recupere as propriedades e as relações de um objeto onlineMeeting.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: f930a0c60b228942781086b4ecae0a17b0e20b91
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516014"
---
# <a name="get-onlinemeeting"></a><span data-ttu-id="136a3-103">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="136a3-103">Get onlineMeeting</span></span>

<span data-ttu-id="136a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="136a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="136a3-105">Recupere as propriedades e as relações de um [objeto onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="136a3-105">Retrieve the properties and relationships of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

<span data-ttu-id="136a3-106">Por exemplo, você pode:</span><span class="sxs-lookup"><span data-stu-id="136a3-106">For example, you can:</span></span>
- <span data-ttu-id="136a3-107">Obter detalhes de um onlineMeeting usando [VideoTeleconferenceId](#example-1-retrieve-an-online-meeting-by-videoteleconferenceid), [ID](#example-2-retrieve-an-online-meeting-by-meeting-id)da reunião ou [JoinWebURL](#example-3-retrieve-an-online-meeting-by-joinweburl).</span><span class="sxs-lookup"><span data-stu-id="136a3-107">Get details of an onlineMeeting using [VideoTeleconferenceId](#example-1-retrieve-an-online-meeting-by-videoteleconferenceid), [meeting ID](#example-2-retrieve-an-online-meeting-by-meeting-id), or [JoinWebURL](#example-3-retrieve-an-online-meeting-by-joinweburl).</span></span>
- <span data-ttu-id="136a3-108">Use o caminho para obter um relatório do participante `/attendeeReport` de um evento ao vivo, conforme mostrado no exemplo [4](#example-4-retrieve-the-attendee-report-of-a-live-event).</span><span class="sxs-lookup"><span data-stu-id="136a3-108">Use the `/attendeeReport` path to get an attendee report of a live event, as shown in [example 4](#example-4-retrieve-the-attendee-report-of-a-live-event).</span></span>
- <span data-ttu-id="136a3-109">Use os caminhos e para obter as gravações de um `/recording` `/alternativeRecording` evento ao vivo, conforme mostrado no exemplo [5](#example-5-retrieve-the-recording-of-a-live-event).</span><span class="sxs-lookup"><span data-stu-id="136a3-109">Use the `/recording` and `/alternativeRecording` paths to get the recordings of a live event, as shown in [example 5](#example-5-retrieve-the-recording-of-a-live-event).</span></span>

><span data-ttu-id="136a3-110">**Observações:**</span><span class="sxs-lookup"><span data-stu-id="136a3-110">**Notes:**</span></span> 
>- <span data-ttu-id="136a3-111">Atualmente, os relatórios e gravações do participante estão disponíveis apenas para eventos ao vivo.</span><span class="sxs-lookup"><span data-stu-id="136a3-111">Currently, attendee reports and recordings are available only to live events.</span></span>
>- <span data-ttu-id="136a3-112">Somente o organizador do evento pode acessar relatórios e gravações do participante.</span><span class="sxs-lookup"><span data-stu-id="136a3-112">Only the event organizer can access attendee reports and recordings.</span></span>
>- <span data-ttu-id="136a3-113">Os relatórios e gravações do participante só estarão disponíveis quando o evento ao vivo for concluído.</span><span class="sxs-lookup"><span data-stu-id="136a3-113">Attendee reports and recordings are only available when the live event has concluded.</span></span>
>- <span data-ttu-id="136a3-114">O link de download na `302 Found` [resposta](#example-4-retrieve-the-attendee-report-of-a-live-event) expira em **60** segundos.</span><span class="sxs-lookup"><span data-stu-id="136a3-114">The download link in the `302 Found` [response](#example-4-retrieve-the-attendee-report-of-a-live-event) expires in **60** seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="136a3-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="136a3-115">Permissions</span></span>

<span data-ttu-id="136a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="136a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="136a3-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="136a3-118">Permission type</span></span>                        | <span data-ttu-id="136a3-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="136a3-119">Permissions (from least to most privileged)</span></span>           |
| :------------------------------------- | :---------------------------------------------------- |
| <span data-ttu-id="136a3-120">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="136a3-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="136a3-121">OnlineMeetings.Read, OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="136a3-121">OnlineMeetings.Read, OnlineMeetings.ReadWrite</span></span>         |
| <span data-ttu-id="136a3-122">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="136a3-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="136a3-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="136a3-123">Not Supported.</span></span>                                        |
| <span data-ttu-id="136a3-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="136a3-124">Application</span></span>                            | <span data-ttu-id="136a3-125">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="136a3-125">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All\*</span></span> |

> [!IMPORTANT]
> <span data-ttu-id="136a3-126">\*Os administradores [](/graph/cloud-communication-online-meeting-application-access-policy) devem criar uma política de acesso a aplicativos e concedi-la a um usuário, autorizando o aplicativo configurado na política para recuperar uma reunião online em nome desse usuário (ID do usuário especificada no caminho da solicitação).</span><span class="sxs-lookup"><span data-stu-id="136a3-126">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to retrieve an online meeting on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="136a3-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="136a3-127">HTTP request</span></span>

<span data-ttu-id="136a3-128">Para obter a onlineMeeting especificada usando a ID da reunião com permissão delegada:</span><span class="sxs-lookup"><span data-stu-id="136a3-128">To get the specified onlineMeeting using meeting ID with delegated permission:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{meetingId}
```

<span data-ttu-id="136a3-129">Para obter o onlineMeeting especificado usando a ID da reunião com permissão de aplicativo:</span><span class="sxs-lookup"><span data-stu-id="136a3-129">To get the specified onlineMeeting using meeting ID with application permission:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{userId}/onlineMeetings/{meetingId}
```

<span data-ttu-id="136a3-130">Para obter o onlineMeeting especificado usando **videoTeleconferenceId**:</span><span class="sxs-lookup"><span data-stu-id="136a3-130">To get the specified onlineMeeting using **videoTeleconferenceId**:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{videoTeleconferenceId}'
GET /communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{videoTeleconferenceId}'
```

<span data-ttu-id="136a3-131">Para obter o onlineMeeting especificado usando **joinWebUrl**:</span><span class="sxs-lookup"><span data-stu-id="136a3-131">To get the specified onlineMeeting using **joinWebUrl**:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{userId}/onlineMeetings?$filter=JoinWebUrl%20eq%20'{joinWebUrl}'
```

<span data-ttu-id="136a3-132">Para obter o relatório do participante de um evento ao vivo:</span><span class="sxs-lookup"><span data-stu-id="136a3-132">To get the attendee report of a live event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{userId}/onlineMeetings/{meetingId}/attendeeReport
```

<span data-ttu-id="136a3-133">Para obter as gravações de um evento ao vivo:</span><span class="sxs-lookup"><span data-stu-id="136a3-133">To get the recordings of a live event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{userId}/onlineMeetings/{meetingId}/recording
GET /users/{userId}/onlineMeetings/{meetingId}/alternativeRecording
```

><span data-ttu-id="136a3-134">**Observações:**</span><span class="sxs-lookup"><span data-stu-id="136a3-134">**Notes:**</span></span>
>- <span data-ttu-id="136a3-135">O caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="136a3-135">The `/app` path is deprecated.</span></span> <span data-ttu-id="136a3-136">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="136a3-136">Going forward, use the `/communications` path.</span></span>
>- <span data-ttu-id="136a3-137">`userId`é a ID do objeto de um usuário no portal de gerenciamento [de usuários do Azure.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="136a3-137">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="136a3-138">Para obter mais detalhes, consulte [política de acesso ao aplicativo](/graph/cloud-communication-online-meeting-application-access-policy).</span><span class="sxs-lookup"><span data-stu-id="136a3-138">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
>- <span data-ttu-id="136a3-139">`meetingId`é a **id** de um [objeto onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="136a3-139">`meetingId` is the **id** of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>
> - <span data-ttu-id="136a3-140">**videoTeleconferenceId** é gerado para usuários licenciados do Cloud-Video-Interop e pode ser encontrado em um [objeto onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="136a3-140">**videoTeleconferenceId** is generated for Cloud-Video-Interop licensed users and can be found in an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span> <span data-ttu-id="136a3-141">Consulte a [ID da conferência VTC](/microsoftteams/cloud-video-interop-for-teams-set-up) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="136a3-141">Refer to [VTC conference id](/microsoftteams/cloud-video-interop-for-teams-set-up) for more details.</span></span>
>- <span data-ttu-id="136a3-142">`joinWebUrl` deve ser codificada por URL e essa rota só pode ser usada para recuperar reuniões criadas por `userId` .</span><span class="sxs-lookup"><span data-stu-id="136a3-142">`joinWebUrl` must be URL encoded and this route can only be used to retrieve meetings created by `userId`.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="136a3-143">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="136a3-143">Optional query parameters</span></span>
<span data-ttu-id="136a3-144">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="136a3-144">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="136a3-145">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="136a3-145">Request headers</span></span>
| <span data-ttu-id="136a3-146">Nome</span><span class="sxs-lookup"><span data-stu-id="136a3-146">Name</span></span>            | <span data-ttu-id="136a3-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="136a3-147">Description</span></span>               |
| :-------------- | :------------------------ |
| <span data-ttu-id="136a3-148">Autorização</span><span class="sxs-lookup"><span data-stu-id="136a3-148">Authorization</span></span>   | <span data-ttu-id="136a3-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="136a3-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="136a3-151">Accept-Language</span><span class="sxs-lookup"><span data-stu-id="136a3-151">Accept-Language</span></span> | <span data-ttu-id="136a3-152">Idioma.</span><span class="sxs-lookup"><span data-stu-id="136a3-152">Language.</span></span> <span data-ttu-id="136a3-153">Opcional.</span><span class="sxs-lookup"><span data-stu-id="136a3-153">Optional.</span></span>       |

<span data-ttu-id="136a3-154">Se a solicitação contiver um `Accept-Language`cabeçalho HTTP, o `content` de `joinInformation` estará na variante de idioma e código de idioma especificada `Accept-Language` no cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="136a3-154">If the request contains an `Accept-Language` HTTP header, the `content` of `joinInformation` will be in the language and locale variant specified in the `Accept-Language` header.</span></span> <span data-ttu-id="136a3-155">O conteúdo padrão será em inglês.</span><span class="sxs-lookup"><span data-stu-id="136a3-155">The default content will be in English.</span></span>

## <a name="request-body"></a><span data-ttu-id="136a3-156">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="136a3-156">Request body</span></span>
<span data-ttu-id="136a3-157">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="136a3-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="136a3-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="136a3-158">Response</span></span>
<span data-ttu-id="136a3-159">Se bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="136a3-159">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="136a3-160">O método também inclui um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="136a3-160">The method also includes one of the following:</span></span>

- <span data-ttu-id="136a3-161">Se você estiver recebendo uma reunião online com base na ID da reunião, **videoTeleconferenceId** ou **joinWebUrl,** este método também retornará um [objeto onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="136a3-161">If you're getting an online meeting based on meeting ID, **videoTeleconferenceId** or **joinWebUrl**, this method also returns an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>
- <span data-ttu-id="136a3-162">Se você estiver recebendo o relatório do participante ou a gravação de uma reunião online ao vivo, este método também retorna um header que indica o URI para o relatório ou gravação do `Location` participante, respectivamente.</span><span class="sxs-lookup"><span data-stu-id="136a3-162">If you're getting the attendee report or recording of a live online meeting, this method also returns a `Location` header that indicates the URI to the attendee report or recording, respectively.</span></span>

## <a name="examples"></a><span data-ttu-id="136a3-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="136a3-163">Examples</span></span>

### <a name="example-1-retrieve-an-online-meeting-by-videoteleconferenceid"></a><span data-ttu-id="136a3-164">Exemplo 1: Recuperar uma reunião online por VideoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="136a3-164">Example 1: Retrieve an online meeting by VideoTeleconferenceId</span></span>

#### <a name="request"></a><span data-ttu-id="136a3-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="136a3-165">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="136a3-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="136a3-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["123456789"],
  "name": "get-onlineMeeting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'123456789'
```
# <a name="c"></a>[<span data-ttu-id="136a3-167">C#</span><span class="sxs-lookup"><span data-stu-id="136a3-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="136a3-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="136a3-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="136a3-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="136a3-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="136a3-170">Java</span><span class="sxs-lookup"><span data-stu-id="136a3-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onlinemeeting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="136a3-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="136a3-171">Response</span></span>

> <span data-ttu-id="136a3-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="136a3-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "autoAdmittedUsers": "everyone",
  "audioConferencing": {
    "tollNumber": "55525634478",
    "tollFreeNumber": "55566390588",
    "ConferenceId": "9999999",
    "dialinUrl": "https://dialin.teams.microsoft.com/6787A136-B9B8-4D39-846C-C0F1FF937F10?id=xxxxxxx"
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
    "messageId": "1533758867081"
  },
  "creationDateTime": "2018-05-30T00:12:19.0726086Z",
  "endDateTime": "2018-05-30T01:00:00Z",
  "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8_19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3a:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context=%7b%22Tid%22%3a%aa67bd4c-8475-432d-bd41-39f255720e0a%22%2c%22Oid%22%3a%22112f7296-5fa4-42ca-bae8-6a692b15d4b8%22%7d",
  "participants": {
    "attendees": [
      {
        "@odata.type": "#microsoft.graph.identitySet",
        "identity": {
          "user": {
            "@odata.type": "#microsoft.graph.identity",
            "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8",
            "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
            "displayName": "Tyler Stein"
          }
        },
        "upn": "upn-value",
        "role": "attendee"
      }
    ],
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "identity": {
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
          "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
          "displayName": "Jasmine Miller"
        }
      },
      "upn": "upn-value",
      "role": "presenter"
    }
  },
  "startDateTime": "2018-05-30T00:30:00Z",
  "subject": "Test Meeting.",
  "videoTeleconferenceId": "123456789",
  "lobbyBypassSettings": {
    "scope": "everyone",
    "isDialInBypassEnabled": true
  },
  "isEntryExitAnnounced": true,
  "allowedPresenters": "everyone"
}
```
><span data-ttu-id="136a3-174">**Observação:** Se 'Accept-Language: ja' for especificado para indicar japonês, por exemplo, a resposta incluirá o seguinte.</span><span class="sxs-lookup"><span data-stu-id="136a3-174">**Note:** If 'Accept-Language: ja' is specified to indicate Japanese, for example, the response will include the following.</span></span>

```json
    "joinInformation": {
        "content": "data%3Atext%2Fhtml%2C%0A++%3Cdiv+style%3D%22width%3A100%25%3Bheight%3A+20px%3B%22%3E%0A%09%09%3Cspan+style%3D%22white-space%3Anowrap%3Bcolor%3Agray%3Bopacity%3A.36%3B%22%3E________________________________________________________________________________%3C%2Fspan%3E%0A%09+%3C%2Fdiv%3E%0A++++%3Cdiv+class%3D%22me-email-text%22+style%3D%22color%3A%23252424%3Bfont-family%3A'Segoe+UI'%2C'Helvetica+Neue'%2CHelvetica%2CArial%2Csans-serif%3B%22%3E%0A+++%3Cdiv+style%3D%22margin-top%3A+24px%3B+margin-bottom%3A+10px%3B%22%3E%0A++++++++%3Ca+class%3D%22me-email-headline%22%0A++++++++++++++style%3D%22font-size%3A+18px%3Bfont-family%3A'Segoe+UI+Semibold'%2C'Segoe+UI'%2C'Helvetica+Neue'%2CHelvetica%2CArial%2Csans-serif%3Btext-decoration%3A+underline%3Bcolor%3A+%236264a7%3B%22%0A++++++++++++++href%3D%22https%3A%2F%2Fteams.microsoft.com%2Fl%2Fmeetup-join%2F19%253ameeting_NDRiZjRiMmUtODI5OC00MzRlLTk1ZWEtMGY1000000000000%2540thread.v2%2F0%3Fcontext%3D%257b%2522Tid%2522%253a%252279a788bf-86f1-41af-91ab-000000000000%2522%252c%2522Oid%2522%253a%2522d4a060b5-a8fc-450c-837b-000000000000%2522%257d%22%0A++++++++++++++target%3D%22_blank%22+rel%3D%22noreferrer+noopener%22%3EMicrosoft+Teams+%E4%BC%9A%E8%AD%B0%E3%81%AB%E5%8F%82%E5%8A%A0%3C%2Fa%3E%0A++++++%3C%2Fdiv%3E%0A%09+%3Cdiv%3E%0A++++%0A++++++%3Cdiv%3E%0A++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+14px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22%0A++++++++++href%3D%22tel%3A%2B16477490000%2C%2C11160000%26%2335%3B+%22+target%3D%22_blank%22+rel%3D%22noreferrer+noopener%22%3E%2B16477490000%3C%2Fa%3E%0A++++++%3Cspan+style%3D%22font-size%3A+12px%3B%22%3E%26nbsp%3B++(%E6%9C%89%E6%96%99)+%3C%2Fspan%3E%0A++++++%3C%2Fdiv%3E%0A++++%0A++%3C%2Fdiv%3E%0A%0A%09+%0A++++++%3Cdiv+style%3D%22margin-top%3A+10px%3B+margin-bottom%3A+20px%3B%22%3E%0A++++++++%3Cspan+style%3D%22font-size%3A+12px%3B%22%3E%0A++++++++++%E4%BC%9A%E8%AD%B0+ID%3A%0A++++++++%3C%2Fspan%3E%0A++++++%3Cspan+style%3D%22font-size%3A+14px%3B%22%3E%0A++++++++111+000+00%23%0A++++++%3C%2Fspan%3E%0A++++%3C%2Fdiv%3E%0A++++%0A%09+%0A++++++++%3Cdiv+style%3D%22margin-bottom%3A+24px%3B%22%3E%0A++++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fdialin.teams.microsoft.com%2F8bf6e654-57eb-4b85-aeaf-36c84429b2fe%3Fid%3D11160000%22+rel%3D%22noreferrer+noopener%22%3E%E6%9C%80%E5%AF%84%E3%82%8A%E3%81%AE%E5%9B%BD%E3%81%AE%E9%9B%BB%E8%A9%B1%E7%95%AA%E5%8F%B7%E3%82%92%E6%A4%9C%E7%B4%A2%3C%2Fa%3E%0A+++++++++%7C%0A++++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fmysettings.lync.com%2Fpstnconferencing%22+rel%3D%22noreferrer+noopener%22%3E%0A++++++++PIN+%E3%82%92%E3%83%AA%E3%82%BB%E3%83%83%E3%83%88%3C%2Fa%3E%0A+++++++++%7C+%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Faka.ms%2FJoinTeamsMeeting%22+rel%3D%22noreferrer+noopener%22%3ETeams+%E3%81%AE%E8%A9%B3%E7%B4%B0%E3%82%92%E8%A1%A8%E7%A4%BA%3C%2Fa%3E%0A+++++%7C+%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fteams.microsoft.com%2FmeetingOptions%2F%3ForganizerId%3Dd4a060b5-a8fc-450c-837b-000000000000%26tenantId%3D79a788bf-86f1-41af-91ab-000000000000%26threadId%3D19_meeting_NDRiZjRiMmUtODI5OC00MzRlLTk1ZWEtMGY1000000000000%40thread.v2%26messageId%3D0%26language%3Dja%22+rel%3D%22noreferrer+noopener%22%3E%E4%BC%9A%E8%AD%B0%E3%81%AE%E3%82%AA%E3%83%97%E3%82%B7%E3%83%A7%E3%83%B3%3C%2Fa%3E%0A++++%0A++++++++%3C%2Fdiv%3E%0A++++%0A+++++%0A++++++++%3Cdiv+style%3D%22font-size%3A+14px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++++++%E3%83%93%E3%83%87%E3%82%AA%E4%BC%9A%E8%AD%B0%E3%83%87%E3%83%90%E3%82%A4%E3%82%B9%E3%81%A7%E5%8F%82%E5%8A%A0%0A++++++++%3C%2Fdiv%3E%0A%0A++++++++%3Cdiv+style%3D%22font-size%3A12px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22text-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+href%3D%22%22%3E000000000%40t.abcd.vc%3C%2Fa%3E+VTC+%E4%BC%9A%E8%AD%B0+ID%3A+0180300000%0A++++++++%3C%2Fdiv%3E%0A%0A++++++++%3Cdiv+style%3D%22font-size%3A+12px%3B+margin-bottom%3A+20px%3B%22%3E%0A++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22text-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+href%3D%22https%3A%2F%2Fdialin.abcd.vc%2Fteams%2F%3Fkey%3D000000000%26conf%3D0180308922%22%3E%E4%BB%A3%E6%9B%BF+VTC+%E3%81%AE%E3%83%80%E3%82%A4%E3%83%A4%E3%83%AB%E6%96%B9%E6%B3%95%3C%2Fa%3E%0A++++++++%3C%2Fdiv%3E%0A++++%0A+++++%0A++++++%3Cdiv+style%3D%22font-size%3A+14px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++%0A++++++%3C%2Fdiv%3E%0A++++++%3Cdiv+style%3D%22font-size%3A+12px%3B%22%3E%0A++++++%0A++++++%3C%2Fdiv%3E%0A++++%0A+++++%3C%2Fdiv%3E%0A%09+%3Cdiv+style%3D%22width%3A100%25%3Bheight%3A+20px%3B%22%3E%0A%09%09%3Cspan+style%3D%22white-space%3Anowrap%3Bcolor%3Agray%3Bopacity%3A.36%3B%22%3E________________________________________________________________________________%3C%2Fspan%3E%0A++%3C%2Fdiv%3E%22%2C%0A",
        "contentType": "Html"
    }  
```

### <a name="example-2-retrieve-an-online-meeting-by-meeting-id"></a><span data-ttu-id="136a3-175">Exemplo 2: Recuperar uma reunião online por ID de reunião</span><span class="sxs-lookup"><span data-stu-id="136a3-175">Example 2: Retrieve an online meeting by meeting ID</span></span>
<span data-ttu-id="136a3-176">Você pode recuperar informações de reunião por meio da ID de reunião com um token de usuário ou aplicativo.</span><span class="sxs-lookup"><span data-stu-id="136a3-176">You can retrieve meeting information via meeting ID with either a user or application token.</span></span> <span data-ttu-id="136a3-177">A ID da reunião é fornecida no objeto de resposta ao criar [um onlineMeeting](../resources/onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="136a3-177">The meeting ID is provided in the response object when creating an [onlineMeeting](../resources/onlinemeeting.md).</span></span> <span data-ttu-id="136a3-178">Essa opção está disponível para dar suporte a casos de uso em que a ID da reunião é conhecida, como quando um aplicativo cria primeiro a reunião online usando a API graph primeiro e recupera informações de reunião posteriormente como uma ação separada.</span><span class="sxs-lookup"><span data-stu-id="136a3-178">This option is available to support use cases where the meeting ID is known, such as when an application first creates the online meeting using Graph API first then retrieves meeting information later as a separate action.</span></span>

#### <a name="request"></a><span data-ttu-id="136a3-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="136a3-179">Request</span></span>

> <span data-ttu-id="136a3-180">**Observação:** A ID da reunião foi truncada para capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="136a3-180">**Note:** The meeting ID has been truncated for readability.</span></span>

<span data-ttu-id="136a3-181">A solicitação a seguir usa um token de usuário.</span><span class="sxs-lookup"><span data-stu-id="136a3-181">The following request uses a user token.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy
```

<span data-ttu-id="136a3-182">A solicitação a seguir usa um token de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="136a3-182">The following request uses an app token.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/dc17674c-81d9-4adb-bfb2-8f6a442e4622/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy
```

#### <a name="response"></a><span data-ttu-id="136a3-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="136a3-183">Response</span></span>

> <span data-ttu-id="136a3-184">**Observação:** O objeto de resposta mostrado aqui foi reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="136a3-184">**Note:** The response object shown here has been shortened for readability.</span></span> <span data-ttu-id="136a3-185">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="136a3-185">All the properties will be returned from an actual call.</span></span>

```json
{
    "id": "MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy",
    "creationDateTime": "2020-09-29T22:35:33.1594516Z",
    "startDateTime": "2020-09-29T22:35:31.389759Z",
    "endDateTime": "2020-09-29T23:35:31.389759Z",
    "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2%40thread.v2/0?context=%7b%22Tid%22%3a%22909c6581-5130-43e9-88f3-fcb3582cde37%22%2c%22Oid%22%3a%22dc17674c-81d9-4adb-bfb2-8f6a442e4622%22%7d",
    "subject": null,
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
        "producers": [],
        "contributors": []
    },
    "lobbyBypassSettings": {
        "scope": "organization",
        "isDialInBypassEnabled": false
    }
}
```

### <a name="example-3-retrieve-an-online-meeting-by-joinweburl"></a><span data-ttu-id="136a3-186">Exemplo 3: Recuperar uma reunião online por JoinWebUrl</span><span class="sxs-lookup"><span data-stu-id="136a3-186">Example 3: Retrieve an online meeting by JoinWebUrl</span></span>
<span data-ttu-id="136a3-187">Você pode recuperar informações de reunião por meio do JoinWebUrl usando um token de usuário ou aplicativo.</span><span class="sxs-lookup"><span data-stu-id="136a3-187">You can retrieve meeting information via JoinWebUrl by using either a user or application token.</span></span> <span data-ttu-id="136a3-188">Essa opção está disponível para dar suporte a casos de uso em que a ID da reunião não é conhecida, mas o JoinWebUrl é, como quando um usuário cria uma reunião (por exemplo, no cliente do Microsoft Teams) e um aplicativo separado precisa recuperar os detalhes da reunião como uma ação de acompanhamento.</span><span class="sxs-lookup"><span data-stu-id="136a3-188">This option is available to support use cases where the meeting ID is not known but the JoinWebUrl is, such as when a user creates a meeting (for example in the Microsoft Teams client), and a seperate application needs to retrieve meeting details as a followup action.</span></span>

#### <a name="request"></a><span data-ttu-id="136a3-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="136a3-189">Request</span></span>

<span data-ttu-id="136a3-190">A solicitação a seguir usa um token de usuário.</span><span class="sxs-lookup"><span data-stu-id="136a3-190">The following request uses a user token.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onlineMeetings?$filter=JoinWebUrl%20eq%20'https%3A%2F%2Fteams.microsoft.com%2Fl%2Fmeetup-join%2F19%253ameeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2%2540thread.v2%2F0%3Fcontext%3D%257b%2522Tid%2522%253a%2522909c6581-5130-43e9-88f3-fcb3582cde37%2522%252c%2522Oid%2522%253a%2522dc17674c-81d9-4adb-bfb2-8f6a442e4622%2522%257d'
```

<span data-ttu-id="136a3-191">A solicitação a seguir usa um token de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="136a3-191">The following request uses an app token.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/dc17674c-81d9-4adb-bfb2-8f6a442e4622/onlineMeetings?$filter=JoinWebUrl%20eq%20'https%3A%2F%2Fteams.microsoft.com%2Fl%2Fmeetup-join%2F19%253ameeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2%2540thread.v2%2F0%3Fcontext%3D%257b%2522Tid%2522%253a%2522909c6581-5130-43e9-88f3-fcb3582cde37%2522%252c%2522Oid%2522%253a%2522dc17674c-81d9-4adb-bfb2-8f6a442e4622%2522%257d'
```

#### <a name="response"></a><span data-ttu-id="136a3-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="136a3-192">Response</span></span>

> <span data-ttu-id="136a3-193">**Observação:** O objeto de resposta mostrado aqui foi reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="136a3-193">**Note:** The response object shown here has been shortened for readability.</span></span> <span data-ttu-id="136a3-194">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="136a3-194">All the properties will be returned from an actual call.</span></span>

```json
{
    "value": [
        {
            "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2@thread.v2",
            "creationDateTime": "2020-09-29T22:35:33.1594516Z",
            "startDateTime": "2020-09-29T22:35:31.389759Z",
            "endDateTime": "2020-09-29T23:35:31.389759Z",
            "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2%40thread.v2/0?context=%7b%22Tid%22%3a%22909c6581-5130-43e9-88f3-fcb3582cde37%22%2c%22Oid%22%3a%22dc17674c-81d9-4adb-bfb2-8f6a442e4622%22%7d",
            "subject": null,
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
                "producers": [],
                "contributors": []
            },
            "lobbyBypassSettings": {
                "scope": "organization",
                "isDialInBypassEnabled": false
            }
        }
    ]
}
```

### <a name="example-4-retrieve-the-attendee-report-of-a-live-event"></a><span data-ttu-id="136a3-195">Exemplo 4: Recuperar o relatório do participante de um evento ao vivo</span><span class="sxs-lookup"><span data-stu-id="136a3-195">Example 4: Retrieve the attendee report of a live event</span></span>
<span data-ttu-id="136a3-196">O exemplo a seguir mostra uma solicitação para baixar um relatório do participante.</span><span class="sxs-lookup"><span data-stu-id="136a3-196">The following example shows a request to download an attendee report.</span></span>

#### <a name="request"></a><span data-ttu-id="136a3-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="136a3-197">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="136a3-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="136a3-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dc74d9bb-6afe-433d-8eaa-e39d80d3a647", "dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw@thread.v2"],
  "name": "get-attendeeReport"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/dc74d9bb-6afe-433d-8eaa-e39d80d3a647/onlineMeetings/dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw@thread.v2/attendeeReport
```
# <a name="c"></a>[<span data-ttu-id="136a3-199">C#</span><span class="sxs-lookup"><span data-stu-id="136a3-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-attendeereport-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="136a3-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="136a3-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-attendeereport-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="136a3-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="136a3-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-attendeereport-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="136a3-202">Java</span><span class="sxs-lookup"><span data-stu-id="136a3-202">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-attendeereport-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="136a3-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="136a3-203">Response</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 302 Found
Location: https://01-a-noam.dog.attend.teams.microsoft.com/broadcast/909c6581-5130-43e9-88f3-fcb3582cde37/dc17674c-81d9-4adb-bfb2-8f6a442e4622/19%3Ameeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw%40thread.v2/0/resource/attendeeReport
```

### <a name="example-5-retrieve-the-recording-of-a-live-event"></a><span data-ttu-id="136a3-204">Exemplo 5: Recuperar a gravação de um evento ao vivo</span><span class="sxs-lookup"><span data-stu-id="136a3-204">Example 5: Retrieve the recording of a live event</span></span>
<span data-ttu-id="136a3-205">O exemplo a seguir mostra uma solicitação para baixar uma gravação.</span><span class="sxs-lookup"><span data-stu-id="136a3-205">The following example shows a request to download a recording.</span></span>

#### <a name="request"></a><span data-ttu-id="136a3-206">Solicitação</span><span class="sxs-lookup"><span data-stu-id="136a3-206">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="136a3-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="136a3-207">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dc74d9bb-6afe-433d-8eaa-e39d80d3a647", "dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw@thread.v2"],
  "name": "get-recording"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/dc74d9bb-6afe-433d-8eaa-e39d80d3a647/onlineMeetings/dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw@thread.v2/recording
```
# <a name="c"></a>[<span data-ttu-id="136a3-208">C#</span><span class="sxs-lookup"><span data-stu-id="136a3-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-recording-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="136a3-209">JavaScript</span><span class="sxs-lookup"><span data-stu-id="136a3-209">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-recording-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="136a3-210">Objective-C</span><span class="sxs-lookup"><span data-stu-id="136a3-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-recording-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="136a3-211">Java</span><span class="sxs-lookup"><span data-stu-id="136a3-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-recording-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="136a3-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="136a3-212">Response</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 302 Found
Location: https://01-a-noam.dog.attend.teams.microsoft.com/broadcast/909c6581-5130-43e9-88f3-fcb3582cde37/dc17674c-81d9-4adb-bfb2-8f6a442e4622/19%3Ameeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw%40thread.v2/0/resource/recording
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
