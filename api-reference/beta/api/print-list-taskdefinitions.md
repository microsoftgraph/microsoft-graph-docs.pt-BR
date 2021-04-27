---
title: Listar taskDefinitions
description: Recupere uma lista de definições de tarefas definidas pelo aplicativo solicitando no locatário.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 68de2409013cff88752f5a26f1ea06e2a25bb755
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053633"
---
# <a name="list-taskdefinitions"></a><span data-ttu-id="be15f-103">Listar taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="be15f-103">List taskDefinitions</span></span>

<span data-ttu-id="be15f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be15f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be15f-105">Recupere uma lista de [definições de tarefas definidas](../resources/printtaskdefinition.md) pelo aplicativo solicitando no locatário.</span><span class="sxs-lookup"><span data-stu-id="be15f-105">Retrieve a list of [task definitions](../resources/printtaskdefinition.md) that the requesting app defined in the tenant.</span></span>

<span data-ttu-id="be15f-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="be15f-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="be15f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="be15f-107">Permissions</span></span>
<span data-ttu-id="be15f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be15f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="be15f-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="be15f-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="be15f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be15f-111">Permission type</span></span> | <span data-ttu-id="be15f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be15f-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="be15f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be15f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="be15f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be15f-114">Not supported.</span></span> |
|<span data-ttu-id="be15f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be15f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be15f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be15f-116">Not Supported.</span></span>|
|<span data-ttu-id="be15f-117">Application</span><span class="sxs-lookup"><span data-stu-id="be15f-117">Application</span></span>| <span data-ttu-id="be15f-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be15f-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="be15f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be15f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be15f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="be15f-120">Optional query parameters</span></span>
<span data-ttu-id="be15f-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="be15f-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="be15f-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="be15f-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="be15f-123">Exceções</span><span class="sxs-lookup"><span data-stu-id="be15f-123">Exceptions</span></span>
<span data-ttu-id="be15f-124">Alguns operadores não têm suporte: `$count` , , , , , , `$format` `$search` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="be15f-124">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be15f-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be15f-125">Request headers</span></span>
| <span data-ttu-id="be15f-126">Nome</span><span class="sxs-lookup"><span data-stu-id="be15f-126">Name</span></span>      |<span data-ttu-id="be15f-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="be15f-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="be15f-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="be15f-128">Authorization</span></span> | <span data-ttu-id="be15f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be15f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be15f-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be15f-131">Request body</span></span>
<span data-ttu-id="be15f-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="be15f-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="be15f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="be15f-133">Response</span></span>
<span data-ttu-id="be15f-134">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos printTaskDefinition](../resources/printtaskdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be15f-134">If successful, this method returns a `200 OK` response code and a collection of [printTaskDefinition](../resources/printtaskdefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be15f-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be15f-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="be15f-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be15f-136">Request</span></span>
<span data-ttu-id="be15f-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="be15f-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="be15f-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="be15f-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "print_list_taskdefinitions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions
```
# <a name="c"></a>[<span data-ttu-id="be15f-139">C#</span><span class="sxs-lookup"><span data-stu-id="be15f-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/print-list-taskdefinitions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be15f-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be15f-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/print-list-taskdefinitions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be15f-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be15f-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/print-list-taskdefinitions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="be15f-142">Java</span><span class="sxs-lookup"><span data-stu-id="be15f-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/print-list-taskdefinitions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="be15f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="be15f-143">Response</span></span>
<span data-ttu-id="be15f-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="be15f-144">The following is an example of the response.</span></span>
><span data-ttu-id="be15f-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="be15f-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions",
  "value": [
    {
      "id": "fab143fd-ee61-4358-8558-2c7dee953982",
      "displayName": "Test TaskDefinitionName",
      "createdBy": {
        "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
        "displayName": "Requesting App Display Name"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List taskDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


