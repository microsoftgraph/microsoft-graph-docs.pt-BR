---
title: 'chamada: ativar mudo'
description: Permitir que o aplicativo se desative sozinho.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: de47162a9a2c3b4baf31f8b3b11f50100730d3b9
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747578"
---
# <a name="call-unmute"></a><span data-ttu-id="77902-103">chamada: ativar mudo</span><span class="sxs-lookup"><span data-stu-id="77902-103">call: unmute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77902-104">Permitir que o aplicativo se desative sozinho.</span><span class="sxs-lookup"><span data-stu-id="77902-104">Allow the application to unmute itself.</span></span>

<span data-ttu-id="77902-105">Este é um servidor que está desativado, o que significa que o servidor começará a enviar pacotes de áudio para este participante a outros participantes novamente.</span><span class="sxs-lookup"><span data-stu-id="77902-105">This is a server unmute, meaning that the server will start sending audio packets for this participant to other participants again.</span></span>

<span data-ttu-id="77902-106">Para obter mais informações sobre como lidar com as operações de desativação, consulte [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md).</span><span class="sxs-lookup"><span data-stu-id="77902-106">For more information about how to handle unmute operations, see [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md).</span></span>

> <span data-ttu-id="77902-107">**Observação:** Este método só tem suporte para chamadas de grupo.</span><span class="sxs-lookup"><span data-stu-id="77902-107">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="77902-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="77902-108">Permissions</span></span>

| <span data-ttu-id="77902-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77902-109">Permission type</span></span>                        | <span data-ttu-id="77902-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77902-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="77902-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77902-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="77902-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77902-112">Not supported.</span></span>                               |
| <span data-ttu-id="77902-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77902-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77902-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77902-114">Not supported.</span></span>                               |
| <span data-ttu-id="77902-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77902-115">Application</span></span>                            | <span data-ttu-id="77902-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="77902-116">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="77902-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77902-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/unmute
POST /communications/calls/{id}/unmute
```
> <span data-ttu-id="77902-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="77902-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="77902-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="77902-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77902-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77902-120">Request headers</span></span>
| <span data-ttu-id="77902-121">Nome</span><span class="sxs-lookup"><span data-stu-id="77902-121">Name</span></span>          | <span data-ttu-id="77902-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="77902-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="77902-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="77902-123">Authorization</span></span> | <span data-ttu-id="77902-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77902-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="77902-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="77902-126">Content-type</span></span> | <span data-ttu-id="77902-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77902-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="77902-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77902-129">Request body</span></span>
<span data-ttu-id="77902-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77902-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="77902-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="77902-131">Parameter</span></span>      | <span data-ttu-id="77902-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="77902-132">Type</span></span>    |<span data-ttu-id="77902-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="77902-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77902-134">clientContext</span><span class="sxs-lookup"><span data-stu-id="77902-134">clientContext</span></span>|<span data-ttu-id="77902-135">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="77902-135">String</span></span>|<span data-ttu-id="77902-136">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="77902-136">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="77902-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="77902-137">Response</span></span>
<span data-ttu-id="77902-138">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77902-138">If successful, this method returns a `200 OK` response code and a [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md) object in the response body.</span></span>

><span data-ttu-id="77902-139">**Observação:** Quando essa API retornar uma resposta bem-sucedida, todos os participantes receberão uma atualização de lista.</span><span class="sxs-lookup"><span data-stu-id="77902-139">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="77902-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77902-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="77902-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77902-141">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="77902-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="77902-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-unmute"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/unmute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="77902-143">C#</span><span class="sxs-lookup"><span data-stu-id="77902-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-unmute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77902-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77902-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-unmute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77902-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77902-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-unmute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="77902-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="77902-146">Response</span></span>

> <span data-ttu-id="77902-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77902-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unmuteParticipantOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.unmuteParticipantOperation",
  "truncated": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.unmuteParticipantOperation",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#unmuteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "clientContext-value"
}
```

##### <a name="notification---roster-updated-with-participant-unmuted"></a><span data-ttu-id="77902-149">Lista de notificação atualizada com o participante sem som</span><span class="sxs-lookup"><span data-stu-id="77902-149">Notification - roster updated with participant unmuted</span></span>

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
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "1",
              "direction": "sendReceive"
            }
          ],
          "isMuted": false, // will be set to false on unmute
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
  "description": "call: unmute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
