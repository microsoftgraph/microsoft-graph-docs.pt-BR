---
title: Criar mensagem
description: Use essa API para criar uma nova mensagem em uma pasta de email.
author: angelgolfer-ms
ms.openlocfilehash: 0db7150c358065c6333091fd27754a8da969d673
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331335"
---
# <a name="create-message"></a><span data-ttu-id="64dfc-103">Criar mensagem</span><span class="sxs-lookup"><span data-stu-id="64dfc-103">Create Message</span></span>

> <span data-ttu-id="64dfc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="64dfc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64dfc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="64dfc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64dfc-106">Use essa API para criar uma nova mensagem em uma pasta de email.</span><span class="sxs-lookup"><span data-stu-id="64dfc-106">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="64dfc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="64dfc-107">Permissions</span></span>
<span data-ttu-id="64dfc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64dfc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64dfc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64dfc-110">Permission type</span></span>      | <span data-ttu-id="64dfc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64dfc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64dfc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64dfc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="64dfc-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64dfc-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="64dfc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64dfc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64dfc-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64dfc-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="64dfc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64dfc-116">Application</span></span> | <span data-ttu-id="64dfc-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64dfc-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="64dfc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64dfc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="64dfc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64dfc-119">Request headers</span></span>
| <span data-ttu-id="64dfc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64dfc-120">Header</span></span>       | <span data-ttu-id="64dfc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="64dfc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="64dfc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="64dfc-122">Authorization</span></span>  | <span data-ttu-id="64dfc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64dfc-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="64dfc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64dfc-125">Content-Type</span></span>  | <span data-ttu-id="64dfc-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64dfc-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="64dfc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64dfc-128">Request body</span></span>
<span data-ttu-id="64dfc-129">No corpo da solicitação, forneça uma representação JSON do objeto [Message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="64dfc-129">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="64dfc-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="64dfc-130">Response</span></span>

<span data-ttu-id="64dfc-131">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64dfc-131">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64dfc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64dfc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64dfc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64dfc-133">Request</span></span>
<span data-ttu-id="64dfc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64dfc-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/messages
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```
<span data-ttu-id="64dfc-135">No corpo da solicitação, forneça uma representação JSON do objeto [message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="64dfc-135">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="64dfc-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="64dfc-136">Response</span></span>
<span data-ttu-id="64dfc-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64dfc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
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
