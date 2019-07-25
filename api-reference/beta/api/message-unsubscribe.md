---
title: 'mensagem: cancelar assinatura'
description: Envia uma solicitação de e-mail em nome do usuário conectado para cancelar a assinatura de uma lista de distribuição de e-mail. Usa as informações do cabeçalho `List-Unsubscribe`.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 87cfe7616319f52561bec46d711770081bf1a32e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879379"
---
# <a name="message-unsubscribe"></a><span data-ttu-id="4c7f7-104">mensagem: cancelar assinatura</span><span class="sxs-lookup"><span data-stu-id="4c7f7-104">message: unsubscribe</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c7f7-105">Envia uma solicitação de e-mail em nome do usuário conectado para cancelar a assinatura de uma lista de distribuição de e-mail.</span><span class="sxs-lookup"><span data-stu-id="4c7f7-105">Submits a email request on behalf of the signed-in user to unsubscribe from an email distribution list.</span></span> <span data-ttu-id="4c7f7-106">Usa as informações do cabeçalho `List-Unsubscribe`.</span><span class="sxs-lookup"><span data-stu-id="4c7f7-106">Uses the information in the `List-Unsubscribe` header.</span></span>

<span data-ttu-id="4c7f7-107">Os remetentes de mensagens podem usar listas de mala direta de forma amigável, incluindo uma opção para que os destinatários recusem. Eles podem fazer isso especificando o `List-Unsubscribe` cabeçalho em cada mensagem após [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span><span class="sxs-lookup"><span data-stu-id="4c7f7-107">Message senders can use mailing lists in a user-friendly way by including an option for recipients to opt out. They can do so by specifying the `List-Unsubscribe` header in each message following [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span></span>

<span data-ttu-id="4c7f7-108">**Observação** Em particular, para que a ação de cancelamento de **assinatura** funcione, `mailto:` o remetente deve especificar e não informações de cancelamento de assinatura baseadas em URL.</span><span class="sxs-lookup"><span data-stu-id="4c7f7-108">**Note** In particular, for the **unsubscribe** action to work, the sender must specify `mailto:` and not URL-based unsubscribe information.</span></span>

<span data-ttu-id="4c7f7-109">Definir esse cabeçalho também definiria a propriedade **unsubscribeEnabled** da instância da [mensagem](../resources/message.md) como `true`e a propriedade **unsubscribeData** para os dados do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="4c7f7-109">Setting that header would also set the **unsubscribeEnabled** property of the [message](../resources/message.md) instance to `true`, and the **unsubscribeData** property to the header data.</span></span>

<span data-ttu-id="4c7f7-110">Se a propriedade **unsubscribeEnabled** de uma mensagem for `true`, você poderá usar a ação **cancelar assinatura** para cancelar a inscrição do usuário de mensagens semelhantes futuras, conforme gerenciado pelo remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="4c7f7-110">If the **unsubscribeEnabled** property of a message is `true`, you can use the **unsubscribe** action to unsubscribe the user from similar future messages as managed by the message sender.</span></span>

<span data-ttu-id="4c7f7-111">Uma ação de cancelamento de **assinatura** bem-sucedida move a mensagem para a pasta **itens excluídos** .</span><span class="sxs-lookup"><span data-stu-id="4c7f7-111">A successful **unsubscribe** action moves the message to the **Deleted Items** folder.</span></span> <span data-ttu-id="4c7f7-112">A exclusão do usuário dos destinatários de futuros e-mails é gerenciada pelo remetente.</span><span class="sxs-lookup"><span data-stu-id="4c7f7-112">The actual exclusion of the user from future mail distribution is managed by the sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c7f7-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c7f7-113">Permissions</span></span>
<span data-ttu-id="4c7f7-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c7f7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c7f7-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c7f7-116">Permission type</span></span>      | <span data-ttu-id="4c7f7-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c7f7-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c7f7-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c7f7-118">Delegated (work or school account)</span></span> | <span data-ttu-id="4c7f7-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="4c7f7-119">Mail.Send</span></span>    |
|<span data-ttu-id="4c7f7-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c7f7-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c7f7-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="4c7f7-121">Mail.Send</span></span>    |
|<span data-ttu-id="4c7f7-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c7f7-122">Application</span></span> | <span data-ttu-id="4c7f7-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="4c7f7-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c7f7-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c7f7-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a><span data-ttu-id="4c7f7-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c7f7-125">Request headers</span></span>
| <span data-ttu-id="4c7f7-126">Nome</span><span class="sxs-lookup"><span data-stu-id="4c7f7-126">Name</span></span>       | <span data-ttu-id="4c7f7-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c7f7-127">Type</span></span> | <span data-ttu-id="4c7f7-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c7f7-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4c7f7-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c7f7-129">Authorization</span></span>  | <span data-ttu-id="4c7f7-130">string</span><span class="sxs-lookup"><span data-stu-id="4c7f7-130">string</span></span>  | <span data-ttu-id="4c7f7-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c7f7-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c7f7-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c7f7-133">Request body</span></span>
<span data-ttu-id="4c7f7-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4c7f7-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c7f7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c7f7-135">Response</span></span>

<span data-ttu-id="4c7f7-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c7f7-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c7f7-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c7f7-138">Example</span></span>
<span data-ttu-id="4c7f7-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4c7f7-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4c7f7-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c7f7-140">Request</span></span>
<span data-ttu-id="4c7f7-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c7f7-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4c7f7-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c7f7-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4c7f7-143">C#</span><span class="sxs-lookup"><span data-stu-id="4c7f7-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-unsubscribe-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c7f7-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="4c7f7-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-unsubscribe-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4c7f7-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4c7f7-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-unsubscribe-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4c7f7-146">Java</span><span class="sxs-lookup"><span data-stu-id="4c7f7-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-unsubscribe-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4c7f7-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c7f7-147">Response</span></span>
<span data-ttu-id="4c7f7-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c7f7-148">Here is an example of the response.</span></span> 
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
