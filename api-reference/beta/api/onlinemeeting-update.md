---
title: Atualizar onlineMeeting
description: Atualizar as propriedades de uma reunião online.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6699071afe0fb8b7e6ec2183e29785558a2c5d48
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292165"
---
# <a name="update-onlinemeeting"></a><span data-ttu-id="1a4ad-103">Atualizar onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="1a4ad-103">Update onlineMeeting</span></span>

<span data-ttu-id="1a4ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a4ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a4ad-105">Atualize **startDateTime**, **endDateTime**,  **participantes** e propriedades de assunto do [onlineMeeting especificado.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="1a4ad-105">Update the **startDateTime**, **endDateTime**, **participants**, and **subject** properties of the specified [onlineMeeting](../resources/onlinemeeting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1a4ad-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a4ad-106">Permissions</span></span>

| <span data-ttu-id="1a4ad-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a4ad-107">Permission type</span></span>                        | <span data-ttu-id="1a4ad-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a4ad-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="1a4ad-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a4ad-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a4ad-110">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a4ad-110">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="1a4ad-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a4ad-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a4ad-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a4ad-112">Not Supported.</span></span>                              |
| <span data-ttu-id="1a4ad-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a4ad-113">Application</span></span>                            | <span data-ttu-id="1a4ad-114">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="1a4ad-114">OnlineMeetings.ReadWrite.All\*</span></span>                |

> [!IMPORTANT]
> <span data-ttu-id="1a4ad-115">\*Os administradores [](/graph/cloud-communication-online-meeting-application-access-policy) devem criar uma política de acesso a aplicativos e concedi-la a um usuário, autorizando o aplicativo configurado na política a atualizar uma reunião online em nome desse usuário (ID de usuário especificada no caminho da solicitação).</span><span class="sxs-lookup"><span data-stu-id="1a4ad-115">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to update an online meeting on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="1a4ad-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a4ad-116">HTTP request</span></span>
<span data-ttu-id="1a4ad-117">Para atualizar o onlineMeeting especificado pela ID de reunião com o token delegado:</span><span class="sxs-lookup"><span data-stu-id="1a4ad-117">To update the specified onlineMeeting by meeting ID with delegated token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onlineMeetings/{meetingId}
```

<span data-ttu-id="1a4ad-118">Para atualizar o onlineMeeting especificado pela ID de reunião com o token de aplicativo:</span><span class="sxs-lookup"><span data-stu-id="1a4ad-118">To update the specified onlineMeeting by meeting ID with application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{userId}/onlineMeetings/{meetingId}
```

> <span data-ttu-id="1a4ad-119">**Observações:**</span><span class="sxs-lookup"><span data-stu-id="1a4ad-119">**Notes:**</span></span>
> - <span data-ttu-id="1a4ad-120">`userId`é a ID de objeto de um usuário no portal de gerenciamento de usuários [do Azure.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="1a4ad-120">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="1a4ad-121">Para obter mais detalhes, consulte política [de acesso ao aplicativo.](/graph/cloud-communication-online-meeting-application-access-policy)</span><span class="sxs-lookup"><span data-stu-id="1a4ad-121">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
> - <span data-ttu-id="1a4ad-122">`meetingId`é a **id de** um [objeto onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="1a4ad-122">`meetingId` is the **id** of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a4ad-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a4ad-123">Request headers</span></span>
| <span data-ttu-id="1a4ad-124">Nome</span><span class="sxs-lookup"><span data-stu-id="1a4ad-124">Name</span></span>          | <span data-ttu-id="1a4ad-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a4ad-125">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="1a4ad-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a4ad-126">Authorization</span></span> | <span data-ttu-id="1a4ad-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a4ad-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="1a4ad-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="1a4ad-129">Content-type</span></span>  | <span data-ttu-id="1a4ad-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a4ad-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a4ad-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a4ad-132">Request body</span></span>
<span data-ttu-id="1a4ad-133">No corpo da solicitação, forneça uma representação JSON do objeto [onlineMeeting](../resources/onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="1a4ad-133">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span> <span data-ttu-id="1a4ad-134">Somente as **propriedades startDateTime**, **endDateTime**, **participantes** e **assunto** podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="1a4ad-134">Only the **startDateTime**, **endDateTime**, **participants**, and **subject** properties can be modified.</span></span> <span data-ttu-id="1a4ad-135">**StartDateTime e** **endDateTime** devem aparecer em pares.</span><span class="sxs-lookup"><span data-stu-id="1a4ad-135">The **startDateTime** and **endDateTime** must appear in pairs.</span></span>

## <a name="response"></a><span data-ttu-id="1a4ad-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a4ad-136">Response</span></span>
<span data-ttu-id="1a4ad-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a4ad-137">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a4ad-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1a4ad-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1a4ad-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a4ad-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1a4ad-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a4ad-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_onlinemeeting_request"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/{id}
Content-Type: application/json 

{
  "startDateTime": "2020-09-09T14:33:30.8546353-07:00",
  "endDateTime": "2020-09-09T15:03:30.8566356-07:00",
  "subject": "Patch Meeting Subject"
}
```
# <a name="c"></a>[<span data-ttu-id="1a4ad-141">C#</span><span class="sxs-lookup"><span data-stu-id="1a4ad-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-onlinemeeting-request-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a4ad-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a4ad-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-onlinemeeting-request-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a4ad-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a4ad-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-onlinemeeting-request-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a4ad-144">Java</span><span class="sxs-lookup"><span data-stu-id="1a4ad-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-onlinemeeting-request-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1a4ad-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a4ad-145">Response</span></span>

><span data-ttu-id="1a4ad-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1a4ad-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "id":"{id}",
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
      "tollNumber":"number",
      "tollFreeNumber":null,
      "dialinUrl":"url"
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


