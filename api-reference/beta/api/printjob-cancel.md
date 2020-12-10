---
title: 'printJob: cancelar'
description: Cancelar um trabalho de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 4c4522ef8fb19226475758986d1245c447358095
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617014"
---
# <a name="printjob-cancel"></a><span data-ttu-id="eac3f-103">printJob: cancelar</span><span class="sxs-lookup"><span data-stu-id="eac3f-103">printJob: cancel</span></span>

<span data-ttu-id="eac3f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eac3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eac3f-105">Cancelar um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="eac3f-105">Cancel a print job.</span></span> <span data-ttu-id="eac3f-106">Os trabalhos de impressão podem ser cancelados somente em nome de um usuário, usando permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="eac3f-106">Print jobs can be canceled only on behalf of a user, using delegated permissions.</span></span>

## <a name="permissions"></a><span data-ttu-id="eac3f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="eac3f-107">Permissions</span></span>
<span data-ttu-id="eac3f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eac3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="eac3f-110">Além das permissões a seguir, o locatário do usuário ou do aplicativo deve ter uma assinatura universal de impressão ativa e ter uma permissão que conceda obter acesso à [impressora](printer-get.md) .</span><span class="sxs-lookup"><span data-stu-id="eac3f-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="eac3f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eac3f-111">Permission type</span></span> | <span data-ttu-id="eac3f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eac3f-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="eac3f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eac3f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="eac3f-114">PrintJob. ReadWriteBasic, PrintJob. ReadWrite, PrintJob. ReadWriteBasic. All, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="eac3f-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="eac3f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eac3f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eac3f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eac3f-116">Not Supported.</span></span>|
|<span data-ttu-id="eac3f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eac3f-117">Application</span></span>| <span data-ttu-id="eac3f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eac3f-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eac3f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eac3f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/cancel
```
## <a name="request-headers"></a><span data-ttu-id="eac3f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eac3f-120">Request headers</span></span>
| <span data-ttu-id="eac3f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="eac3f-121">Name</span></span>          | <span data-ttu-id="eac3f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="eac3f-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="eac3f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="eac3f-123">Authorization</span></span> | <span data-ttu-id="eac3f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eac3f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eac3f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eac3f-126">Request body</span></span>
<span data-ttu-id="eac3f-127">O corpo da solicitação deve estar vazio.</span><span class="sxs-lookup"><span data-stu-id="eac3f-127">Request body should be empty.</span></span>

## <a name="response"></a><span data-ttu-id="eac3f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="eac3f-128">Response</span></span>
<span data-ttu-id="eac3f-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eac3f-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eac3f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eac3f-131">Example</span></span>
<span data-ttu-id="eac3f-132">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="eac3f-132">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="eac3f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eac3f-133">Request</span></span>
<span data-ttu-id="eac3f-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eac3f-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="eac3f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="eac3f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-cancel"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/cancel
```
# <a name="c"></a>[<span data-ttu-id="eac3f-136">C#</span><span class="sxs-lookup"><span data-stu-id="eac3f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eac3f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eac3f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eac3f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eac3f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eac3f-139">Java</span><span class="sxs-lookup"><span data-stu-id="eac3f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eac3f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="eac3f-140">Response</span></span>
<span data-ttu-id="eac3f-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eac3f-141">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
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


