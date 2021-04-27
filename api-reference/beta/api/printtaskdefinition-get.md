---
title: Obter taskDefinition
description: Obter detalhes sobre uma definição de tarefa.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 40e3b2c32545cebc548cbaec27463904ea5ce384
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053584"
---
# <a name="get-taskdefinition"></a><span data-ttu-id="8ed6d-103">Obter taskDefinition</span><span class="sxs-lookup"><span data-stu-id="8ed6d-103">Get taskDefinition</span></span>

<span data-ttu-id="8ed6d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ed6d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ed6d-105">Obter detalhes sobre uma definição de tarefa.</span><span class="sxs-lookup"><span data-stu-id="8ed6d-105">Get details about a task definition.</span></span>

<span data-ttu-id="8ed6d-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="8ed6d-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="8ed6d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ed6d-107">Permissions</span></span>
<span data-ttu-id="8ed6d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ed6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8ed6d-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="8ed6d-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="8ed6d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ed6d-111">Permission type</span></span> | <span data-ttu-id="8ed6d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ed6d-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8ed6d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ed6d-113">Delegated (work or school account)</span></span>| <span data-ttu-id="8ed6d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ed6d-114">Not supported.</span></span> |
|<span data-ttu-id="8ed6d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ed6d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ed6d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ed6d-116">Not Supported.</span></span>|
|<span data-ttu-id="8ed6d-117">Application</span><span class="sxs-lookup"><span data-stu-id="8ed6d-117">Application</span></span>| <span data-ttu-id="8ed6d-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ed6d-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ed6d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ed6d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8ed6d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed6d-120">Request headers</span></span>
| <span data-ttu-id="8ed6d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8ed6d-121">Name</span></span>      |<span data-ttu-id="8ed6d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ed6d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8ed6d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ed6d-123">Authorization</span></span> | <span data-ttu-id="8ed6d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ed6d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ed6d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed6d-126">Request body</span></span>
<span data-ttu-id="8ed6d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ed6d-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8ed6d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ed6d-128">Response</span></span>
<span data-ttu-id="8ed6d-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto printTaskDefinition](../resources/printtaskdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ed6d-129">If successful, this method returns a `200 OK` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8ed6d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ed6d-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="8ed6d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed6d-131">Request</span></span>
<span data-ttu-id="8ed6d-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ed6d-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8ed6d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ed6d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskdefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions/fab143fd-ee61-4358-8558-2c7dee953982
```
# <a name="c"></a>[<span data-ttu-id="8ed6d-134">C#</span><span class="sxs-lookup"><span data-stu-id="8ed6d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskdefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ed6d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ed6d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskdefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ed6d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ed6d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskdefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8ed6d-137">Java</span><span class="sxs-lookup"><span data-stu-id="8ed6d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-taskdefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="8ed6d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ed6d-138">Response</span></span>
<span data-ttu-id="8ed6d-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8ed6d-139">The following is an example of the response.</span></span>
><span data-ttu-id="8ed6d-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8ed6d-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 380

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions/$entity",
  "@odata.type": "#microsoft.graph.printTaskDefinition",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
    "displayName": "Requesting App Display Name"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


