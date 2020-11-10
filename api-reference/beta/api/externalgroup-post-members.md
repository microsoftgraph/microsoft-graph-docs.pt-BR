---
title: Criar externalGroupMember
description: Criar um novo objeto externalGroupMember.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b6c1d278fed4d32ac61afb7989c27d16e3fb275c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954619"
---
# <a name="create-externalgroupmember"></a><span data-ttu-id="dac3f-103">Criar externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="dac3f-103">Create externalGroupMember</span></span>

<span data-ttu-id="dac3f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dac3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dac3f-105">Criar um novo objeto [externalGroupMember](../resources/externalgroupmember.md) .</span><span class="sxs-lookup"><span data-stu-id="dac3f-105">Create a new [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dac3f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dac3f-106">Permissions</span></span>

<span data-ttu-id="dac3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dac3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dac3f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dac3f-109">Permission type</span></span>                        | <span data-ttu-id="dac3f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dac3f-110">Permissions (from most to least privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dac3f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dac3f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dac3f-112">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dac3f-112">Not supported</span></span>                               |
| <span data-ttu-id="dac3f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dac3f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dac3f-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dac3f-114">Not supported</span></span>                               |
| <span data-ttu-id="dac3f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dac3f-115">Application</span></span>                            | <span data-ttu-id="dac3f-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dac3f-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="dac3f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dac3f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionsId}/groups/{externalGroupId}/members
```

## <a name="request-headers"></a><span data-ttu-id="dac3f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dac3f-118">Request headers</span></span>

| <span data-ttu-id="dac3f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dac3f-119">Name</span></span>          | <span data-ttu-id="dac3f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dac3f-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="dac3f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dac3f-121">Authorization</span></span> | <span data-ttu-id="dac3f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dac3f-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="dac3f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dac3f-124">Content-Type</span></span>  | <span data-ttu-id="dac3f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dac3f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dac3f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dac3f-127">Request body</span></span>

<span data-ttu-id="dac3f-128">No corpo da solicitação, forneça uma representação JSON do objeto [externalGroupMember](../resources/externalgroupmember.md) .</span><span class="sxs-lookup"><span data-stu-id="dac3f-128">In the request body, supply a JSON representation of the [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

<span data-ttu-id="dac3f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [externalGroupMember](../resources/externalgroupmember.md).</span><span class="sxs-lookup"><span data-stu-id="dac3f-129">The following table shows the properties that are required when you create the [externalGroupMember](../resources/externalgroupmember.md).</span></span>

| <span data-ttu-id="dac3f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dac3f-130">Property</span></span>       | <span data-ttu-id="dac3f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dac3f-131">Type</span></span>                    | <span data-ttu-id="dac3f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dac3f-132">Description</span></span>                                              |
|:---------------|:------------------------|:---------------------------------------------------------|
| <span data-ttu-id="dac3f-133">id</span><span class="sxs-lookup"><span data-stu-id="dac3f-133">id</span></span>             | <span data-ttu-id="dac3f-134">String</span><span class="sxs-lookup"><span data-stu-id="dac3f-134">String</span></span>                  | <span data-ttu-id="dac3f-135">O exclusivo `id` do membro.</span><span class="sxs-lookup"><span data-stu-id="dac3f-135">The unique `id` of the member.</span></span> <span data-ttu-id="dac3f-136">Seria o objectId em caso de usuários ou grupos do Azure Active Directory e o externalGroupId no caso de grupos externos.</span><span class="sxs-lookup"><span data-stu-id="dac3f-136">It would be the objectId in case of Azure Active Directory users or groups and the externalGroupId in case of external groups.</span></span>                                    |
| <span data-ttu-id="dac3f-137">tipo</span><span class="sxs-lookup"><span data-stu-id="dac3f-137">type</span></span>           | <span data-ttu-id="dac3f-138">externalGroupMemberType</span><span class="sxs-lookup"><span data-stu-id="dac3f-138">externalGroupMemberType</span></span> | <span data-ttu-id="dac3f-139">O tipo de membro adicionado ao grupo externo.</span><span class="sxs-lookup"><span data-stu-id="dac3f-139">The type of member added to the external group.</span></span> <span data-ttu-id="dac3f-140">Os valores possíveis são: `user` ou `group` quando IdentityName é `azureActiveDirectory` e apenas `group` quando IdentityName é `external` .</span><span class="sxs-lookup"><span data-stu-id="dac3f-140">Possible values are: `user` or `group` when the identitySource is `azureActiveDirectory` and just `group` when the identitySource is `external`.</span></span> |
| <span data-ttu-id="dac3f-141">identificação da identidade</span><span class="sxs-lookup"><span data-stu-id="dac3f-141">identitySource</span></span> | <span data-ttu-id="dac3f-142">identitySourceType</span><span class="sxs-lookup"><span data-stu-id="dac3f-142">identitySourceType</span></span>      | <span data-ttu-id="dac3f-143">A origem de identidade à qual o membro pertence.</span><span class="sxs-lookup"><span data-stu-id="dac3f-143">The identity source that the member belongs to.</span></span> <span data-ttu-id="dac3f-144">Os valores possíveis são: `azureActiveDirectory` e `external`.</span><span class="sxs-lookup"><span data-stu-id="dac3f-144">Possible values are: `azureActiveDirectory`, `external`.</span></span>                                                                                         |

## <a name="response"></a><span data-ttu-id="dac3f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="dac3f-145">Response</span></span>

<span data-ttu-id="dac3f-146">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [externalGroupMember](../resources/externalgroupmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dac3f-146">If successful, this method returns a `201 Created` response code and an [externalGroupMember](../resources/externalgroupmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dac3f-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dac3f-147">Examples</span></span>

### <a name="example-1-add-an-azure-active-directory-user-as-a-member"></a><span data-ttu-id="dac3f-148">Exemplo 1: adicionar um usuário do Azure Active Directory como membro</span><span class="sxs-lookup"><span data-stu-id="dac3f-148">Example 1: Add an Azure Active Directory user as a member</span></span>

### <a name="request"></a><span data-ttu-id="dac3f-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dac3f-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dac3f-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="dac3f-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user",
  "identitySource": "azureActiveDirectory"
}
```
# <a name="c"></a>[<span data-ttu-id="dac3f-151">C#</span><span class="sxs-lookup"><span data-stu-id="dac3f-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroupmember-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dac3f-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dac3f-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroupmember-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dac3f-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dac3f-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroupmember-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dac3f-154">Java</span><span class="sxs-lookup"><span data-stu-id="dac3f-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalgroupmember-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="dac3f-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="dac3f-155">Response</span></span>

<span data-ttu-id="dac3f-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dac3f-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="example-2-add-an-azure-active-directory-group-as-a-member"></a><span data-ttu-id="dac3f-157">Exemplo 2: adicionar um grupo do Azure Active Directory como membro</span><span class="sxs-lookup"><span data-stu-id="dac3f-157">Example 2: Add an Azure Active Directory group as a member</span></span>

### <a name="request"></a><span data-ttu-id="dac3f-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dac3f-158">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="response"></a><span data-ttu-id="dac3f-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="dac3f-159">Response</span></span>

<span data-ttu-id="dac3f-160">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dac3f-160">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="example-3-add-another-external-group-as-a-member"></a><span data-ttu-id="dac3f-161">Exemplo 3: adicionar outro grupo externo como membro</span><span class="sxs-lookup"><span data-stu-id="dac3f-161">Example 3: Add another external group as a member</span></span>

### <a name="request"></a><span data-ttu-id="dac3f-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dac3f-162">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "1431b9c38ee647f6a",
  "type": "group",
  "identitySource": "external"
}
```

### <a name="response"></a><span data-ttu-id="dac3f-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="dac3f-163">Response</span></span>

<span data-ttu-id="dac3f-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dac3f-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "14m1b9c38qe647f6a",
  "type": "group",
  "identitySource": "external"
}
```
