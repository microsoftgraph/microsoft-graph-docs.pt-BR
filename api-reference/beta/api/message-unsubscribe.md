---
title: 'mensagem: cancelar assinatura'
description: Envia uma solicitação de e-mail em nome do usuário conectado para cancelar a assinatura de uma lista de distribuição de e-mail. Usa as informações do cabeçalho `List-Unsubscribe`.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e3f3378f813bce61f5ecef5b6003fb10fc680d59
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456863"
---
# <a name="message-unsubscribe"></a><span data-ttu-id="ff4a6-104">mensagem: cancelar assinatura</span><span class="sxs-lookup"><span data-stu-id="ff4a6-104">message: unsubscribe</span></span>

<span data-ttu-id="ff4a6-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ff4a6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff4a6-106">Envia uma solicitação de e-mail em nome do usuário conectado para cancelar a assinatura de uma lista de distribuição de e-mail.</span><span class="sxs-lookup"><span data-stu-id="ff4a6-106">Submits a email request on behalf of the signed-in user to unsubscribe from an email distribution list.</span></span> <span data-ttu-id="ff4a6-107">Usa as informações do cabeçalho `List-Unsubscribe`.</span><span class="sxs-lookup"><span data-stu-id="ff4a6-107">Uses the information in the `List-Unsubscribe` header.</span></span>

<span data-ttu-id="ff4a6-108">Os remetentes de mensagens podem usar listas de mala direta de forma amigável, incluindo uma opção para que os destinatários recusem. Eles podem fazer isso especificando o `List-Unsubscribe` cabeçalho em cada mensagem após [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span><span class="sxs-lookup"><span data-stu-id="ff4a6-108">Message senders can use mailing lists in a user-friendly way by including an option for recipients to opt out. They can do so by specifying the `List-Unsubscribe` header in each message following [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span></span>

<span data-ttu-id="ff4a6-109">**Observação** Em particular, para que a ação de **cancelamento de assinatura** funcione, `mailto:` o remetente deve especificar e não informações de cancelamento de assinatura baseadas em URL.</span><span class="sxs-lookup"><span data-stu-id="ff4a6-109">**Note** In particular, for the **unsubscribe** action to work, the sender must specify `mailto:` and not URL-based unsubscribe information.</span></span>

<span data-ttu-id="ff4a6-110">Definir esse cabeçalho também definiria a propriedade **unsubscribeEnabled** da instância da [mensagem](../resources/message.md) como `true`e a propriedade **unsubscribeData** para os dados do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="ff4a6-110">Setting that header would also set the **unsubscribeEnabled** property of the [message](../resources/message.md) instance to `true`, and the **unsubscribeData** property to the header data.</span></span>

<span data-ttu-id="ff4a6-111">Se a propriedade **unsubscribeEnabled** de uma mensagem for `true`, você poderá usar a ação **cancelar assinatura** para cancelar a inscrição do usuário de mensagens semelhantes futuras, conforme gerenciado pelo remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="ff4a6-111">If the **unsubscribeEnabled** property of a message is `true`, you can use the **unsubscribe** action to unsubscribe the user from similar future messages as managed by the message sender.</span></span>

<span data-ttu-id="ff4a6-112">Uma ação de **cancelamento de assinatura** bem-sucedida move a mensagem para a pasta **itens excluídos** .</span><span class="sxs-lookup"><span data-stu-id="ff4a6-112">A successful **unsubscribe** action moves the message to the **Deleted Items** folder.</span></span> <span data-ttu-id="ff4a6-113">A exclusão do usuário dos destinatários de futuros e-mails é gerenciada pelo remetente.</span><span class="sxs-lookup"><span data-stu-id="ff4a6-113">The actual exclusion of the user from future mail distribution is managed by the sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff4a6-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff4a6-114">Permissions</span></span>
<span data-ttu-id="ff4a6-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff4a6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff4a6-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff4a6-117">Permission type</span></span>      | <span data-ttu-id="ff4a6-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff4a6-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff4a6-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff4a6-119">Delegated (work or school account)</span></span> | <span data-ttu-id="ff4a6-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ff4a6-120">Mail.Send</span></span>    |
|<span data-ttu-id="ff4a6-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff4a6-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff4a6-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ff4a6-122">Mail.Send</span></span>    |
|<span data-ttu-id="ff4a6-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff4a6-123">Application</span></span> | <span data-ttu-id="ff4a6-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ff4a6-124">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff4a6-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff4a6-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a><span data-ttu-id="ff4a6-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff4a6-126">Request headers</span></span>
| <span data-ttu-id="ff4a6-127">Nome</span><span class="sxs-lookup"><span data-stu-id="ff4a6-127">Name</span></span>       | <span data-ttu-id="ff4a6-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff4a6-128">Type</span></span> | <span data-ttu-id="ff4a6-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff4a6-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ff4a6-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff4a6-130">Authorization</span></span>  | <span data-ttu-id="ff4a6-131">string</span><span class="sxs-lookup"><span data-stu-id="ff4a6-131">string</span></span>  | <span data-ttu-id="ff4a6-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff4a6-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff4a6-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff4a6-134">Request body</span></span>
<span data-ttu-id="ff4a6-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff4a6-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff4a6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff4a6-136">Response</span></span>

<span data-ttu-id="ff4a6-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff4a6-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff4a6-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff4a6-139">Example</span></span>
<span data-ttu-id="ff4a6-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ff4a6-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ff4a6-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff4a6-141">Request</span></span>
<span data-ttu-id="ff4a6-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff4a6-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ff4a6-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff4a6-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```
# <a name="c"></a>[<span data-ttu-id="ff4a6-144">C#</span><span class="sxs-lookup"><span data-stu-id="ff4a6-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-unsubscribe-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff4a6-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff4a6-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-unsubscribe-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff4a6-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff4a6-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-unsubscribe-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ff4a6-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff4a6-147">Response</span></span>
<span data-ttu-id="ff4a6-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff4a6-148">Here is an example of the response.</span></span> 
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
