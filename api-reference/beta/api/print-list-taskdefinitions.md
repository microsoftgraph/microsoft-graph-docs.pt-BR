---
title: Listar taskDefinitions
description: Recupere uma lista de definições de tarefas que o aplicativo solicitante definido no locatário.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 26a3a8aa25d66b3cffa163078a8e466057433311
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566435"
---
# <a name="list-taskdefinitions"></a><span data-ttu-id="c1e36-103">Listar taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="c1e36-103">List taskDefinitions</span></span>

<span data-ttu-id="c1e36-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1e36-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1e36-105">Recupere uma lista de [definições de tarefas](../resources/printtaskdefinition.md) que o aplicativo solicitante definido no locatário.</span><span class="sxs-lookup"><span data-stu-id="c1e36-105">Retrieve a list of [task definitions](../resources/printtaskdefinition.md) that the requesting app defined in the tenant.</span></span>

<span data-ttu-id="c1e36-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à impressão universal, consulte [Estendeing universal print to support pull Printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="c1e36-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="c1e36-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c1e36-107">Permissions</span></span>
<span data-ttu-id="c1e36-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1e36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c1e36-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="c1e36-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="c1e36-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1e36-111">Permission type</span></span> | <span data-ttu-id="c1e36-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c1e36-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c1e36-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1e36-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c1e36-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1e36-114">Not supported.</span></span> |
|<span data-ttu-id="c1e36-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1e36-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1e36-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1e36-116">Not Supported.</span></span>|
|<span data-ttu-id="c1e36-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1e36-117">Application</span></span>| <span data-ttu-id="c1e36-118">PrintTaskDefinition. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c1e36-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1e36-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1e36-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1e36-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c1e36-120">Optional query parameters</span></span>
<span data-ttu-id="c1e36-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c1e36-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c1e36-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c1e36-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="c1e36-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="c1e36-123">Exceptions</span></span>
<span data-ttu-id="c1e36-124">Não há suporte para alguns operadores: `$count` ,,,, `$format` `$search` `$select` `$skip` , `$top` .</span><span class="sxs-lookup"><span data-stu-id="c1e36-124">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1e36-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1e36-125">Request headers</span></span>
| <span data-ttu-id="c1e36-126">Nome</span><span class="sxs-lookup"><span data-stu-id="c1e36-126">Name</span></span>      |<span data-ttu-id="c1e36-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1e36-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c1e36-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1e36-128">Authorization</span></span> | <span data-ttu-id="c1e36-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1e36-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1e36-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1e36-131">Request body</span></span>
<span data-ttu-id="c1e36-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c1e36-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c1e36-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1e36-133">Response</span></span>
<span data-ttu-id="c1e36-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [printTaskDefinition](../resources/printtaskdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1e36-134">If successful, this method returns a `200 OK` response code and a collection of [printTaskDefinition](../resources/printtaskdefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c1e36-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1e36-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="c1e36-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1e36-136">Request</span></span>
<span data-ttu-id="c1e36-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1e36-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c1e36-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1e36-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "print_list_taskdefinitions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions
```
# <a name="c"></a>[<span data-ttu-id="c1e36-139">C#</span><span class="sxs-lookup"><span data-stu-id="c1e36-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/print-list-taskdefinitions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1e36-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1e36-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/print-list-taskdefinitions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1e36-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1e36-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/print-list-taskdefinitions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="c1e36-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1e36-142">Response</span></span>
<span data-ttu-id="c1e36-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c1e36-143">The following is an example of the response.</span></span>
><span data-ttu-id="c1e36-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1e36-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
