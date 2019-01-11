---
title: 'message: createForward'
description: Crie um rascunho para encaminhar a mensagem especificada. Você pode atualizar o rascunho para adicionar conteúdo ao **corpo** ou alterar outras propriedades da mensagem ou, simplesmente, enviar o rascunho.
localization_priority: Normal
ms.openlocfilehash: 230fdfd4a1700e5bcbe2e1cb364de08d86c7be39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888260"
---
# <a name="message-createforward"></a><span data-ttu-id="4d438-104">message: createForward</span><span class="sxs-lookup"><span data-stu-id="4d438-104">message: createForward</span></span>

<span data-ttu-id="4d438-105">Crie um rascunho para encaminhar a [mensagem](../resources/message.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="4d438-105">Create a draft to forward the specified [message](../resources/message.md).</span></span> <span data-ttu-id="4d438-106">Você pode [atualizar](../api/message-update.md) o rascunho para adicionar conteúdo ao **corpo** ou alterar outras propriedades da mensagem ou, simplesmente, [enviar](../api/message-send.md) o rascunho.</span><span class="sxs-lookup"><span data-stu-id="4d438-106">You can then [update](../api/message-update.md) the draft to add content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d438-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d438-107">Permissions</span></span>

<span data-ttu-id="4d438-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d438-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d438-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d438-110">Permission type</span></span>      | <span data-ttu-id="4d438-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d438-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d438-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d438-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4d438-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d438-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4d438-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d438-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d438-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d438-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4d438-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d438-116">Application</span></span> | <span data-ttu-id="4d438-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d438-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d438-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d438-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```

## <a name="request-headers"></a><span data-ttu-id="4d438-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d438-119">Request headers</span></span>

| <span data-ttu-id="4d438-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4d438-120">Name</span></span>       | <span data-ttu-id="4d438-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d438-121">Type</span></span> | <span data-ttu-id="4d438-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d438-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4d438-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d438-123">Authorization</span></span>  | <span data-ttu-id="4d438-124">string</span><span class="sxs-lookup"><span data-stu-id="4d438-124">string</span></span>  | <span data-ttu-id="4d438-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d438-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d438-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d438-127">Request body</span></span>

<span data-ttu-id="4d438-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4d438-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d438-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d438-129">Response</span></span>

<span data-ttu-id="4d438-130">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d438-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d438-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d438-131">Example</span></span>

<span data-ttu-id="4d438-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4d438-132">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4d438-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d438-133">Request</span></span>

<span data-ttu-id="4d438-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d438-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createForward
```

##### <a name="response"></a><span data-ttu-id="4d438-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d438-135">Response</span></span>

<span data-ttu-id="4d438-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d438-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
