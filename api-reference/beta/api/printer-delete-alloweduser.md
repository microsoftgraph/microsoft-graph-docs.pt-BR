---
title: Excluir allowedUser
description: Revogar o acesso do usuário especificado para enviar trabalhos de impressão à impressora associada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 790a4db92d2ad4f90839508f0dc15c83599422c9
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948055"
---
# <a name="delete-alloweduser"></a><span data-ttu-id="55171-103">Excluir allowedUser</span><span class="sxs-lookup"><span data-stu-id="55171-103">Delete allowedUser</span></span>

<span data-ttu-id="55171-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55171-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55171-105">Revogar o acesso do usuário especificado para enviar trabalhos de impressão à [impressora](../resources/printer.md)associada.</span><span class="sxs-lookup"><span data-stu-id="55171-105">Revoke the specified user's access to submit print jobs to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="55171-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="55171-106">Permissions</span></span>
<span data-ttu-id="55171-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55171-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="55171-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="55171-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="55171-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55171-110">Permission type</span></span> | <span data-ttu-id="55171-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55171-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="55171-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55171-112">Delegated (work or school account)</span></span>| <span data-ttu-id="55171-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="55171-113">Users.Read.All</span></span> |
|<span data-ttu-id="55171-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55171-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55171-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55171-115">Not Supported.</span></span>|
|<span data-ttu-id="55171-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55171-116">Application</span></span>|<span data-ttu-id="55171-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55171-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55171-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55171-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printers/{id}/allowedUsers/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="55171-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55171-119">Request headers</span></span>
| <span data-ttu-id="55171-120">Nome</span><span class="sxs-lookup"><span data-stu-id="55171-120">Name</span></span>          | <span data-ttu-id="55171-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="55171-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="55171-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="55171-122">Authorization</span></span> | <span data-ttu-id="55171-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55171-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55171-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55171-125">Request body</span></span>
<span data-ttu-id="55171-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55171-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55171-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="55171-127">Response</span></span>
<span data-ttu-id="55171-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55171-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55171-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55171-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55171-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55171-131">Request</span></span>
<span data-ttu-id="55171-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55171-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55171-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="55171-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_alloweduser"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printers/{id}/allowedUsers/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="55171-134">C#</span><span class="sxs-lookup"><span data-stu-id="55171-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-alloweduser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55171-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55171-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-alloweduser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55171-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55171-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-alloweduser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="55171-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="55171-137">Response</span></span>
<span data-ttu-id="55171-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55171-138">The following is an example of the response.</span></span>
><span data-ttu-id="55171-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55171-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete allowedUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
