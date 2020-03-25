---
title: Excluir printerShare
description: Excluir um compartilhamento de impressora (descompartilhar a impressora associada). Não é possível desfazer a ação. Se a impressora for compartilhada novamente no futuro, qualquer usuário do Windows que tenha instalado anteriormente a impressora deverá descobrir e reinstalá-la.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 78d81fe559d40f6d1244c4ea1c281d48a4337cde
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947690"
---
# <a name="delete-printershare"></a><span data-ttu-id="37e5d-105">Excluir printerShare</span><span class="sxs-lookup"><span data-stu-id="37e5d-105">Delete printerShare</span></span>

<span data-ttu-id="37e5d-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37e5d-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37e5d-107">Excluir um compartilhamento de impressora (descompartilhar a [impressora](../resources/printer.md)associada).</span><span class="sxs-lookup"><span data-stu-id="37e5d-107">Delete a printer share (unshare the associated [printer](../resources/printer.md)).</span></span> <span data-ttu-id="37e5d-108">Não é possível desfazer a ação.</span><span class="sxs-lookup"><span data-stu-id="37e5d-108">This action cannot be undone.</span></span> <span data-ttu-id="37e5d-109">Se a [impressora](../resources/printer.md) for compartilhada novamente no futuro, qualquer usuário do Windows que tenha instalado anteriormente a [impressora](../resources/printer.md) deverá descobrir e reinstalá-la.</span><span class="sxs-lookup"><span data-stu-id="37e5d-109">If the [printer](../resources/printer.md) is shared again in the future, any Windows users who had previously installed the [printer](../resources/printer.md) will need to discover and reinstall it.</span></span>

## <a name="permissions"></a><span data-ttu-id="37e5d-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="37e5d-110">Permissions</span></span>
<span data-ttu-id="37e5d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37e5d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="37e5d-113">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="37e5d-113">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="37e5d-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37e5d-114">Permission type</span></span> | <span data-ttu-id="37e5d-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37e5d-115">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="37e5d-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37e5d-116">Delegated (work or school account)</span></span>| <span data-ttu-id="37e5d-117">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="37e5d-117">Users.Read.All</span></span> |
|<span data-ttu-id="37e5d-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37e5d-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37e5d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37e5d-119">Not Supported.</span></span>|
|<span data-ttu-id="37e5d-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37e5d-120">Application</span></span>|<span data-ttu-id="37e5d-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37e5d-121">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37e5d-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37e5d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printerShares/{id}
DELETE /print/printers/{id}/share
```
## <a name="request-headers"></a><span data-ttu-id="37e5d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37e5d-123">Request headers</span></span>
| <span data-ttu-id="37e5d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="37e5d-124">Name</span></span>          | <span data-ttu-id="37e5d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="37e5d-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="37e5d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="37e5d-126">Authorization</span></span> | <span data-ttu-id="37e5d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37e5d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37e5d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37e5d-129">Request body</span></span>
<span data-ttu-id="37e5d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37e5d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37e5d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="37e5d-131">Response</span></span>
<span data-ttu-id="37e5d-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37e5d-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37e5d-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37e5d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37e5d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37e5d-135">Request</span></span>
<span data-ttu-id="37e5d-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="37e5d-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37e5d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="37e5d-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printershare"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printerShares/{id}
```
# <a name="c"></a>[<span data-ttu-id="37e5d-138">C#</span><span class="sxs-lookup"><span data-stu-id="37e5d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37e5d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37e5d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37e5d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37e5d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="37e5d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="37e5d-141">Response</span></span>
<span data-ttu-id="37e5d-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="37e5d-142">The following is an example of the response.</span></span>
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
  "description": "Delete printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
