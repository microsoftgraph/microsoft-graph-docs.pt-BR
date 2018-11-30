---
title: 'mensagem: Cancelar a assinatura'
description: Envia uma solicitação de e-mail em nome do usuário conectado para cancelar a assinatura de uma lista de distribuição de e-mail. Usa as informações do cabeçalho `List-Unsubscribe`.
ms.openlocfilehash: b4f72a0b629fb59074acbbd58f09a3c16118cc8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037365"
---
# <a name="message-unsubscribe"></a><span data-ttu-id="c9898-104">mensagem: Cancelar a assinatura</span><span class="sxs-lookup"><span data-stu-id="c9898-104">message: unsubscribe</span></span>

> <span data-ttu-id="c9898-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c9898-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9898-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c9898-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9898-107">Envia uma solicitação de e-mail em nome do usuário conectado para cancelar a assinatura de uma lista de distribuição de e-mail.</span><span class="sxs-lookup"><span data-stu-id="c9898-107">Submits a email request on behalf of the signed-in user to unsubscribe from an email distribution list.</span></span> <span data-ttu-id="c9898-108">Usa as informações do cabeçalho `List-Unsubscribe`.</span><span class="sxs-lookup"><span data-stu-id="c9898-108">Uses the information in the `List-Unsubscribe` header.</span></span>

<span data-ttu-id="c9898-109">Remetentes de mensagens podem usar listas de endereçamento de forma amigável, incluindo uma opção para destinatários para rejeitar. Eles podem fazer isso, especificando o `List-Unsubscribe` cabeçalho em cada mensagem seguindo [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span><span class="sxs-lookup"><span data-stu-id="c9898-109">Message senders can use mailing lists in a user-friendly way by including an option for recipients to opt out. They can do so by specifying the `List-Unsubscribe` header in each message following [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span></span>

<span data-ttu-id="c9898-110">**Observação** Em particular, para a ação **Cancelar** funcione, o remetente deve especificar `mailto:` e não baseado em URL cancelar a assinatura de informações.</span><span class="sxs-lookup"><span data-stu-id="c9898-110">**Note** In particular, for the **unsubscribe** action to work, the sender must specify `mailto:` and not URL-based unsubscribe information.</span></span>

<span data-ttu-id="c9898-111">A definição desse cabeçalho seria também definir a propriedade de **unsubscribeEnabled** da instância da [mensagem](../resources/message.md) para `true`e a propriedade **unsubscribeData** para os dados de cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="c9898-111">Setting that header would also set the **unsubscribeEnabled** property of the [message](../resources/message.md) instance to `true`, and the **unsubscribeData** property to the header data.</span></span>

<span data-ttu-id="c9898-112">Se a propriedade **unsubscribeEnabled** de uma mensagem é `true`, você pode usar a ação **Cancelar** para cancelar o usuário de mensagens futuras semelhantes como gerenciado pelo remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c9898-112">If the **unsubscribeEnabled** property of a message is `true`, you can use the **unsubscribe** action to unsubscribe the user from similar future messages as managed by the message sender.</span></span>

<span data-ttu-id="c9898-113">Uma ação bem-sucedida **Cancelar** move a mensagem para a pasta **Itens excluídos** .</span><span class="sxs-lookup"><span data-stu-id="c9898-113">A successful **unsubscribe** action moves the message to the **Deleted Items** folder.</span></span> <span data-ttu-id="c9898-114">A exclusão do usuário dos destinatários de futuros e-mails é gerenciada pelo remetente.</span><span class="sxs-lookup"><span data-stu-id="c9898-114">The actual exclusion of the user from future mail distribution is managed by the sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9898-115">Permissions</span><span class="sxs-lookup"><span data-stu-id="c9898-115">Permissions</span></span>
<span data-ttu-id="c9898-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9898-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9898-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9898-118">Permission type</span></span>      | <span data-ttu-id="c9898-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9898-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9898-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9898-120">Delegated (work or school account)</span></span> | <span data-ttu-id="c9898-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c9898-121">Mail.Send</span></span>    |
|<span data-ttu-id="c9898-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9898-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9898-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c9898-123">Mail.Send</span></span>    |
|<span data-ttu-id="c9898-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9898-124">Application</span></span> | <span data-ttu-id="c9898-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c9898-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9898-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9898-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a><span data-ttu-id="c9898-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9898-127">Request headers</span></span>
| <span data-ttu-id="c9898-128">Nome</span><span class="sxs-lookup"><span data-stu-id="c9898-128">Name</span></span>       | <span data-ttu-id="c9898-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9898-129">Type</span></span> | <span data-ttu-id="c9898-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9898-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c9898-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9898-131">Authorization</span></span>  | <span data-ttu-id="c9898-132">string</span><span class="sxs-lookup"><span data-stu-id="c9898-132">string</span></span>  | <span data-ttu-id="c9898-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9898-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9898-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9898-135">Request body</span></span>
<span data-ttu-id="c9898-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c9898-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9898-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9898-137">Response</span></span>

<span data-ttu-id="c9898-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9898-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9898-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9898-140">Example</span></span>
<span data-ttu-id="c9898-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c9898-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c9898-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9898-142">Request</span></span>
<span data-ttu-id="c9898-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9898-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```

##### <a name="response"></a><span data-ttu-id="c9898-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9898-144">Response</span></span>
<span data-ttu-id="c9898-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9898-145">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: unsubscribe",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
