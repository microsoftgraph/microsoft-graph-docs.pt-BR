---
title: 'Call: changeScreenSharingRole'
description: Permitir que os aplicativos compartilhem conteúdo de tela com os participantes de uma chamada de grupo.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 333a9a2ebb6fa5b3c43ccee47f0256ef5ba6dee3
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912766"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="3e05f-103">Call: changeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="3e05f-103">call: changeScreenSharingRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e05f-104">Permitir que os aplicativos compartilhem conteúdo de tela com os participantes de uma chamada de grupo.</span><span class="sxs-lookup"><span data-stu-id="3e05f-104">Allow applications to share screen content with the participants of a group call.</span></span>

> <span data-ttu-id="3e05f-105">**Observação:** Isso só é suportado para chamadas de grupo que usam mídia hospedada em aplicativos.</span><span class="sxs-lookup"><span data-stu-id="3e05f-105">**Note:** This is only supported for group calls that use App-Hosted Media.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e05f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e05f-106">Permissions</span></span>
<span data-ttu-id="3e05f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e05f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e05f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e05f-109">Permission type</span></span>                        | <span data-ttu-id="3e05f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e05f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3e05f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e05f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e05f-112">Não suportado</span><span class="sxs-lookup"><span data-stu-id="3e05f-112">Not Supported</span></span>                               |
| <span data-ttu-id="3e05f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e05f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e05f-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="3e05f-114">Not Supported</span></span>                               |
| <span data-ttu-id="3e05f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e05f-115">Application</span></span>                            | <span data-ttu-id="3e05f-116">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="3e05f-116">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="3e05f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e05f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /communications/calls/{id}/changeScreenSharingRole
```
> <span data-ttu-id="3e05f-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="3e05f-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="3e05f-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="3e05f-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e05f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e05f-120">Request headers</span></span>
| <span data-ttu-id="3e05f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3e05f-121">Name</span></span>          | <span data-ttu-id="3e05f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e05f-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3e05f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e05f-123">Authorization</span></span> | <span data-ttu-id="3e05f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e05f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e05f-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="3e05f-126">Content-type</span></span>  | <span data-ttu-id="3e05f-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e05f-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e05f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e05f-129">Request body</span></span>
<span data-ttu-id="3e05f-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e05f-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3e05f-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3e05f-131">Parameter</span></span>      | <span data-ttu-id="3e05f-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e05f-132">Type</span></span>    |<span data-ttu-id="3e05f-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e05f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e05f-134">role</span><span class="sxs-lookup"><span data-stu-id="3e05f-134">role</span></span>|<span data-ttu-id="3e05f-135">String</span><span class="sxs-lookup"><span data-stu-id="3e05f-135">String</span></span>|<span data-ttu-id="3e05f-136">Os valores possíveis são: ' Visualizador ', ' participante '</span><span class="sxs-lookup"><span data-stu-id="3e05f-136">Possible values are: 'viewer', 'sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="3e05f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e05f-137">Response</span></span>
<span data-ttu-id="3e05f-138">Se tiver êxito, este método retornará `202 Accepted` um código de resposta e todos os participantes receberão uma atualização de lista.</span><span class="sxs-lookup"><span data-stu-id="3e05f-138">If successful, this method returns a `202 Accepted` response code, and all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="3e05f-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e05f-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3e05f-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e05f-140">Request</span></span>
<span data-ttu-id="3e05f-141">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e05f-141">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3e05f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e05f-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3e05f-143">C#</span><span class="sxs-lookup"><span data-stu-id="3e05f-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-changescreensharingrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e05f-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e05f-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-changescreensharingrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3e05f-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e05f-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-changescreensharingrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3e05f-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e05f-146">Response</span></span>
<span data-ttu-id="3e05f-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e05f-147">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---roster-updated-with-participant-sending-screen-sharing-video"></a><span data-ttu-id="3e05f-148">Lista de notificação atualizada com o participante enviando vídeo de compartilhamento de tela</span><span class="sxs-lookup"><span data-stu-id="3e05f-148">Notification - roster updated with participant sending screen sharing video</span></span>
<span data-ttu-id="3e05f-149">Observe a `direction: sendOnly` Propriedade no fluxo de mídia.</span><span class="sxs-lookup"><span data-stu-id="3e05f-149">Note the `direction: sendOnly` property on the media stream.</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "2765eb15-01f8-47c6-b12b-c32111a4a86f",
          "info": {
            "identity": {
              "user": {
                "displayName": "Bob",
                "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "videoBasedScreenSharing",
              "label": "applicationsharing-video",
              "sourceId": "1",
              "direction": "sendOnly"
            }
          ],
          "isMuted": false,
          "isInLobby": false
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
