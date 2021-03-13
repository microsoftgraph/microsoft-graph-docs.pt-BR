---
title: List taskTriggers
description: Recupere uma lista de gatilhos de tarefas associados à impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 62f2d3cc19a518edf65206bb26a1249dc9472b27
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771894"
---
# <a name="list-tasktriggers"></a><span data-ttu-id="7b172-103">List taskTriggers</span><span class="sxs-lookup"><span data-stu-id="7b172-103">List taskTriggers</span></span>
<span data-ttu-id="7b172-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b172-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="7b172-105">Recupere uma lista de [gatilhos de tarefas associados](../resources/printtasktrigger.md) à [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="7b172-105">Retrieve a list of [task triggers](../resources/printtasktrigger.md) associated with the [printer](../resources/printer.md).</span></span> <span data-ttu-id="7b172-106">A lista de gatilhos de tarefas define quais tarefas serão disparadas como resultado de eventos que ocorrem durante a impressão.</span><span class="sxs-lookup"><span data-stu-id="7b172-106">The list of task triggers defines which tasks will be triggered as a result of events that occur during printing.</span></span>

<span data-ttu-id="7b172-107">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="7b172-107">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="7b172-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b172-108">Permissions</span></span>
<span data-ttu-id="7b172-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b172-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7b172-111">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="7b172-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="7b172-112">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="7b172-112">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="7b172-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b172-113">Permission type</span></span> | <span data-ttu-id="7b172-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b172-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="7b172-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b172-115">Delegated (work or school account)</span></span>| <span data-ttu-id="7b172-116">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="7b172-116">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="7b172-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b172-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b172-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b172-118">Not Supported.</span></span>|
|<span data-ttu-id="7b172-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b172-119">Application</span></span>| <span data-ttu-id="7b172-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b172-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b172-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b172-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{printerId}/taskTriggers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b172-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7b172-122">Optional query parameters</span></span>
<span data-ttu-id="7b172-123">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7b172-123">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7b172-124">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7b172-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="7b172-125">Exceptions</span><span class="sxs-lookup"><span data-stu-id="7b172-125">Exceptions</span></span>
<span data-ttu-id="7b172-126">Alguns operadores não têm suporte: `$count` , , , , , , `$format` `$search` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="7b172-126">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b172-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b172-127">Request headers</span></span>
|<span data-ttu-id="7b172-128">Nome</span><span class="sxs-lookup"><span data-stu-id="7b172-128">Name</span></span>|<span data-ttu-id="7b172-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b172-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7b172-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b172-130">Authorization</span></span>|<span data-ttu-id="7b172-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b172-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b172-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b172-133">Request body</span></span>
<span data-ttu-id="7b172-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7b172-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b172-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b172-135">Response</span></span>

<span data-ttu-id="7b172-136">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printTaskTrigger](../resources/printtasktrigger.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b172-136">If successful, this method returns a `200 OK` response code and a collection of [printTaskTrigger](../resources/printtasktrigger.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7b172-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7b172-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7b172-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b172-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7b172-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b172-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printtasktrigger"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/taskTriggers
```
# <a name="c"></a>[<span data-ttu-id="7b172-140">C#</span><span class="sxs-lookup"><span data-stu-id="7b172-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printtasktrigger-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b172-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b172-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printtasktrigger-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b172-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b172-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printtasktrigger-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b172-143">Java</span><span class="sxs-lookup"><span data-stu-id="7b172-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printtasktrigger-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7b172-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b172-144">Response</span></span>
<span data-ttu-id="7b172-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7b172-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printTaskTrigger)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('fcc7fe6a-5ba7-4059-8017-702f3a41c8a4')/taskTriggers",
  "value": [
    {
      "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
      "event": "jobStarted"
    }
  ]
}
```

