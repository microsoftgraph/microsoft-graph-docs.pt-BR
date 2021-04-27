---
title: Criar taskDefinition
description: Crie uma nova definição de tarefa.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 2e6a9eaca89e7ec68d2eee2053ead369cbcd5831
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053619"
---
# <a name="create-taskdefinition"></a><span data-ttu-id="e965c-103">Criar taskDefinition</span><span class="sxs-lookup"><span data-stu-id="e965c-103">Create taskDefinition</span></span>

<span data-ttu-id="e965c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e965c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e965c-105">Crie uma nova definição de tarefa.</span><span class="sxs-lookup"><span data-stu-id="e965c-105">Create a new task definition.</span></span>

<span data-ttu-id="e965c-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="e965c-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="e965c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e965c-107">Permissions</span></span>
<span data-ttu-id="e965c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e965c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e965c-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="e965c-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="e965c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e965c-111">Permission type</span></span> | <span data-ttu-id="e965c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e965c-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e965c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e965c-113">Delegated (work or school account)</span></span>| <span data-ttu-id="e965c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e965c-114">Not supported.</span></span> |
|<span data-ttu-id="e965c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e965c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e965c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e965c-116">Not Supported.</span></span>|
|<span data-ttu-id="e965c-117">Application</span><span class="sxs-lookup"><span data-stu-id="e965c-117">Application</span></span>| <span data-ttu-id="e965c-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e965c-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e965c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e965c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/taskDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="e965c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e965c-120">Request headers</span></span>
| <span data-ttu-id="e965c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e965c-121">Name</span></span>      |<span data-ttu-id="e965c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e965c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e965c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e965c-123">Authorization</span></span> | <span data-ttu-id="e965c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e965c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e965c-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="e965c-126">Content-type</span></span>  | <span data-ttu-id="e965c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e965c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e965c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e965c-129">Request body</span></span>
<span data-ttu-id="e965c-130">No corpo da solicitação, fornece uma representação JSON do [objeto printTaskDefinition.](../resources/printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e965c-130">In the request body, supply a JSON representation of [printTaskDefinition](../resources/printtaskdefinition.md) object.</span></span>

<span data-ttu-id="e965c-131">As [propriedades printTaskDefinition](../resources/printtaskdefinition.md)e **createdBy.appId** são definidas automaticamente após a criação de recursos. </span><span class="sxs-lookup"><span data-stu-id="e965c-131">The [printTaskDefinition](../resources/printtaskdefinition.md)'s **id** and **createdBy.appId** properties are set automatically upon resource creation.</span></span>

## <a name="response"></a><span data-ttu-id="e965c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e965c-132">Response</span></span>
<span data-ttu-id="e965c-133">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto printTaskDefinition](../resources/printtaskdefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e965c-133">If successful, this method returns a `201 Created` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e965c-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e965c-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="e965c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e965c-135">Request</span></span>
<span data-ttu-id="e965c-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e965c-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e965c-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e965c-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "print_create_taskdefinition"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/print/taskDefinitions
Content-type: application/json
Content-length: 122

{
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "displayName": "Requesting App Display Name"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="e965c-138">C#</span><span class="sxs-lookup"><span data-stu-id="e965c-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/print-create-taskdefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e965c-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e965c-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/print-create-taskdefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e965c-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e965c-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/print-create-taskdefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e965c-141">Java</span><span class="sxs-lookup"><span data-stu-id="e965c-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/print-create-taskdefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="e965c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e965c-142">Response</span></span>
<span data-ttu-id="e965c-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e965c-143">The following is an example of the response.</span></span>
><span data-ttu-id="e965c-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e965c-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 322

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions/$entity",
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
  "description": "Create taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


