---
title: 'printJob: Redirect'
description: Redirecionar um trabalho de impressão para uma impressora diferente.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a498f85238127a6816ed5d6597839862cd00f58d
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319456"
---
# <a name="printjob-redirect"></a><span data-ttu-id="13927-103">printJob: Redirect</span><span class="sxs-lookup"><span data-stu-id="13927-103">printJob: redirect</span></span>

<span data-ttu-id="13927-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13927-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13927-105">Redirecionar um [trabalho de impressão](../resources/printjob.md) para uma [impressora](../resources/printer.md)diferente.</span><span class="sxs-lookup"><span data-stu-id="13927-105">Redirect a [print job](../resources/printjob.md) to a different [printer](../resources/printer.md).</span></span>

<span data-ttu-id="13927-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à impressão universal, consulte [Estendeing universal print to support pull Printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="13927-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="13927-107">Os trabalhos de impressão pausados que não são redirecionados em 2 dias serão excluídos.</span><span class="sxs-lookup"><span data-stu-id="13927-107">Paused print jobs that are not redirected within 2 days will be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="13927-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="13927-108">Permissions</span></span>
<span data-ttu-id="13927-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13927-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="13927-111">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura universal de impressão ativa, uma permissão que conceda obter acesso à [impressora](printer-get.md) e uma das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="13927-111">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="13927-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13927-112">Permission type</span></span> | <span data-ttu-id="13927-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13927-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="13927-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13927-114">Delegated (work or school account)</span></span>| <span data-ttu-id="13927-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13927-115">Not supported.</span></span> |
|<span data-ttu-id="13927-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13927-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13927-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13927-117">Not Supported.</span></span>|
|<span data-ttu-id="13927-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13927-118">Application</span></span>| <span data-ttu-id="13927-119">PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="13927-119">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13927-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13927-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/redirect
```
## <a name="request-headers"></a><span data-ttu-id="13927-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13927-121">Request headers</span></span>
| <span data-ttu-id="13927-122">Nome</span><span class="sxs-lookup"><span data-stu-id="13927-122">Name</span></span>          | <span data-ttu-id="13927-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="13927-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="13927-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="13927-124">Authorization</span></span> | <span data-ttu-id="13927-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13927-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13927-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13927-127">Request body</span></span>
<span data-ttu-id="13927-128">No corpo da solicitação, forneça a ID da impressora para a qual o trabalho de impressão deve ser redirecionado.</span><span class="sxs-lookup"><span data-stu-id="13927-128">In the request body, supply the ID of the printer that the print job should be redirected to.</span></span>

| <span data-ttu-id="13927-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13927-129">Property</span></span>     | <span data-ttu-id="13927-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="13927-130">Type</span></span>        | <span data-ttu-id="13927-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="13927-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="13927-132">destinationPrinterId</span><span class="sxs-lookup"><span data-stu-id="13927-132">destinationPrinterId</span></span>|<span data-ttu-id="13927-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13927-133">String</span></span>|<span data-ttu-id="13927-134">A ID da impressora para a qual o trabalho de impressão deve ser redirecionado.</span><span class="sxs-lookup"><span data-stu-id="13927-134">The ID of the printer the print job should be redirected to.</span></span>|

## <a name="response"></a><span data-ttu-id="13927-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="13927-135">Response</span></span>
<span data-ttu-id="13927-136">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [printJob](../resources/printjob.md) enfileirados para a impressora de destino.</span><span class="sxs-lookup"><span data-stu-id="13927-136">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object queued for the destination printer.</span></span>

## <a name="example"></a><span data-ttu-id="13927-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13927-137">Example</span></span>
<span data-ttu-id="13927-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="13927-138">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="13927-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13927-139">Request</span></span>
<span data-ttu-id="13927-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="13927-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="13927-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="13927-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-redirect"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/redirect

{
  "destinationPrinterId": "9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea"
}
```
# <a name="c"></a>[<span data-ttu-id="13927-142">C#</span><span class="sxs-lookup"><span data-stu-id="13927-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13927-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13927-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13927-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13927-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="13927-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="13927-145">Response</span></span>
<span data-ttu-id="13927-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="13927-146">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 437

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#printJob",
  "@odata.type": "#microsoft.graph.printJob",
  "id": "44354",
  "createdDateTime": "2020-06-30T17:19:09Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "userPrincipalName": ""
  },
  "status": {
    "processingState": "processing",
    "processingStateDescription": "The print job is currently being processed by the printer."
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob: redirect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
