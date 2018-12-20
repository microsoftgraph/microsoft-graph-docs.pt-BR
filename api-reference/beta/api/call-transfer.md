---
title: 'chamar: transferência'
description: Transferir uma chamada ativa.
author: VinodRavichandran
ms.openlocfilehash: 71d250453051c705dcc0646a8e4ad298253d0ee6
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380503"
---
# <a name="call-transfer"></a><span data-ttu-id="324a4-103">chamar: transferência</span><span class="sxs-lookup"><span data-stu-id="324a4-103">call: transfer</span></span>

> <span data-ttu-id="324a4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="324a4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="324a4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="324a4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="324a4-106">Transferir uma chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="324a4-106">Transfer an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="324a4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="324a4-107">Permissions</span></span>
<span data-ttu-id="324a4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="324a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="324a4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="324a4-110">Permission type</span></span> | <span data-ttu-id="324a4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="324a4-111">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="324a4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="324a4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="324a4-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="324a4-113">Not Supported</span></span>                |
| <span data-ttu-id="324a4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="324a4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="324a4-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="324a4-115">Not Supported</span></span>                |
| <span data-ttu-id="324a4-116">Application</span><span class="sxs-lookup"><span data-stu-id="324a4-116">Application</span></span>     | <span data-ttu-id="324a4-117">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="324a4-117">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="324a4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="324a4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /applications/{id}/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="324a4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="324a4-119">Request headers</span></span>
| <span data-ttu-id="324a4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="324a4-120">Name</span></span>          | <span data-ttu-id="324a4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="324a4-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="324a4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="324a4-122">Authorization</span></span> | <span data-ttu-id="324a4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="324a4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="324a4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="324a4-125">Request body</span></span>
<span data-ttu-id="324a4-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="324a4-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="324a4-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="324a4-127">Parameter</span></span>      | <span data-ttu-id="324a4-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="324a4-128">Type</span></span>    |<span data-ttu-id="324a4-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="324a4-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="324a4-130">transferTarget</span><span class="sxs-lookup"><span data-stu-id="324a4-130">transferTarget</span></span>|[<span data-ttu-id="324a4-131">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="324a4-131">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="324a4-132">O participante que é o destino da transferência.</span><span class="sxs-lookup"><span data-stu-id="324a4-132">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="324a4-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="324a4-133">clientContext</span></span>|<span data-ttu-id="324a4-134">String</span><span class="sxs-lookup"><span data-stu-id="324a4-134">String</span></span>|<span data-ttu-id="324a4-135">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="324a4-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="324a4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="324a4-136">Response</span></span>
<span data-ttu-id="324a4-137">Retorna `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="324a4-137">Returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="324a4-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="324a4-138">Examples</span></span>

### <a name="transfer-call-directly-with-no-user-involvement"></a><span data-ttu-id="324a4-139">Transferir a chamada diretamente, com nenhum envolvimento do usuário</span><span class="sxs-lookup"><span data-stu-id="324a4-139">Transfer call directly, with no user involvement</span></span>

<span data-ttu-id="324a4-140">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="324a4-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="324a4-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="324a4-141">Request</span></span>
<span data-ttu-id="324a4-142">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="324a4-142">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="324a4-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="324a4-143">Response</span></span>

> <span data-ttu-id="324a4-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="324a4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="324a4-146">Notificação - transferindo</span><span class="sxs-lookup"><span data-stu-id="324a4-146">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="324a4-147">Notificação - transferência aceito</span><span class="sxs-lookup"><span data-stu-id="324a4-147">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="324a4-148">Notificação - terminada</span><span class="sxs-lookup"><span data-stu-id="324a4-148">Notification - terminated</span></span>

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

### <a name="consultative-transfer"></a><span data-ttu-id="324a4-149">Transferência com consultoria</span><span class="sxs-lookup"><span data-stu-id="324a4-149">Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="324a4-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="324a4-150">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="324a4-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="324a4-151">Response</span></span>

> <span data-ttu-id="324a4-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="324a4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="324a4-154">Notificação - transferindo</span><span class="sxs-lookup"><span data-stu-id="324a4-154">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="324a4-155">Notificação - transferência aceito</span><span class="sxs-lookup"><span data-stu-id="324a4-155">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="324a4-156">Notificação - terminada</span><span class="sxs-lookup"><span data-stu-id="324a4-156">Notification - terminated</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "call: transfer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
