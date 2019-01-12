---
title: Atualizar conversationthread
description: Bloqueia ou desbloqueia um thread, para permitir ou evitar postar ainda mais no thread.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 99ed0a7c635fc02bd0b0c6ea485e18a5875d8fe2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985078"
---
# <a name="update-conversationthread"></a><span data-ttu-id="51f77-103">Atualizar conversationthread</span><span class="sxs-lookup"><span data-stu-id="51f77-103">Update conversationthread</span></span>

> <span data-ttu-id="51f77-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="51f77-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51f77-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="51f77-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51f77-106">Bloqueia ou desbloqueia um thread, para permitir ou evitar postar ainda mais no thread.</span><span class="sxs-lookup"><span data-stu-id="51f77-106">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="51f77-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="51f77-107">Permissions</span></span>
<span data-ttu-id="51f77-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51f77-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51f77-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51f77-110">Permission type</span></span>      | <span data-ttu-id="51f77-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51f77-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51f77-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51f77-112">Delegated (work or school account)</span></span> | <span data-ttu-id="51f77-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51f77-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="51f77-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51f77-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51f77-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51f77-115">Not supported.</span></span>    |
|<span data-ttu-id="51f77-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51f77-116">Application</span></span> | <span data-ttu-id="51f77-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51f77-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="51f77-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51f77-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="51f77-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51f77-119">Request headers</span></span>
| <span data-ttu-id="51f77-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51f77-120">Header</span></span>       | <span data-ttu-id="51f77-121">Valor</span><span class="sxs-lookup"><span data-stu-id="51f77-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="51f77-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="51f77-122">Authorization</span></span>  | <span data-ttu-id="51f77-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51f77-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="51f77-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51f77-125">Content-Type</span></span>  | <span data-ttu-id="51f77-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51f77-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51f77-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51f77-128">Request body</span></span>
<span data-ttu-id="51f77-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="51f77-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="51f77-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51f77-132">Property</span></span>     | <span data-ttu-id="51f77-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="51f77-133">Type</span></span>   |<span data-ttu-id="51f77-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="51f77-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51f77-135">isLocked</span><span class="sxs-lookup"><span data-stu-id="51f77-135">isLocked</span></span>|<span data-ttu-id="51f77-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="51f77-136">Boolean</span></span>|<span data-ttu-id="51f77-p106">Indica se o thread está bloqueado. Defina como `true` para proibir a postagem.</span><span class="sxs-lookup"><span data-stu-id="51f77-p106">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="51f77-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="51f77-139">Response</span></span>

<span data-ttu-id="51f77-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversationThread](../resources/conversationthread.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51f77-140">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="51f77-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51f77-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51f77-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51f77-142">Request</span></span>
<span data-ttu-id="51f77-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51f77-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_conversationthread"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups/{id}/threads/{id}
Content-type: application/json
Content-length: 419

{
  "@odata.type":"#Microsoft.OutlookServices.ConversationThread",
  "isLocked": true
}
```
##### <a name="response"></a><span data-ttu-id="51f77-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="51f77-144">Response</span></span>
<span data-ttu-id="51f77-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51f77-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "isLocked": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update conversationthread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
