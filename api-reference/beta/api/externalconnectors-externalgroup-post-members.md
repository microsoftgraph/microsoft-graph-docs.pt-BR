---
title: Criar externalGroupMember
description: Crie um novo objeto externalGroupMember.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 3120c6aa7744aeedebf8fa6b4eb1a696b21e6e37
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467546"
---
# <a name="create-externalgroupmember"></a><span data-ttu-id="569e1-103">Criar externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="569e1-103">Create externalGroupMember</span></span>

<span data-ttu-id="569e1-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="569e1-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="569e1-105">Crie um novo [objeto externalGroupMember.](../resources/externalconnectors-externalgroupmember.md)</span><span class="sxs-lookup"><span data-stu-id="569e1-105">Create a new [externalGroupMember](../resources/externalconnectors-externalgroupmember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="569e1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="569e1-106">Permissions</span></span>

<span data-ttu-id="569e1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="569e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="569e1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="569e1-109">Permission type</span></span>                        | <span data-ttu-id="569e1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="569e1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="569e1-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="569e1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="569e1-112">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="569e1-112">Not supported</span></span>                               |
| <span data-ttu-id="569e1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="569e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="569e1-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="569e1-114">Not supported</span></span>                               |
| <span data-ttu-id="569e1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="569e1-115">Application</span></span>                            | <span data-ttu-id="569e1-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="569e1-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="569e1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="569e1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionsId}/groups/{externalGroupId}/members
```

## <a name="request-headers"></a><span data-ttu-id="569e1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="569e1-118">Request headers</span></span>

| <span data-ttu-id="569e1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="569e1-119">Name</span></span>          | <span data-ttu-id="569e1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="569e1-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="569e1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="569e1-121">Authorization</span></span> | <span data-ttu-id="569e1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="569e1-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="569e1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="569e1-124">Content-Type</span></span>  | <span data-ttu-id="569e1-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="569e1-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="569e1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="569e1-127">Request body</span></span>

<span data-ttu-id="569e1-128">No corpo da solicitação, fornece uma representação JSON do [objeto externalGroupMember.](../resources/externalconnectors-externalgroupmember.md)</span><span class="sxs-lookup"><span data-stu-id="569e1-128">In the request body, supply a JSON representation of the [externalGroupMember](../resources/externalconnectors-externalgroupmember.md) object.</span></span>

<span data-ttu-id="569e1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [externalGroupMember](../resources/externalconnectors-externalgroupmember.md).</span><span class="sxs-lookup"><span data-stu-id="569e1-129">The following table shows the properties that are required when you create the [externalGroupMember](../resources/externalconnectors-externalgroupmember.md).</span></span>

| <span data-ttu-id="569e1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="569e1-130">Property</span></span>       | <span data-ttu-id="569e1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="569e1-131">Type</span></span>                    | <span data-ttu-id="569e1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="569e1-132">Description</span></span>                                              |
|:---------------|:------------------------|:---------------------------------------------------------|
| <span data-ttu-id="569e1-133">id</span><span class="sxs-lookup"><span data-stu-id="569e1-133">id</span></span>             | <span data-ttu-id="569e1-134">String</span><span class="sxs-lookup"><span data-stu-id="569e1-134">String</span></span>                  | <span data-ttu-id="569e1-135">O exclusivo `id` do membro.</span><span class="sxs-lookup"><span data-stu-id="569e1-135">The unique `id` of the member.</span></span> <span data-ttu-id="569e1-136">Seria o objectId no caso de Azure Active Directory ou grupos e externalGroupId no caso de grupos externos.</span><span class="sxs-lookup"><span data-stu-id="569e1-136">It would be the objectId in case of Azure Active Directory users or groups and the externalGroupId in case of external groups.</span></span>                                    |
| <span data-ttu-id="569e1-137">tipo</span><span class="sxs-lookup"><span data-stu-id="569e1-137">type</span></span>           | <span data-ttu-id="569e1-138">microsoft.graph.externalConnectors.externalGroupMemberType</span><span class="sxs-lookup"><span data-stu-id="569e1-138">microsoft.graph.externalConnectors.externalGroupMemberType</span></span> | <span data-ttu-id="569e1-139">O tipo de membro adicionado ao grupo externo.</span><span class="sxs-lookup"><span data-stu-id="569e1-139">The type of member added to the external group.</span></span> <span data-ttu-id="569e1-140">Os valores possíveis são: `user` `group` ou quando identitySource é `azureActiveDirectory` e apenas quando `group` identitySource é `external` .</span><span class="sxs-lookup"><span data-stu-id="569e1-140">Possible values are: `user` or `group` when the identitySource is `azureActiveDirectory` and just `group` when the identitySource is `external`.</span></span> |
| <span data-ttu-id="569e1-141">identitySource</span><span class="sxs-lookup"><span data-stu-id="569e1-141">identitySource</span></span> | <span data-ttu-id="569e1-142">microsoft.graph.externalConnectors.identitySourceType</span><span class="sxs-lookup"><span data-stu-id="569e1-142">microsoft.graph.externalConnectors.identitySourceType</span></span>      | <span data-ttu-id="569e1-143">A fonte de identidade à que o membro pertence.</span><span class="sxs-lookup"><span data-stu-id="569e1-143">The identity source that the member belongs to.</span></span> <span data-ttu-id="569e1-144">Os valores possíveis são: `azureActiveDirectory` e `external`.</span><span class="sxs-lookup"><span data-stu-id="569e1-144">Possible values are: `azureActiveDirectory`, `external`.</span></span>                                                                                         |

## <a name="response"></a><span data-ttu-id="569e1-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="569e1-145">Response</span></span>

<span data-ttu-id="569e1-146">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto externalGroupMember](../resources/externalconnectors-externalgroupmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="569e1-146">If successful, this method returns a `201 Created` response code and an [externalGroupMember](../resources/externalconnectors-externalgroupmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="569e1-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="569e1-147">Examples</span></span>

### <a name="example-1-add-an-azure-active-directory-user-as-a-member"></a><span data-ttu-id="569e1-148">Exemplo 1: Adicionar um usuário Azure Active Directory como membro</span><span class="sxs-lookup"><span data-stu-id="569e1-148">Example 1: Add an Azure Active Directory user as a member</span></span>

### <a name="request"></a><span data-ttu-id="569e1-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="569e1-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="569e1-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="569e1-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from__1"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user",
  "identitySource": "azureActiveDirectory"
}
```
# <a name="c"></a>[<span data-ttu-id="569e1-151">C#</span><span class="sxs-lookup"><span data-stu-id="569e1-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroupmember-from--1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="569e1-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="569e1-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroupmember-from--1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="569e1-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="569e1-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroupmember-from--1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="569e1-154">Java</span><span class="sxs-lookup"><span data-stu-id="569e1-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalgroupmember-from--1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="569e1-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="569e1-155">Response</span></span>

<span data-ttu-id="569e1-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="569e1-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="example-2-add-an-azure-active-directory-group-as-a-member"></a><span data-ttu-id="569e1-157">Exemplo 2: Adicionar um grupo Azure Active Directory como membro</span><span class="sxs-lookup"><span data-stu-id="569e1-157">Example 2: Add an Azure Active Directory group as a member</span></span>

### <a name="request"></a><span data-ttu-id="569e1-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="569e1-158">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="569e1-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="569e1-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from__2"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group",
  "identitySource": "azureActiveDirectory"
}
```
# <a name="c"></a>[<span data-ttu-id="569e1-160">C#</span><span class="sxs-lookup"><span data-stu-id="569e1-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroupmember-from--2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="569e1-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="569e1-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroupmember-from--2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="569e1-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="569e1-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroupmember-from--2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="569e1-163">Java</span><span class="sxs-lookup"><span data-stu-id="569e1-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalgroupmember-from--2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="569e1-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="569e1-164">Response</span></span>

<span data-ttu-id="569e1-165">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="569e1-165">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="example-3-add-another-external-group-as-a-member"></a><span data-ttu-id="569e1-166">Exemplo 3: Adicionar outro grupo externo como membro</span><span class="sxs-lookup"><span data-stu-id="569e1-166">Example 3: Add another external group as a member</span></span>

### <a name="request"></a><span data-ttu-id="569e1-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="569e1-167">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="569e1-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="569e1-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from__3"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "id": "1431b9c38ee647f6a",
  "type": "group",
  "identitySource": "external"
}
```
# <a name="c"></a>[<span data-ttu-id="569e1-169">C#</span><span class="sxs-lookup"><span data-stu-id="569e1-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroupmember-from--3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="569e1-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="569e1-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroupmember-from--3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="569e1-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="569e1-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroupmember-from--3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="569e1-172">Java</span><span class="sxs-lookup"><span data-stu-id="569e1-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalgroupmember-from--3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="569e1-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="569e1-173">Response</span></span>

<span data-ttu-id="569e1-174">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="569e1-174">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "14m1b9c38qe647f6a",
  "type": "group",
  "identitySource": "external"
}
```
