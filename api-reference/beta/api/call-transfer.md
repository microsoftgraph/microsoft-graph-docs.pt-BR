---
title: 'Call: transferência'
description: Transferir uma chamada ativa.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 96f5e7cdcd9996eb409743186a03239949f4e727
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792284"
---
# <a name="call-transfer"></a><span data-ttu-id="8a0b7-103">Call: transferência</span><span class="sxs-lookup"><span data-stu-id="8a0b7-103">call: transfer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a0b7-104">Transferir uma chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="8a0b7-104">Transfer an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a0b7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a0b7-105">Permissions</span></span>
<span data-ttu-id="8a0b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a0b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8a0b7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a0b7-108">Permission type</span></span> | <span data-ttu-id="8a0b7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a0b7-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="8a0b7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a0b7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8a0b7-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="8a0b7-111">Not Supported</span></span>                |
| <span data-ttu-id="8a0b7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a0b7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a0b7-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="8a0b7-113">Not Supported</span></span>                |
| <span data-ttu-id="8a0b7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a0b7-114">Application</span></span>     | <span data-ttu-id="8a0b7-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="8a0b7-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="8a0b7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a0b7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="8a0b7-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a0b7-117">Request headers</span></span>
| <span data-ttu-id="8a0b7-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8a0b7-118">Name</span></span>          | <span data-ttu-id="8a0b7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a0b7-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8a0b7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a0b7-120">Authorization</span></span> | <span data-ttu-id="8a0b7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a0b7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a0b7-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a0b7-123">Request body</span></span>
<span data-ttu-id="8a0b7-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a0b7-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8a0b7-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8a0b7-125">Parameter</span></span>      | <span data-ttu-id="8a0b7-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a0b7-126">Type</span></span>    |<span data-ttu-id="8a0b7-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a0b7-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a0b7-128">transferTarget</span><span class="sxs-lookup"><span data-stu-id="8a0b7-128">transferTarget</span></span>|[<span data-ttu-id="8a0b7-129">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="8a0b7-129">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="8a0b7-130">O participante que é o destino da transferência.</span><span class="sxs-lookup"><span data-stu-id="8a0b7-130">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="8a0b7-131">clientContext</span><span class="sxs-lookup"><span data-stu-id="8a0b7-131">clientContext</span></span>|<span data-ttu-id="8a0b7-132">String</span><span class="sxs-lookup"><span data-stu-id="8a0b7-132">String</span></span>|<span data-ttu-id="8a0b7-133">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="8a0b7-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="8a0b7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a0b7-134">Response</span></span>
<span data-ttu-id="8a0b7-135">Retorna `202 Accepted` o código de resposta.</span><span class="sxs-lookup"><span data-stu-id="8a0b7-135">Returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8a0b7-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8a0b7-136">Examples</span></span>

### <a name="transfer-call-directly-with-no-user-involvement"></a><span data-ttu-id="8a0b7-137">Transferir a chamada diretamente, sem envolvimento do usuário</span><span class="sxs-lookup"><span data-stu-id="8a0b7-137">Transfer call directly, with no user involvement</span></span>

<span data-ttu-id="8a0b7-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8a0b7-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8a0b7-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a0b7-139">Request</span></span>
<span data-ttu-id="8a0b7-140">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a0b7-140">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8a0b7-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a0b7-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8a0b7-142">C#</span><span class="sxs-lookup"><span data-stu-id="8a0b7-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8a0b7-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a0b7-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8a0b7-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8a0b7-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8a0b7-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a0b7-145">Response</span></span>

> <span data-ttu-id="8a0b7-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a0b7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="8a0b7-148">Notificação-Transferindo</span><span class="sxs-lookup"><span data-stu-id="8a0b7-148">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="8a0b7-149">Notificação-transferência aceita</span><span class="sxs-lookup"><span data-stu-id="8a0b7-149">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="8a0b7-150">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="8a0b7-150">Notification - terminated</span></span>

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

### <a name="consultative-transfer"></a><span data-ttu-id="8a0b7-151">Transferência consultiva</span><span class="sxs-lookup"><span data-stu-id="8a0b7-151">Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="8a0b7-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a0b7-152">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="8a0b7-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a0b7-153">Response</span></span>

> <span data-ttu-id="8a0b7-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a0b7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="8a0b7-156">Notificação-Transferindo</span><span class="sxs-lookup"><span data-stu-id="8a0b7-156">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="8a0b7-157">Notificação-transferência aceita</span><span class="sxs-lookup"><span data-stu-id="8a0b7-157">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="8a0b7-158">Notificação-terminada</span><span class="sxs-lookup"><span data-stu-id="8a0b7-158">Notification - terminated</span></span>

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
