---
title: Criar mensagem
description: Use essa API para criar uma nova mensagem em uma pasta de email.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 50eac4d20ff5ce82298b74dbfff2da510bd49a27
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565426"
---
# <a name="create-message"></a><span data-ttu-id="7aeae-103">Criar mensagem</span><span class="sxs-lookup"><span data-stu-id="7aeae-103">Create Message</span></span>

<span data-ttu-id="7aeae-104">Use essa API para criar uma nova mensagem em uma pasta de email.</span><span class="sxs-lookup"><span data-stu-id="7aeae-104">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="7aeae-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7aeae-105">Permissions</span></span>
<span data-ttu-id="7aeae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7aeae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aeae-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7aeae-108">Permission type</span></span>      | <span data-ttu-id="7aeae-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7aeae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7aeae-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7aeae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7aeae-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7aeae-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7aeae-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7aeae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aeae-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7aeae-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7aeae-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7aeae-114">Application</span></span> | <span data-ttu-id="7aeae-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7aeae-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7aeae-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7aeae-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="7aeae-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7aeae-117">Request headers</span></span>
| <span data-ttu-id="7aeae-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7aeae-118">Header</span></span>       | <span data-ttu-id="7aeae-119">Valor</span><span class="sxs-lookup"><span data-stu-id="7aeae-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7aeae-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7aeae-120">Authorization</span></span>  | <span data-ttu-id="7aeae-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7aeae-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7aeae-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7aeae-123">Content-Type</span></span>  | <span data-ttu-id="7aeae-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7aeae-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7aeae-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7aeae-126">Request body</span></span>
<span data-ttu-id="7aeae-127">No corpo da solicitação, forneça uma representação JSON do objeto [Message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="7aeae-127">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7aeae-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aeae-128">Response</span></span>

<span data-ttu-id="7aeae-129">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7aeae-129">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7aeae-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7aeae-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7aeae-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7aeae-131">Request</span></span>
<span data-ttu-id="7aeae-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7aeae-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="7aeae-133">No corpo da solicitação, forneça uma representação JSON do objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="7aeae-133">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7aeae-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aeae-134">Response</span></span>
<span data-ttu-id="7aeae-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7aeae-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
