---
title: Criar mensagem
description: Use essa API para criar uma nova mensagem em uma pasta de email.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6943331c260d4ac18718c46f39dfc870aded584f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984898"
---
# <a name="create-message"></a><span data-ttu-id="31907-103">Criar mensagem</span><span class="sxs-lookup"><span data-stu-id="31907-103">Create Message</span></span>

<span data-ttu-id="31907-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31907-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="31907-105">Use essa API para criar uma nova mensagem em uma pasta de email.</span><span class="sxs-lookup"><span data-stu-id="31907-105">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="31907-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="31907-106">Permissions</span></span>
<span data-ttu-id="31907-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31907-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31907-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31907-109">Permission type</span></span>      | <span data-ttu-id="31907-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31907-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31907-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31907-111">Delegated (work or school account)</span></span> | <span data-ttu-id="31907-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31907-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="31907-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31907-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31907-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31907-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="31907-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31907-115">Application</span></span> | <span data-ttu-id="31907-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31907-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="31907-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31907-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="31907-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31907-118">Request headers</span></span>
| <span data-ttu-id="31907-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31907-119">Header</span></span>       | <span data-ttu-id="31907-120">Valor</span><span class="sxs-lookup"><span data-stu-id="31907-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="31907-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="31907-121">Authorization</span></span>  | <span data-ttu-id="31907-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31907-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="31907-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31907-124">Content-Type</span></span>  | <span data-ttu-id="31907-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31907-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="31907-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31907-127">Request body</span></span>
<span data-ttu-id="31907-128">No corpo da solicitação, forneça uma representação JSON do objeto [Message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="31907-128">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="31907-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="31907-129">Response</span></span>

<span data-ttu-id="31907-130">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31907-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31907-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31907-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31907-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31907-132">Request</span></span>
<span data-ttu-id="31907-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31907-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="31907-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="31907-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```
# <a name="c"></a>[<span data-ttu-id="31907-135">C#</span><span class="sxs-lookup"><span data-stu-id="31907-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31907-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31907-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31907-137">Java</span><span class="sxs-lookup"><span data-stu-id="31907-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="31907-138">No corpo da solicitação, forneça uma representação JSON do objeto [mensagem](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="31907-138">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="31907-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="31907-139">Response</span></span>
<span data-ttu-id="31907-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31907-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

