---
title: 'printJob: abort'
description: Aborte um trabalho de impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 55ee53dd758116edd14149a9dc20270fa49b1679
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771404"
---
# <a name="printjob-abort"></a><span data-ttu-id="3f7d9-103">printJob: abort</span><span class="sxs-lookup"><span data-stu-id="3f7d9-103">printJob: abort</span></span>

<span data-ttu-id="3f7d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f7d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="3f7d9-105">Aborte um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="3f7d9-105">Abort a print job.</span></span> <span data-ttu-id="3f7d9-106">Somente aplicativos que usam permissões de aplicativo podem cancelar um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="3f7d9-106">Only applications using application permissions can abort a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f7d9-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="3f7d9-107">Permissions</span></span>
<span data-ttu-id="3f7d9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f7d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3f7d9-110">Além das permissões a seguir, o locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter a permissão Printer.Read.All ou Printer.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="3f7d9-110">In addition to the following permissions, the app's tenant must have an active Universal Print subscription and have either the Printer.Read.All or Printer.ReadWrite.All application permission.</span></span>

|<span data-ttu-id="3f7d9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f7d9-111">Permission type</span></span> | <span data-ttu-id="3f7d9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3f7d9-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3f7d9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f7d9-113">Delegated (work or school account)</span></span>| <span data-ttu-id="3f7d9-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="3f7d9-114">Not Supported</span></span> |
|<span data-ttu-id="3f7d9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f7d9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f7d9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f7d9-116">Not Supported.</span></span>|
|<span data-ttu-id="3f7d9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f7d9-117">Application</span></span>| <span data-ttu-id="3f7d9-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="3f7d9-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f7d9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f7d9-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/jobs/{printJobId}/abort
```

## <a name="request-headers"></a><span data-ttu-id="3f7d9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f7d9-120">Request headers</span></span>
|<span data-ttu-id="3f7d9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3f7d9-121">Name</span></span>|<span data-ttu-id="3f7d9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f7d9-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3f7d9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f7d9-123">Authorization</span></span>|<span data-ttu-id="3f7d9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f7d9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f7d9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f7d9-126">Request body</span></span>
<span data-ttu-id="3f7d9-127">No corpo da solicitação, opcionalmente, você pode fornecer o motivo pelo qual o trabalho está sendo abortado.</span><span class="sxs-lookup"><span data-stu-id="3f7d9-127">In the request body, you can optionally provide the reason why the job is being aborted.</span></span>

| <span data-ttu-id="3f7d9-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f7d9-128">Property</span></span>     | <span data-ttu-id="3f7d9-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f7d9-129">Type</span></span>        | <span data-ttu-id="3f7d9-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f7d9-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3f7d9-131">motivo</span><span class="sxs-lookup"><span data-stu-id="3f7d9-131">reason</span></span>|<span data-ttu-id="3f7d9-132">String</span><span class="sxs-lookup"><span data-stu-id="3f7d9-132">String</span></span>|<span data-ttu-id="3f7d9-133">Motivo pelo qual o trabalho está sendo abortado.</span><span class="sxs-lookup"><span data-stu-id="3f7d9-133">Reason why job is being aborted.</span></span>|

## <a name="response"></a><span data-ttu-id="3f7d9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f7d9-134">Response</span></span>

<span data-ttu-id="3f7d9-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f7d9-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3f7d9-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3f7d9-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3f7d9-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f7d9-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3f7d9-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f7d9-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob_abort"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/abort
Content-Type: application/json
Content-length: 26

{
  "reason": "String"
}
```
# <a name="c"></a>[<span data-ttu-id="3f7d9-140">C#</span><span class="sxs-lookup"><span data-stu-id="3f7d9-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-abort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f7d9-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f7d9-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-abort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f7d9-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f7d9-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-abort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f7d9-143">Java</span><span class="sxs-lookup"><span data-stu-id="3f7d9-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-abort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3f7d9-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f7d9-144">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

