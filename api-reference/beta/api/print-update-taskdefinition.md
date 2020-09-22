---
title: Atualizar taskDefinition
description: Atualizar uma definição de tarefa.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: f029dd1e5463d6d69e78e76a90504ab610388533
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035898"
---
# <a name="update-taskdefinition"></a><span data-ttu-id="f3b41-103">Atualizar taskDefinition</span><span class="sxs-lookup"><span data-stu-id="f3b41-103">Update taskDefinition</span></span>

<span data-ttu-id="f3b41-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3b41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3b41-105">Atualizar uma definição de tarefa.</span><span class="sxs-lookup"><span data-stu-id="f3b41-105">Update a task definition.</span></span>

<span data-ttu-id="f3b41-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à impressão universal, consulte [Estendeing universal print to support pull Printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="f3b41-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="f3b41-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f3b41-107">Permissions</span></span>
<span data-ttu-id="f3b41-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3b41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f3b41-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="f3b41-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="f3b41-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3b41-111">Permission type</span></span> | <span data-ttu-id="f3b41-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3b41-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f3b41-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3b41-113">Delegated (work or school account)</span></span>| <span data-ttu-id="f3b41-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3b41-114">Not supported.</span></span> |
|<span data-ttu-id="f3b41-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3b41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3b41-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3b41-116">Not Supported.</span></span>|
|<span data-ttu-id="f3b41-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3b41-117">Application</span></span>| <span data-ttu-id="f3b41-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3b41-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3b41-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3b41-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/taskDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f3b41-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3b41-120">Request headers</span></span>
| <span data-ttu-id="f3b41-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f3b41-121">Name</span></span>      |<span data-ttu-id="f3b41-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3b41-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f3b41-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3b41-123">Authorization</span></span> | <span data-ttu-id="f3b41-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3b41-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f3b41-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="f3b41-126">Content-type</span></span>  | <span data-ttu-id="f3b41-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3b41-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3b41-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3b41-129">Request body</span></span>
<span data-ttu-id="f3b41-130">No corpo da solicitação, forneça os valores para os campos [printTaskDefinition](../resources/printtaskdefinition.md) relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f3b41-130">In the request body, supply the values for the relevant [printTaskDefinition](../resources/printtaskdefinition.md) fields that should be updated.</span></span> <span data-ttu-id="f3b41-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="f3b41-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f3b41-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f3b41-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f3b41-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3b41-133">Property</span></span>     | <span data-ttu-id="f3b41-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3b41-134">Type</span></span>        | <span data-ttu-id="f3b41-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3b41-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f3b41-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f3b41-136">displayName</span></span>|<span data-ttu-id="f3b41-137">String</span><span class="sxs-lookup"><span data-stu-id="f3b41-137">String</span></span>|<span data-ttu-id="f3b41-138">O nome do printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="f3b41-138">The name of the printTaskDefinition.</span></span>|
|<span data-ttu-id="f3b41-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="f3b41-139">createdBy</span></span>|<span data-ttu-id="f3b41-140">String</span><span class="sxs-lookup"><span data-stu-id="f3b41-140">String</span></span>|<span data-ttu-id="f3b41-141">Informações sobre o aplicativo que criou a definição de tarefa.</span><span class="sxs-lookup"><span data-stu-id="f3b41-141">Information about the app that created the task definition.</span></span> <span data-ttu-id="f3b41-142">Somente a `createdBy.displayName` propriedade pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="f3b41-142">Only the `createdBy.displayName` property can be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="f3b41-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3b41-143">Response</span></span>
<span data-ttu-id="f3b41-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3b41-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f3b41-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3b41-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="f3b41-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3b41-147">Request</span></span>
<span data-ttu-id="f3b41-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3b41-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f3b41-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3b41-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "print_update_taskdefinition"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/beta/print/taskDefinitions/fab143fd-ee61-4358-8558-2c7dee953982
Content-type: application/json
Content-length: 122

{
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "displayName": "Requesting App Display Name"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="f3b41-150">C#</span><span class="sxs-lookup"><span data-stu-id="f3b41-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/print-update-taskdefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f3b41-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f3b41-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/print-update-taskdefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f3b41-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f3b41-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/print-update-taskdefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="f3b41-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3b41-153">Response</span></span>
<span data-ttu-id="f3b41-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f3b41-154">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


