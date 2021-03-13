---
title: Excluir printTaskTrigger
description: Exclua o gatilho de tarefas de uma impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: bba66bb6c11d930b1b9065769181f55efc114dd4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772013"
---
# <a name="delete-printtasktrigger"></a><span data-ttu-id="eff58-103">Excluir printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="eff58-103">Delete printTaskTrigger</span></span>
<span data-ttu-id="eff58-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eff58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="eff58-105">[Exclua o gatilho de](../resources/printtasktrigger.md) tarefas de uma [impressora](../resources/printer.md) para impedir que eventos de impressão relacionados acionem tarefas na impressora especificada.</span><span class="sxs-lookup"><span data-stu-id="eff58-105">Delete the [task trigger](../resources/printtasktrigger.md) of a [printer](../resources/printer.md) to prevent related print events from triggering tasks on the specified printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="eff58-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="eff58-106">Permissions</span></span>
<span data-ttu-id="eff58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eff58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="eff58-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="eff58-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="eff58-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eff58-110">Permission type</span></span> | <span data-ttu-id="eff58-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eff58-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="eff58-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eff58-112">Delegated (work or school account)</span></span>| <span data-ttu-id="eff58-113">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="eff58-113">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="eff58-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eff58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eff58-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eff58-115">Not Supported.</span></span>|
|<span data-ttu-id="eff58-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eff58-116">Application</span></span>|<span data-ttu-id="eff58-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eff58-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eff58-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eff58-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
```

## <a name="request-headers"></a><span data-ttu-id="eff58-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eff58-119">Request headers</span></span>
|<span data-ttu-id="eff58-120">Nome</span><span class="sxs-lookup"><span data-stu-id="eff58-120">Name</span></span>|<span data-ttu-id="eff58-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="eff58-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eff58-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eff58-122">Authorization</span></span>|<span data-ttu-id="eff58-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eff58-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eff58-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eff58-125">Request body</span></span>
<span data-ttu-id="eff58-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eff58-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eff58-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="eff58-127">Response</span></span>

<span data-ttu-id="eff58-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="eff58-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="eff58-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eff58-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eff58-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eff58-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="eff58-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="eff58-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printtasktrigger"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
```
# <a name="c"></a>[<span data-ttu-id="eff58-132">C#</span><span class="sxs-lookup"><span data-stu-id="eff58-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printtasktrigger-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eff58-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eff58-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printtasktrigger-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eff58-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eff58-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printtasktrigger-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eff58-135">Java</span><span class="sxs-lookup"><span data-stu-id="eff58-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-printtasktrigger-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eff58-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="eff58-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

