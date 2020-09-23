---
title: Atualizar continuousAccessEvaluationPolicy
description: Atualiza as propriedades de um objeto continuousAccessEvaluationPolicy.
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2838a02481690db3d81fd544e88fce65b2053495
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223087"
---
# <a name="update-continuousaccessevaluationpolicy"></a><span data-ttu-id="714ee-103">Atualizar continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="714ee-103">Update continuousAccessEvaluationPolicy</span></span>
<span data-ttu-id="714ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="714ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="714ee-105">Atualiza as propriedades de um objeto [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="714ee-105">Update the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="714ee-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="714ee-106">Permissions</span></span>
<span data-ttu-id="714ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="714ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="714ee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="714ee-109">Permission type</span></span>                        | <span data-ttu-id="714ee-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="714ee-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="714ee-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="714ee-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="714ee-112">Policy. Read. All, Policy. ReadWrite. ConditionalAccess e Application. Read. All</span><span class="sxs-lookup"><span data-stu-id="714ee-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
|<span data-ttu-id="714ee-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="714ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="714ee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="714ee-114">Not supported.</span></span> |
|<span data-ttu-id="714ee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="714ee-115">Application</span></span>                            | <span data-ttu-id="714ee-116">Policy. Read. All, Policy. ReadWrite. ConditionalAccess e Application. Read. All</span><span class="sxs-lookup"><span data-stu-id="714ee-116">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="714ee-117">Essa API tem um [problema conhecido](/graph/known-issues#permissions) relacionado às permissões.</span><span class="sxs-lookup"><span data-stu-id="714ee-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="714ee-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="714ee-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identity/continuousAccessEvaluationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="714ee-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="714ee-119">Request headers</span></span>
|<span data-ttu-id="714ee-120">Nome</span><span class="sxs-lookup"><span data-stu-id="714ee-120">Name</span></span>|<span data-ttu-id="714ee-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="714ee-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="714ee-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="714ee-122">Authorization</span></span>|<span data-ttu-id="714ee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="714ee-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="714ee-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="714ee-125">Content-Type</span></span>|<span data-ttu-id="714ee-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="714ee-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="714ee-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="714ee-128">Request body</span></span>
<span data-ttu-id="714ee-129">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="714ee-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="714ee-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="714ee-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="714ee-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="714ee-131">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="714ee-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="714ee-132">Property</span></span>|<span data-ttu-id="714ee-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="714ee-133">Type</span></span>|<span data-ttu-id="714ee-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="714ee-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="714ee-135">grupos</span><span class="sxs-lookup"><span data-stu-id="714ee-135">groups</span></span>|<span data-ttu-id="714ee-136">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="714ee-136">String collection</span></span>|<span data-ttu-id="714ee-137">A coleção de identificadores de grupo no escopo para avaliação.</span><span class="sxs-lookup"><span data-stu-id="714ee-137">The collection of group identifiers in scope for evaluation.</span></span> <span data-ttu-id="714ee-138">Todos os grupos estão no escopo quando a coleção está vazia.</span><span class="sxs-lookup"><span data-stu-id="714ee-138">All groups are in scope when the collection is empty.</span></span>|
|<span data-ttu-id="714ee-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="714ee-139">isEnabled</span></span>|<span data-ttu-id="714ee-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="714ee-140">Boolean</span></span>| <span data-ttu-id="714ee-141">`true` para indicar se a avaliação de acesso contínuo deve ser executada; caso contrário `false` .</span><span class="sxs-lookup"><span data-stu-id="714ee-141">`true` to indicate whether continuous access evaluation should be performed; otherwise `false`.</span></span> |
|<span data-ttu-id="714ee-142">usuários</span><span class="sxs-lookup"><span data-stu-id="714ee-142">users</span></span>|<span data-ttu-id="714ee-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="714ee-143">String collection</span></span>|<span data-ttu-id="714ee-144">A coleção de identificadores de usuário no escopo para avaliação.</span><span class="sxs-lookup"><span data-stu-id="714ee-144">The collection of user identifiers in scope for evaluation.</span></span> <span data-ttu-id="714ee-145">Todos os usuários estão no escopo quando a coleção está vazia.</span><span class="sxs-lookup"><span data-stu-id="714ee-145">All users are in scope when the collection is empty.</span></span>|


## <a name="response"></a><span data-ttu-id="714ee-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="714ee-146">Response</span></span>

<span data-ttu-id="714ee-p107">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="714ee-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="714ee-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="714ee-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="714ee-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="714ee-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="714ee-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="714ee-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_continuousaccessevaluationpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identity/continuousAccessEvaluationPolicy
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.continuousAccessEvaluationPolicy",
  "users": [ "88139f01-1f8d-4c06-ad74-a2544cee9aee" ],
  "groups": [ "9972fb3f-7a40-49f5-85f6-129d9dfbd47a", "ea178055-4713-4d9a-a06c-ff17466b7e77"]
}
```
# <a name="c"></a>[<span data-ttu-id="714ee-152">C#</span><span class="sxs-lookup"><span data-stu-id="714ee-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-continuousaccessevaluationpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="714ee-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="714ee-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-continuousaccessevaluationpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="714ee-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="714ee-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-continuousaccessevaluationpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="714ee-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="714ee-155">Response</span></span>

<span data-ttu-id="714ee-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="714ee-156">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```
