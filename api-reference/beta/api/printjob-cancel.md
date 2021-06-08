---
title: 'printJob: cancel'
description: Cancele um trabalho de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: b2eb7c40f1f2474752b316a412dbb4c382152741
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787510"
---
# <a name="printjob-cancel"></a><span data-ttu-id="8009d-103">printJob: cancel</span><span class="sxs-lookup"><span data-stu-id="8009d-103">printJob: cancel</span></span>

<span data-ttu-id="8009d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8009d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8009d-105">Cancele um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="8009d-105">Cancel a print job.</span></span> <span data-ttu-id="8009d-106">Trabalhos de impressão só podem ser cancelados em nome de um usuário, usando permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="8009d-106">Print jobs can be canceled only on behalf of a user, using delegated permissions.</span></span>

## <a name="permissions"></a><span data-ttu-id="8009d-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="8009d-107">Permissions</span></span>
<span data-ttu-id="8009d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8009d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8009d-110">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda [acesso à](printer-get.md) impressora.</span><span class="sxs-lookup"><span data-stu-id="8009d-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="8009d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8009d-111">Permission type</span></span> | <span data-ttu-id="8009d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8009d-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8009d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8009d-113">Delegated (work or school account)</span></span>| <span data-ttu-id="8009d-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8009d-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="8009d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8009d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8009d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8009d-116">Not Supported.</span></span>|
|<span data-ttu-id="8009d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8009d-117">Application</span></span>| <span data-ttu-id="8009d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8009d-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8009d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8009d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/cancel
```
## <a name="request-headers"></a><span data-ttu-id="8009d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8009d-120">Request headers</span></span>
| <span data-ttu-id="8009d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8009d-121">Name</span></span>          | <span data-ttu-id="8009d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8009d-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8009d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8009d-123">Authorization</span></span> | <span data-ttu-id="8009d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8009d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8009d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8009d-126">Request body</span></span>
<span data-ttu-id="8009d-127">O corpo da solicitação deve estar vazio.</span><span class="sxs-lookup"><span data-stu-id="8009d-127">Request body should be empty.</span></span>

## <a name="response"></a><span data-ttu-id="8009d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8009d-128">Response</span></span>
<span data-ttu-id="8009d-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8009d-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8009d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8009d-131">Example</span></span>
<span data-ttu-id="8009d-132">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8009d-132">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="8009d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8009d-133">Request</span></span>
<span data-ttu-id="8009d-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8009d-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8009d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8009d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-cancel"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/cancel
```
# <a name="c"></a>[<span data-ttu-id="8009d-136">C#</span><span class="sxs-lookup"><span data-stu-id="8009d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8009d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8009d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8009d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8009d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8009d-139">Java</span><span class="sxs-lookup"><span data-stu-id="8009d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8009d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8009d-140">Response</span></span>
<span data-ttu-id="8009d-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8009d-141">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


