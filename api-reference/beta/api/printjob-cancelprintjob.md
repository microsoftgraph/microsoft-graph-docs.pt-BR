---
title: 'printJob: cancelPrintJob'
description: Cancelar um trabalho de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 311236ed0c34064291db93731c5ad8bb62c242a3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035461"
---
# <a name="printjob-cancelprintjob"></a><span data-ttu-id="36209-103">printJob: cancelPrintJob</span><span class="sxs-lookup"><span data-stu-id="36209-103">printJob: cancelPrintJob</span></span>

<span data-ttu-id="36209-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36209-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36209-105">Cancelar um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="36209-105">Cancel a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="36209-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="36209-106">Permissions</span></span>
<span data-ttu-id="36209-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36209-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="36209-109">Além das permissões a seguir, o locatário do usuário ou do aplicativo deve ter uma assinatura universal de impressão ativa e ter uma permissão que conceda obter acesso à [impressora](printer-get.md) .</span><span class="sxs-lookup"><span data-stu-id="36209-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="36209-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36209-110">Permission type</span></span> | <span data-ttu-id="36209-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36209-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="36209-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36209-112">Delegated (work or school account)</span></span>| <span data-ttu-id="36209-113">PrintJob. ReadWriteBasic, PrintJob. ReadWrite, PrintJob. ReadWriteBasic. All, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="36209-113">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="36209-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36209-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36209-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36209-115">Not Supported.</span></span>|
|<span data-ttu-id="36209-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36209-116">Application</span></span>| <span data-ttu-id="36209-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36209-117">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36209-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36209-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/cancelPrintJob
```
## <a name="request-headers"></a><span data-ttu-id="36209-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36209-119">Request headers</span></span>
| <span data-ttu-id="36209-120">Nome</span><span class="sxs-lookup"><span data-stu-id="36209-120">Name</span></span>          | <span data-ttu-id="36209-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="36209-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="36209-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="36209-122">Authorization</span></span> | <span data-ttu-id="36209-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36209-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36209-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36209-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="36209-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="36209-126">Response</span></span>
<span data-ttu-id="36209-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36209-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36209-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36209-129">Example</span></span>
<span data-ttu-id="36209-130">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="36209-130">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="36209-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36209-131">Request</span></span>
<span data-ttu-id="36209-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="36209-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="36209-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="36209-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-cancelprintjob"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/cancelPrintJob
```
# <a name="c"></a>[<span data-ttu-id="36209-134">C#</span><span class="sxs-lookup"><span data-stu-id="36209-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-cancelprintjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36209-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36209-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-cancelprintjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36209-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36209-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-cancelprintjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="36209-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="36209-137">Response</span></span>
<span data-ttu-id="36209-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="36209-138">The following is an example of the response.</span></span> 
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
  "description": "printJob: cancelPrintJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


