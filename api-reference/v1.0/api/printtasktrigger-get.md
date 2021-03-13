---
title: Get taskTrigger
description: Obter um gatilho de tarefa de uma impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 42794100705dff60c224cd511984d2d29a8014f3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774479"
---
# <a name="get-printtasktrigger"></a><span data-ttu-id="f447f-103">Obter printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="f447f-103">Get printTaskTrigger</span></span>

<span data-ttu-id="f447f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f447f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="f447f-105">Obter um [gatilho de tarefa](../resources/printtasktrigger.md) de uma [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="f447f-105">Get a [task trigger](../resources/printtasktrigger.md) from a [printer](../resources/printer.md).</span></span>

<span data-ttu-id="f447f-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="f447f-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="f447f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f447f-107">Permissions</span></span>
<span data-ttu-id="f447f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f447f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f447f-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="f447f-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="f447f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f447f-111">Permission type</span></span> | <span data-ttu-id="f447f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f447f-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f447f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f447f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="f447f-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="f447f-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="f447f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f447f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f447f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f447f-116">Not Supported.</span></span>|
|<span data-ttu-id="f447f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f447f-117">Application</span></span>|<span data-ttu-id="f447f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f447f-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f447f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f447f-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
```

## <a name="request-headers"></a><span data-ttu-id="f447f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f447f-120">Request headers</span></span>
|<span data-ttu-id="f447f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f447f-121">Name</span></span>|<span data-ttu-id="f447f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f447f-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f447f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f447f-123">Authorization</span></span>|<span data-ttu-id="f447f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f447f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f447f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f447f-126">Request body</span></span>
<span data-ttu-id="f447f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f447f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f447f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f447f-128">Response</span></span>

<span data-ttu-id="f447f-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printTaskTrigger](../resources/printtasktrigger.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f447f-129">If successful, this method returns a `200 OK` response code and a [printTaskTrigger](../resources/printtasktrigger.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f447f-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f447f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f447f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f447f-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f447f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f447f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printtasktrigger"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
```
# <a name="c"></a>[<span data-ttu-id="f447f-133">C#</span><span class="sxs-lookup"><span data-stu-id="f447f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printtasktrigger-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f447f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f447f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printtasktrigger-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f447f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f447f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printtasktrigger-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f447f-136">Java</span><span class="sxs-lookup"><span data-stu-id="f447f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printtasktrigger-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f447f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f447f-137">Response</span></span>
<span data-ttu-id="f447f-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f447f-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers/taskTriggers/$entity",
  "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
  "event": "jobStarted"
}
```

