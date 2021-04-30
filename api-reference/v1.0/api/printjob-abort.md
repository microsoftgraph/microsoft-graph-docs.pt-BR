---
title: 'printJob: abort'
description: Aborte um trabalho de impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 4f9bfb7623e546c402853c31eba750f5c4040966
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080089"
---
# <a name="printjob-abort"></a><span data-ttu-id="d4e0c-103">printJob: abort</span><span class="sxs-lookup"><span data-stu-id="d4e0c-103">printJob: abort</span></span>

<span data-ttu-id="d4e0c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4e0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="d4e0c-105">Aborte um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="d4e0c-105">Abort a print job.</span></span> <span data-ttu-id="d4e0c-106">Somente aplicativos que usam permissões de aplicativo podem cancelar um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="d4e0c-106">Only applications using application permissions can abort a print job.</span></span>

<span data-ttu-id="d4e0c-107">A anulação de um trabalho de impressão só terá êxito se houver [uma printTask](../resources/printTask.md) em um estado no trabalho de impressão associado, iniciado por um gatilho criado pelo aplicativo `processing` solicitante.</span><span class="sxs-lookup"><span data-stu-id="d4e0c-107">Aborting a print job will only succeed if there is a [printTask](../resources/printTask.md) in a `processing` state on the associated print job, started by a trigger that the requesting app created.</span></span> <span data-ttu-id="d4e0c-108">Para obter detalhes sobre como registrar um gatilho de tarefas, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="d4e0c-108">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="d4e0c-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4e0c-109">Permissions</span></span>
<span data-ttu-id="d4e0c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4e0c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d4e0c-112">Além das permissões a seguir, o locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter a permissão Printer.Read.All ou Printer.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="d4e0c-112">In addition to the following permissions, the app's tenant must have an active Universal Print subscription and have either the Printer.Read.All or Printer.ReadWrite.All application permission.</span></span>

|<span data-ttu-id="d4e0c-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4e0c-113">Permission type</span></span> | <span data-ttu-id="d4e0c-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4e0c-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d4e0c-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4e0c-115">Delegated (work or school account)</span></span>| <span data-ttu-id="d4e0c-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="d4e0c-116">Not Supported</span></span> |
|<span data-ttu-id="d4e0c-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4e0c-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4e0c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4e0c-118">Not Supported.</span></span>|
|<span data-ttu-id="d4e0c-119">Application</span><span class="sxs-lookup"><span data-stu-id="d4e0c-119">Application</span></span>| <span data-ttu-id="d4e0c-120">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="d4e0c-120">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4e0c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4e0c-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/jobs/{printJobId}/abort
```

## <a name="request-headers"></a><span data-ttu-id="d4e0c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e0c-122">Request headers</span></span>
|<span data-ttu-id="d4e0c-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d4e0c-123">Name</span></span>|<span data-ttu-id="d4e0c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4e0c-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d4e0c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4e0c-125">Authorization</span></span>|<span data-ttu-id="d4e0c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4e0c-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4e0c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e0c-128">Request body</span></span>
<span data-ttu-id="d4e0c-129">No corpo da solicitação, opcionalmente, você pode fornecer o motivo pelo qual o trabalho está sendo abortado.</span><span class="sxs-lookup"><span data-stu-id="d4e0c-129">In the request body, you can optionally provide the reason why the job is being aborted.</span></span>

| <span data-ttu-id="d4e0c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4e0c-130">Property</span></span>     | <span data-ttu-id="d4e0c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4e0c-131">Type</span></span>        | <span data-ttu-id="d4e0c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4e0c-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d4e0c-133">motivo</span><span class="sxs-lookup"><span data-stu-id="d4e0c-133">reason</span></span>|<span data-ttu-id="d4e0c-134">String</span><span class="sxs-lookup"><span data-stu-id="d4e0c-134">String</span></span>|<span data-ttu-id="d4e0c-135">Motivo pelo qual o trabalho está sendo abortado.</span><span class="sxs-lookup"><span data-stu-id="d4e0c-135">Reason why job is being aborted.</span></span>|

## <a name="response"></a><span data-ttu-id="d4e0c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4e0c-136">Response</span></span>

<span data-ttu-id="d4e0c-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4e0c-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4e0c-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d4e0c-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4e0c-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e0c-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d4e0c-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4e0c-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d4e0c-142">C#</span><span class="sxs-lookup"><span data-stu-id="d4e0c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-abort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4e0c-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4e0c-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-abort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4e0c-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4e0c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-abort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4e0c-145">Java</span><span class="sxs-lookup"><span data-stu-id="d4e0c-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-abort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d4e0c-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4e0c-146">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

