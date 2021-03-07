---
title: Get taskTrigger
description: Obter um gatilho de tarefa de uma impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: ab17b71bcdb166b4db2732b88e9ba9b3b4ddc83c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517051"
---
# <a name="get-printtasktrigger"></a><span data-ttu-id="19442-103">Obter printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="19442-103">Get printTaskTrigger</span></span>

<span data-ttu-id="19442-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19442-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="19442-105">Obter um [gatilho de tarefa](../resources/printtasktrigger.md) de uma [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="19442-105">Get a [task trigger](../resources/printtasktrigger.md) from a [printer](../resources/printer.md).</span></span>

<span data-ttu-id="19442-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="19442-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="19442-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="19442-107">Permissions</span></span>
<span data-ttu-id="19442-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19442-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="19442-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="19442-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="19442-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19442-111">Permission type</span></span> | <span data-ttu-id="19442-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19442-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="19442-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19442-113">Delegated (work or school account)</span></span>| <span data-ttu-id="19442-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="19442-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="19442-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19442-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19442-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19442-116">Not Supported.</span></span>|
|<span data-ttu-id="19442-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19442-117">Application</span></span>|<span data-ttu-id="19442-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19442-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19442-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19442-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
```

## <a name="request-headers"></a><span data-ttu-id="19442-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19442-120">Request headers</span></span>
|<span data-ttu-id="19442-121">Nome</span><span class="sxs-lookup"><span data-stu-id="19442-121">Name</span></span>|<span data-ttu-id="19442-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="19442-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="19442-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="19442-123">Authorization</span></span>|<span data-ttu-id="19442-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19442-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="19442-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19442-126">Request body</span></span>
<span data-ttu-id="19442-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="19442-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19442-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="19442-128">Response</span></span>

<span data-ttu-id="19442-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printTaskTrigger](../resources/printtasktrigger.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19442-129">If successful, this method returns a `200 OK` response code and a [printTaskTrigger](../resources/printtasktrigger.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="19442-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="19442-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="19442-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19442-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printtasktrigger"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
```


### <a name="response"></a><span data-ttu-id="19442-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="19442-132">Response</span></span>
<span data-ttu-id="19442-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="19442-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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

