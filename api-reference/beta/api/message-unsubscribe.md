---
title: 'mensagem: cancelar assinatura'
description: Envia uma solicitação de e-mail em nome do usuário conectado para cancelar a assinatura de uma lista de distribuição de e-mail. Usa as informações do cabeçalho `List-Unsubscribe`.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0055621687e6ea3e991b3ee21f2bda10a95a76b3
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33597709"
---
# <a name="message-unsubscribe"></a><span data-ttu-id="25a77-104">mensagem: cancelar assinatura</span><span class="sxs-lookup"><span data-stu-id="25a77-104">message: unsubscribe</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25a77-105">Envia uma solicitação de e-mail em nome do usuário conectado para cancelar a assinatura de uma lista de distribuição de e-mail.</span><span class="sxs-lookup"><span data-stu-id="25a77-105">Submits a email request on behalf of the signed-in user to unsubscribe from an email distribution list.</span></span> <span data-ttu-id="25a77-106">Usa as informações do cabeçalho `List-Unsubscribe`.</span><span class="sxs-lookup"><span data-stu-id="25a77-106">Uses the information in the `List-Unsubscribe` header.</span></span>

<span data-ttu-id="25a77-107">Os remetentes de mensagens podem usar listas de mala direta de forma amigável, incluindo uma opção para que os destinatários recusem. Eles podem fazer isso especificando o `List-Unsubscribe` cabeçalho em cada mensagem após [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span><span class="sxs-lookup"><span data-stu-id="25a77-107">Message senders can use mailing lists in a user-friendly way by including an option for recipients to opt out. They can do so by specifying the `List-Unsubscribe` header in each message following [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span></span>

<span data-ttu-id="25a77-108">**Observação** Em particular, para que a ação de cancelamento de **assinatura** funcione, `mailto:` o remetente deve especificar e não informações de cancelamento de assinatura baseadas em URL.</span><span class="sxs-lookup"><span data-stu-id="25a77-108">**Note** In particular, for the **unsubscribe** action to work, the sender must specify `mailto:` and not URL-based unsubscribe information.</span></span>

<span data-ttu-id="25a77-109">Definir esse cabeçalho também definiria a propriedade **unsubscribeEnabled** da instância da [mensagem](../resources/message.md) como `true`e a propriedade **unsubscribeData** para os dados do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="25a77-109">Setting that header would also set the **unsubscribeEnabled** property of the [message](../resources/message.md) instance to `true`, and the **unsubscribeData** property to the header data.</span></span>

<span data-ttu-id="25a77-110">Se a propriedade **unsubscribeEnabled** de uma mensagem for `true`, você poderá usar a ação **cancelar assinatura** para cancelar a inscrição do usuário de mensagens semelhantes futuras, conforme gerenciado pelo remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="25a77-110">If the **unsubscribeEnabled** property of a message is `true`, you can use the **unsubscribe** action to unsubscribe the user from similar future messages as managed by the message sender.</span></span>

<span data-ttu-id="25a77-111">Uma ação de cancelamento de **assinatura** bem-sucedida move a mensagem para a pasta **itens excluídos** .</span><span class="sxs-lookup"><span data-stu-id="25a77-111">A successful **unsubscribe** action moves the message to the **Deleted Items** folder.</span></span> <span data-ttu-id="25a77-112">A exclusão do usuário dos destinatários de futuros e-mails é gerenciada pelo remetente.</span><span class="sxs-lookup"><span data-stu-id="25a77-112">The actual exclusion of the user from future mail distribution is managed by the sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="25a77-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="25a77-113">Permissions</span></span>
<span data-ttu-id="25a77-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25a77-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25a77-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25a77-116">Permission type</span></span>      | <span data-ttu-id="25a77-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25a77-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25a77-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25a77-118">Delegated (work or school account)</span></span> | <span data-ttu-id="25a77-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="25a77-119">Mail.Send</span></span>    |
|<span data-ttu-id="25a77-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25a77-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25a77-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="25a77-121">Mail.Send</span></span>    |
|<span data-ttu-id="25a77-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25a77-122">Application</span></span> | <span data-ttu-id="25a77-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="25a77-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="25a77-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25a77-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a><span data-ttu-id="25a77-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25a77-125">Request headers</span></span>
| <span data-ttu-id="25a77-126">Nome</span><span class="sxs-lookup"><span data-stu-id="25a77-126">Name</span></span>       | <span data-ttu-id="25a77-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="25a77-127">Type</span></span> | <span data-ttu-id="25a77-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="25a77-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="25a77-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="25a77-129">Authorization</span></span>  | <span data-ttu-id="25a77-130">string</span><span class="sxs-lookup"><span data-stu-id="25a77-130">string</span></span>  | <span data-ttu-id="25a77-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25a77-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25a77-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25a77-133">Request body</span></span>
<span data-ttu-id="25a77-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25a77-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25a77-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="25a77-135">Response</span></span>

<span data-ttu-id="25a77-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25a77-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25a77-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25a77-138">Example</span></span>
<span data-ttu-id="25a77-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="25a77-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="25a77-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25a77-140">Request</span></span>
<span data-ttu-id="25a77-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25a77-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```

##### <a name="response"></a><span data-ttu-id="25a77-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="25a77-142">Response</span></span>
<span data-ttu-id="25a77-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25a77-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="25a77-144">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="25a77-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="25a77-145">Basic</span><span class="sxs-lookup"><span data-stu-id="25a77-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_unsubscribe-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="25a77-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25a77-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_unsubscribe-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/message-unsubscribe.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-unsubscribe.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
