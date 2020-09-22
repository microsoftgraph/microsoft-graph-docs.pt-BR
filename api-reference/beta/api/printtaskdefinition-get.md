---
title: Obter taskDefinition
description: Obter detalhes sobre uma definição de tarefa.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 33851ed2c70b17bbfa09ee6f3e68c15de53fd758
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035327"
---
# <a name="get-taskdefinition"></a><span data-ttu-id="c69a5-103">Obter taskDefinition</span><span class="sxs-lookup"><span data-stu-id="c69a5-103">Get taskDefinition</span></span>

<span data-ttu-id="c69a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c69a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c69a5-105">Obter detalhes sobre uma definição de tarefa.</span><span class="sxs-lookup"><span data-stu-id="c69a5-105">Get details about a task definition.</span></span>

<span data-ttu-id="c69a5-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à impressão universal, consulte [Estendeing universal print to support pull Printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="c69a5-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="c69a5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c69a5-107">Permissions</span></span>
<span data-ttu-id="c69a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c69a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c69a5-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="c69a5-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="c69a5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c69a5-111">Permission type</span></span> | <span data-ttu-id="c69a5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c69a5-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c69a5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c69a5-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c69a5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c69a5-114">Not supported.</span></span> |
|<span data-ttu-id="c69a5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c69a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c69a5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c69a5-116">Not Supported.</span></span>|
|<span data-ttu-id="c69a5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c69a5-117">Application</span></span>| <span data-ttu-id="c69a5-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c69a5-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c69a5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c69a5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c69a5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c69a5-120">Request headers</span></span>
| <span data-ttu-id="c69a5-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c69a5-121">Name</span></span>      |<span data-ttu-id="c69a5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c69a5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c69a5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c69a5-123">Authorization</span></span> | <span data-ttu-id="c69a5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c69a5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c69a5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c69a5-126">Request body</span></span>
<span data-ttu-id="c69a5-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c69a5-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c69a5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c69a5-128">Response</span></span>
<span data-ttu-id="c69a5-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [printTaskDefinition](../resources/printtaskdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c69a5-129">If successful, this method returns a `200 OK` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c69a5-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c69a5-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="c69a5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c69a5-131">Request</span></span>
<span data-ttu-id="c69a5-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c69a5-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c69a5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c69a5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskdefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions/fab143fd-ee61-4358-8558-2c7dee953982
```
# <a name="c"></a>[<span data-ttu-id="c69a5-134">C#</span><span class="sxs-lookup"><span data-stu-id="c69a5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskdefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c69a5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c69a5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskdefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c69a5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c69a5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskdefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="c69a5-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c69a5-137">Response</span></span>
<span data-ttu-id="c69a5-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c69a5-138">The following is an example of the response.</span></span>
><span data-ttu-id="c69a5-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c69a5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


