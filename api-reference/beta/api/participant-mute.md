---
title: 'participante: sem áudio'
description: Ativar mudo de um participante específico na chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 63ed2f659d79c005915b8ecf2e781e813e8f7044
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992441"
---
# <a name="participant-mute"></a><span data-ttu-id="5dc91-103">participante: sem áudio</span><span class="sxs-lookup"><span data-stu-id="5dc91-103">participant: mute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dc91-104">Ativar mudo de um participante específico na chamada.</span><span class="sxs-lookup"><span data-stu-id="5dc91-104">Mute a specific participant in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="5dc91-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5dc91-105">Permissions</span></span>
<span data-ttu-id="5dc91-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dc91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5dc91-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dc91-108">Permission type</span></span> | <span data-ttu-id="5dc91-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5dc91-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="5dc91-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dc91-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5dc91-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="5dc91-111">Not Supported</span></span>        |
| <span data-ttu-id="5dc91-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dc91-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dc91-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="5dc91-113">Not Supported</span></span>        |
| <span data-ttu-id="5dc91-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dc91-114">Application</span></span>     | <span data-ttu-id="5dc91-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5dc91-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="5dc91-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dc91-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/{id}/mute
POST /applications/{id}/calls/{id}/participants/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="5dc91-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc91-117">Request headers</span></span>
| <span data-ttu-id="5dc91-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5dc91-118">Name</span></span>          | <span data-ttu-id="5dc91-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dc91-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5dc91-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5dc91-120">Authorization</span></span> | <span data-ttu-id="5dc91-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5dc91-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5dc91-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc91-123">Request body</span></span>
<span data-ttu-id="5dc91-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dc91-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5dc91-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5dc91-125">Parameter</span></span>      | <span data-ttu-id="5dc91-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dc91-126">Type</span></span>    |<span data-ttu-id="5dc91-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dc91-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5dc91-128">clientContext</span><span class="sxs-lookup"><span data-stu-id="5dc91-128">clientContext</span></span>|<span data-ttu-id="5dc91-129">String</span><span class="sxs-lookup"><span data-stu-id="5dc91-129">String</span></span>|<span data-ttu-id="5dc91-130">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="5dc91-130">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="5dc91-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dc91-131">Response</span></span>
<span data-ttu-id="5dc91-132">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [commsOperation](../resources/commsoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5dc91-132">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dc91-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5dc91-133">Example</span></span>
<span data-ttu-id="5dc91-134">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5dc91-134">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5dc91-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc91-135">Request</span></span>
<span data-ttu-id="5dc91-136">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dc91-136">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5dc91-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="5dc91-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-mute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}/mute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5dc91-138">C#</span><span class="sxs-lookup"><span data-stu-id="5dc91-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5dc91-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="5dc91-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5dc91-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5dc91-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5dc91-141">Java</span><span class="sxs-lookup"><span data-stu-id="5dc91-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-mute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5dc91-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dc91-142">Response</span></span>

> <span data-ttu-id="5dc91-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5dc91-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.commsOperation",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

## <a name="example---mute-specific-participant"></a><span data-ttu-id="5dc91-145">Exemplo-sem áudio o participante específico</span><span class="sxs-lookup"><span data-stu-id="5dc91-145">Example - Mute specific participant</span></span>

##### <a name="request"></a><span data-ttu-id="5dc91-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc91-146">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/0698446E77E24E4D85F80597083CB830/mute
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="5dc91-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dc91-147">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation",
  "truncated": true
}-->
```json
{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="5dc91-148">Lista de notificação atualizada com o participante sem som</span><span class="sxs-lookup"><span data-stu-id="5dc91-148">Notification - roster updated with participant muted</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "0698446E77E24E4D85F80597083CB830",
          "info": {
            "identity": {
              "user": {
                "displayName": "Test User",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
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
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": true,
          "isInLobby": false
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "123456W77E24E4D85F80597083CB830",
          "info": {
            "identity": {
              "application": {
                "displayName": "Test Bot",
                "id": "1234A46B-3D17-4ADC-8DCE-DC4E7D556789"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
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
  "description": "participant: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
