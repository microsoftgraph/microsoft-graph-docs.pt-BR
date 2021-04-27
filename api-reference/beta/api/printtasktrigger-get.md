---
title: Get taskTrigger
description: Obter um gatilho de tarefa de uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 3976b61801d6f7bff3a1355666849a8e46f56c70
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053563"
---
# <a name="get-tasktrigger"></a><span data-ttu-id="23cb7-103">Get taskTrigger</span><span class="sxs-lookup"><span data-stu-id="23cb7-103">Get taskTrigger</span></span>

<span data-ttu-id="23cb7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23cb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23cb7-105">Obter um [gatilho de tarefa](../resources/printtasktrigger.md) de uma [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="23cb7-105">Get a [task trigger](../resources/printtasktrigger.md) from a [printer](../resources/printer.md).</span></span>

<span data-ttu-id="23cb7-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="23cb7-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="23cb7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="23cb7-107">Permissions</span></span>
<span data-ttu-id="23cb7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23cb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="23cb7-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="23cb7-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="23cb7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23cb7-111">Permission type</span></span> | <span data-ttu-id="23cb7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23cb7-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="23cb7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23cb7-113">Delegated (work or school account)</span></span>| <span data-ttu-id="23cb7-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="23cb7-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="23cb7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23cb7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23cb7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23cb7-116">Not Supported.</span></span>|
|<span data-ttu-id="23cb7-117">Application</span><span class="sxs-lookup"><span data-stu-id="23cb7-117">Application</span></span>|<span data-ttu-id="23cb7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23cb7-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23cb7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23cb7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/taskTriggers/{id}
```

## <a name="request-headers"></a><span data-ttu-id="23cb7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23cb7-120">Request headers</span></span>
| <span data-ttu-id="23cb7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="23cb7-121">Name</span></span>      |<span data-ttu-id="23cb7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="23cb7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="23cb7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="23cb7-123">Authorization</span></span> | <span data-ttu-id="23cb7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23cb7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23cb7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23cb7-126">Request body</span></span>
<span data-ttu-id="23cb7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23cb7-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="23cb7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="23cb7-128">Response</span></span>
<span data-ttu-id="23cb7-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto printTaskTrigger](../resources/printtasktrigger.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23cb7-129">If successful, this method returns a `200 OK` response code and [printTaskTrigger](../resources/printtasktrigger.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="23cb7-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23cb7-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="23cb7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23cb7-131">Request</span></span>
<span data-ttu-id="23cb7-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="23cb7-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="23cb7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="23cb7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer_tasktrigger"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{printerId}/taskTriggers/{taskTriggerId}
```
# <a name="c"></a>[<span data-ttu-id="23cb7-134">C#</span><span class="sxs-lookup"><span data-stu-id="23cb7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-tasktrigger-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23cb7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23cb7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-tasktrigger-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23cb7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23cb7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-tasktrigger-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23cb7-137">Java</span><span class="sxs-lookup"><span data-stu-id="23cb7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printer-tasktrigger-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="23cb7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="23cb7-138">Response</span></span>
<span data-ttu-id="23cb7-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="23cb7-139">The following is an example of the response.</span></span>
><span data-ttu-id="23cb7-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="23cb7-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 181

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers/taskTriggers/$entity",
  "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
  "event": "jobStarted"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get taskTrigger",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


