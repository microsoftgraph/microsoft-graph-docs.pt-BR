---
title: 'printJob: abort'
description: Anula um trabalho de impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: c92786af585eed2ba2b405fb9c6042c96b415a7b
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784835"
---
# <a name="printjob-abort"></a><span data-ttu-id="bbbb0-103">printJob: abort</span><span class="sxs-lookup"><span data-stu-id="bbbb0-103">printJob: abort</span></span>

<span data-ttu-id="bbbb0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbbb0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbbb0-105">Anula um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="bbbb0-105">Abort a print job.</span></span> <span data-ttu-id="bbbb0-106">Somente aplicativos que usam permissões de aplicativo podem anular um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="bbbb0-106">Only applications using application permissions can abort a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbbb0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bbbb0-107">Permissions</span></span>
<span data-ttu-id="bbbb0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbbb0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="bbbb0-110">Além das permissões a seguir, o locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter a permissão de aplicativo Printer.Read.All ou Printer.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="bbbb0-110">In addition to the following permissions, the app's tenant must have an active Universal Print subscription and have either the Printer.Read.All or Printer.ReadWrite.All application permission.</span></span>

|<span data-ttu-id="bbbb0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbbb0-111">Permission type</span></span> | <span data-ttu-id="bbbb0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbbb0-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="bbbb0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbbb0-113">Delegated (work or school account)</span></span>| <span data-ttu-id="bbbb0-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="bbbb0-114">Not Supported</span></span> |
|<span data-ttu-id="bbbb0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbbb0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbbb0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbbb0-116">Not Supported.</span></span>|
|<span data-ttu-id="bbbb0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbbb0-117">Application</span></span>| <span data-ttu-id="bbbb0-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbbb0-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbbb0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbbb0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/abort
```
## <a name="request-headers"></a><span data-ttu-id="bbbb0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbbb0-120">Request headers</span></span>
| <span data-ttu-id="bbbb0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="bbbb0-121">Name</span></span>          | <span data-ttu-id="bbbb0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbbb0-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bbbb0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbbb0-123">Authorization</span></span> | <span data-ttu-id="bbbb0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbbb0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbbb0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbbb0-126">Request body</span></span>
<span data-ttu-id="bbbb0-127">No corpo da solicitação, opcionalmente, você pode fornecer o motivo pelo qual o trabalho está sendo anulado.</span><span class="sxs-lookup"><span data-stu-id="bbbb0-127">In the request body, you can optionally provide the reason why the job is being aborted.</span></span>

| <span data-ttu-id="bbbb0-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbbb0-128">Property</span></span>     | <span data-ttu-id="bbbb0-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbbb0-129">Type</span></span>        | <span data-ttu-id="bbbb0-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbbb0-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bbbb0-131">motivo</span><span class="sxs-lookup"><span data-stu-id="bbbb0-131">reason</span></span>|<span data-ttu-id="bbbb0-132">String</span><span class="sxs-lookup"><span data-stu-id="bbbb0-132">String</span></span>|<span data-ttu-id="bbbb0-133">Motivo pelo qual o trabalho está sendo anulado.</span><span class="sxs-lookup"><span data-stu-id="bbbb0-133">Reason why job is being aborted.</span></span>|

## <a name="response"></a><span data-ttu-id="bbbb0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbbb0-134">Response</span></span>
<span data-ttu-id="bbbb0-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbbb0-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbbb0-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbbb0-137">Example</span></span>
<span data-ttu-id="bbbb0-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="bbbb0-138">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="bbbb0-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbbb0-139">Request</span></span>
<span data-ttu-id="bbbb0-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbbb0-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bbbb0-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbbb0-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-abort"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/abort
```
# <a name="c"></a>[<span data-ttu-id="bbbb0-142">C#</span><span class="sxs-lookup"><span data-stu-id="bbbb0-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-abort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bbbb0-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbbb0-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-abort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bbbb0-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbbb0-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-abort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bbbb0-145">Java</span><span class="sxs-lookup"><span data-stu-id="bbbb0-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-abort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bbbb0-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbbb0-146">Response</span></span>
<span data-ttu-id="bbbb0-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bbbb0-147">The following is an example of the response.</span></span> 
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
  "description": "printJob: abort",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
