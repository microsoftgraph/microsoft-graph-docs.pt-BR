---
title: 'Call: transferência'
description: Transferir uma chamada ativa.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 97918efa4f55aa435214e15396283a4aa4e3cdd3
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418849"
---
# <a name="call-transfer"></a><span data-ttu-id="de669-103">Call: transferência</span><span class="sxs-lookup"><span data-stu-id="de669-103">call: transfer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de669-104">Transferir uma chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="de669-104">Transfer an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="de669-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="de669-105">Permissions</span></span>
<span data-ttu-id="de669-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de669-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de669-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de669-108">Permission type</span></span> | <span data-ttu-id="de669-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de669-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="de669-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de669-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="de669-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="de669-111">Not Supported</span></span>                |
| <span data-ttu-id="de669-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de669-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de669-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="de669-113">Not Supported</span></span>                |
| <span data-ttu-id="de669-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de669-114">Application</span></span>     | <span data-ttu-id="de669-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="de669-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="de669-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de669-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /applications/{id}/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="de669-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de669-117">Request headers</span></span>
| <span data-ttu-id="de669-118">Nome</span><span class="sxs-lookup"><span data-stu-id="de669-118">Name</span></span>          | <span data-ttu-id="de669-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="de669-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="de669-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="de669-120">Authorization</span></span> | <span data-ttu-id="de669-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de669-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de669-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de669-123">Request body</span></span>
<span data-ttu-id="de669-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de669-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="de669-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="de669-125">Parameter</span></span>      | <span data-ttu-id="de669-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="de669-126">Type</span></span>    |<span data-ttu-id="de669-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="de669-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de669-128">transferTarget</span><span class="sxs-lookup"><span data-stu-id="de669-128">transferTarget</span></span>|[<span data-ttu-id="de669-129">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="de669-129">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="de669-130">O participante que é o destino da transferência.</span><span class="sxs-lookup"><span data-stu-id="de669-130">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="de669-131">clientContext</span><span class="sxs-lookup"><span data-stu-id="de669-131">clientContext</span></span>|<span data-ttu-id="de669-132">String</span><span class="sxs-lookup"><span data-stu-id="de669-132">String</span></span>|<span data-ttu-id="de669-133">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="de669-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="de669-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="de669-134">Response</span></span>
<span data-ttu-id="de669-135">Retorna `202 Accepted` o código de resposta.</span><span class="sxs-lookup"><span data-stu-id="de669-135">Returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="de669-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="de669-136">Examples</span></span>

### <a name="transfer-call-directly-with-no-user-involvement"></a><span data-ttu-id="de669-137">Transferir a chamada diretamente, sem envolvimento do usuário</span><span class="sxs-lookup"><span data-stu-id="de669-137">Transfer call directly, with no user involvement</span></span>

<span data-ttu-id="de669-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="de669-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="de669-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de669-139">Request</span></span>
<span data-ttu-id="de669-140">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="de669-140">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="de669-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="de669-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/transfer
Content-Type: application/json
Content-Length: 430

{
  "transferTarget": {
    "endpointType": "default",
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value",
    "replacesCallId": "replacesCallId-value"
  },
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="de669-142">C#</span><span class="sxs-lookup"><span data-stu-id="de669-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de669-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de669-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de669-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="de669-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="de669-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="de669-145">Response</span></span>

> <span data-ttu-id="de669-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de669-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="de669-148">Notificação-Transferindo</span><span class="sxs-lookup"><span data-stu-id="de669-148">Notification - transferring</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferring"
        },
        "status": "running"
      }
    }
  ]
}
```

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="de669-149">Notificação-transferência aceita</span><span class="sxs-lookup"><span data-stu-id="de669-149">Notification - transfer accepted</span></span>

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
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferAccepted"
        },
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="de669-150">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="de669-150">Notification - terminated</span></span>

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
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "terminationReason": "AppTransferred"
      }
    }
  ]
}
```

### <a name="consultative-transfer"></a><span data-ttu-id="de669-151">Transferência consultiva</span><span class="sxs-lookup"><span data-stu-id="de669-151">Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="de669-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de669-152">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/transfer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```
<!-- {
  "blockType": "ignored",
  "@odata.type": "call-transfer"
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "transferTarget": {
    "endpointType": "default",
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-US",
    "region": "westus",
    "replacesCallId": "e5d39592-99bd-4db8-bca8-30fb894ec51d"
  }
}
```

##### <a name="response"></a><span data-ttu-id="de669-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="de669-153">Response</span></span>

> <span data-ttu-id="de669-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de669-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="de669-156">Notificação-Transferindo</span><span class="sxs-lookup"><span data-stu-id="de669-156">Notification - transferring</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferring"
        },
        "status": "running"
      }
    }
  ]
}
```

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="de669-157">Notificação-transferência aceita</span><span class="sxs-lookup"><span data-stu-id="de669-157">Notification - transfer accepted</span></span>

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
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferAccepted"
        },
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="de669-158">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="de669-158">Notification - terminated</span></span>

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
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "terminationReason": "AppTransferred"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: transfer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
