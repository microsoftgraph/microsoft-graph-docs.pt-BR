---
title: 'message: unsubscribe'
description: Envia uma solicitação de e-mail em nome do usuário conectado para cancelar a assinatura de uma lista de distribuição de e-mail. Usa as informações do cabeçalho `List-Unsubscribe`.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7bf800fe385c75c6d472f9cee40f55ec81633640
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131093"
---
# <a name="message-unsubscribe"></a><span data-ttu-id="838ae-104">message: unsubscribe</span><span class="sxs-lookup"><span data-stu-id="838ae-104">message: unsubscribe</span></span>

<span data-ttu-id="838ae-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="838ae-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="838ae-106">Envia uma solicitação de e-mail em nome do usuário conectado para cancelar a assinatura de uma lista de distribuição de e-mail.</span><span class="sxs-lookup"><span data-stu-id="838ae-106">Submits a email request on behalf of the signed-in user to unsubscribe from an email distribution list.</span></span> <span data-ttu-id="838ae-107">Usa as informações do cabeçalho `List-Unsubscribe`.</span><span class="sxs-lookup"><span data-stu-id="838ae-107">Uses the information in the `List-Unsubscribe` header.</span></span>

<span data-ttu-id="838ae-108">Os destinatários de mensagens podem usar listas de email de maneira amigável, incluindo uma opção para os destinatários a rechaem. Eles podem fazer isso especificando o `List-Unsubscribe` header em cada mensagem após [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span><span class="sxs-lookup"><span data-stu-id="838ae-108">Message senders can use mailing lists in a user-friendly way by including an option for recipients to opt out. They can do so by specifying the `List-Unsubscribe` header in each message following [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span></span>

<span data-ttu-id="838ae-109">**Observação** Em particular, para que **a ação de** cancelamento de assinatura funcione, o remetente deve especificar, e não com base em URL, informações de cancelamento de `mailto:` assinatura.</span><span class="sxs-lookup"><span data-stu-id="838ae-109">**Note** In particular, for the **unsubscribe** action to work, the sender must specify `mailto:` and not URL-based unsubscribe information.</span></span>

<span data-ttu-id="838ae-110">Definir esse header também definiria a propriedade [](../resources/message.md) **unsubscribeEnabled** da instância da mensagem como e a propriedade `true` **unsubscribeData** para os dados do header.</span><span class="sxs-lookup"><span data-stu-id="838ae-110">Setting that header would also set the **unsubscribeEnabled** property of the [message](../resources/message.md) instance to `true`, and the **unsubscribeData** property to the header data.</span></span>

<span data-ttu-id="838ae-111">Se a **propriedade unsubscribeEnabled** de uma mensagem for , você pode usar a ação de cancelar a assinatura do usuário de mensagens futuras semelhantes, como gerenciadas pelo remetente `true` da mensagem. </span><span class="sxs-lookup"><span data-stu-id="838ae-111">If the **unsubscribeEnabled** property of a message is `true`, you can use the **unsubscribe** action to unsubscribe the user from similar future messages as managed by the message sender.</span></span>

<span data-ttu-id="838ae-112">Uma ação **de cancelamento de** assinatura bem-sucedida move a mensagem para a pasta Itens **Excluídos.**</span><span class="sxs-lookup"><span data-stu-id="838ae-112">A successful **unsubscribe** action moves the message to the **Deleted Items** folder.</span></span> <span data-ttu-id="838ae-113">A exclusão do usuário dos destinatários de futuros e-mails é gerenciada pelo remetente.</span><span class="sxs-lookup"><span data-stu-id="838ae-113">The actual exclusion of the user from future mail distribution is managed by the sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="838ae-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="838ae-114">Permissions</span></span>
<span data-ttu-id="838ae-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="838ae-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="838ae-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="838ae-117">Permission type</span></span>      | <span data-ttu-id="838ae-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="838ae-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="838ae-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="838ae-119">Delegated (work or school account)</span></span> | <span data-ttu-id="838ae-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="838ae-120">Mail.Send</span></span>    |
|<span data-ttu-id="838ae-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="838ae-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="838ae-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="838ae-122">Mail.Send</span></span>    |
|<span data-ttu-id="838ae-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="838ae-123">Application</span></span> | <span data-ttu-id="838ae-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="838ae-124">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="838ae-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="838ae-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a><span data-ttu-id="838ae-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="838ae-126">Request headers</span></span>
| <span data-ttu-id="838ae-127">Nome</span><span class="sxs-lookup"><span data-stu-id="838ae-127">Name</span></span>       | <span data-ttu-id="838ae-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="838ae-128">Type</span></span> | <span data-ttu-id="838ae-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="838ae-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="838ae-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="838ae-130">Authorization</span></span>  | <span data-ttu-id="838ae-131">string</span><span class="sxs-lookup"><span data-stu-id="838ae-131">string</span></span>  | <span data-ttu-id="838ae-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="838ae-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="838ae-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="838ae-134">Request body</span></span>
<span data-ttu-id="838ae-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="838ae-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="838ae-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="838ae-136">Response</span></span>

<span data-ttu-id="838ae-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="838ae-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="838ae-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="838ae-139">Example</span></span>
<span data-ttu-id="838ae-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="838ae-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="838ae-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="838ae-141">Request</span></span>
<span data-ttu-id="838ae-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="838ae-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="838ae-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="838ae-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```
# <a name="c"></a>[<span data-ttu-id="838ae-144">C#</span><span class="sxs-lookup"><span data-stu-id="838ae-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-unsubscribe-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="838ae-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="838ae-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-unsubscribe-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="838ae-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="838ae-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-unsubscribe-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="838ae-147">Java</span><span class="sxs-lookup"><span data-stu-id="838ae-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-unsubscribe-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="838ae-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="838ae-148">Response</span></span>
<span data-ttu-id="838ae-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="838ae-149">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: unsubscribe",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


