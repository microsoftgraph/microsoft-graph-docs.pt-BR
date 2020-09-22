---
title: Criar externalGroupMember
description: Criar um novo objeto externalGroupMember.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c66c21e4b0842df4fb7ececa3378249347f3002d
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193814"
---
# <a name="create-externalgroupmember"></a><span data-ttu-id="e211c-103">Criar externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="e211c-103">Create externalGroupMember</span></span>

<span data-ttu-id="e211c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e211c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e211c-105">Criar um novo objeto [externalGroupMember](../resources/externalgroupmember.md) .</span><span class="sxs-lookup"><span data-stu-id="e211c-105">Create a new [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e211c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e211c-106">Permissions</span></span>

<span data-ttu-id="e211c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e211c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e211c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e211c-109">Permission type</span></span>                        | <span data-ttu-id="e211c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e211c-110">Permissions (from most to least privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e211c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e211c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e211c-112">Incompatível</span><span class="sxs-lookup"><span data-stu-id="e211c-112">Not supported</span></span>                               |
| <span data-ttu-id="e211c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e211c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e211c-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e211c-114">Not supported</span></span>                               |
| <span data-ttu-id="e211c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e211c-115">Application</span></span>                            | <span data-ttu-id="e211c-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e211c-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="e211c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e211c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionsId}/groups/{externalGroupId}/members
```

## <a name="request-headers"></a><span data-ttu-id="e211c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e211c-118">Request headers</span></span>

| <span data-ttu-id="e211c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e211c-119">Name</span></span>          | <span data-ttu-id="e211c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e211c-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="e211c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e211c-121">Authorization</span></span> | <span data-ttu-id="e211c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e211c-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e211c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e211c-124">Content-Type</span></span>  | <span data-ttu-id="e211c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e211c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e211c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e211c-127">Request body</span></span>

<span data-ttu-id="e211c-128">No corpo da solicitação, forneça uma representação JSON do objeto [externalGroupMember](../resources/externalgroupmember.md) .</span><span class="sxs-lookup"><span data-stu-id="e211c-128">In the request body, supply a JSON representation of the [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

<span data-ttu-id="e211c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [externalGroupMember](../resources/externalgroupmember.md).</span><span class="sxs-lookup"><span data-stu-id="e211c-129">The following table shows the properties that are required when you create the [externalGroupMember](../resources/externalgroupmember.md).</span></span>

| <span data-ttu-id="e211c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e211c-130">Property</span></span>       | <span data-ttu-id="e211c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e211c-131">Type</span></span>                    | <span data-ttu-id="e211c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e211c-132">Description</span></span>                                              |
|:---------------|:------------------------|:---------------------------------------------------------|
| <span data-ttu-id="e211c-133">id</span><span class="sxs-lookup"><span data-stu-id="e211c-133">id</span></span>             | <span data-ttu-id="e211c-134">String</span><span class="sxs-lookup"><span data-stu-id="e211c-134">String</span></span>                  | <span data-ttu-id="e211c-135">O exclusivo `id` do membro.</span><span class="sxs-lookup"><span data-stu-id="e211c-135">The unique `id` of the member.</span></span> <span data-ttu-id="e211c-136">Seria o objectId em caso de usuários ou grupos do Azure Active Directory e o externalGroupId no caso de grupos externos.</span><span class="sxs-lookup"><span data-stu-id="e211c-136">It would be the objectId in case of Azure Active Directory users or groups and the externalGroupId in case of external groups.</span></span>                                    |
| <span data-ttu-id="e211c-137">tipo</span><span class="sxs-lookup"><span data-stu-id="e211c-137">type</span></span>           | <span data-ttu-id="e211c-138">externalGroupMemberType</span><span class="sxs-lookup"><span data-stu-id="e211c-138">externalGroupMemberType</span></span> | <span data-ttu-id="e211c-139">O tipo de membro adicionado ao grupo externo.</span><span class="sxs-lookup"><span data-stu-id="e211c-139">The type of member added to the external group.</span></span> <span data-ttu-id="e211c-140">Os valores possíveis são: `user` ou `group` quando IdentityName é `azureActiveDirectory` e apenas `group` quando IdentityName é `external` .</span><span class="sxs-lookup"><span data-stu-id="e211c-140">Possible values are: `user` or `group` when the identitySource is `azureActiveDirectory` and just `group` when the identitySource is `external`.</span></span> |
| <span data-ttu-id="e211c-141">identificação da identidade</span><span class="sxs-lookup"><span data-stu-id="e211c-141">identitySource</span></span> | <span data-ttu-id="e211c-142">identitySourceType</span><span class="sxs-lookup"><span data-stu-id="e211c-142">identitySourceType</span></span>      | <span data-ttu-id="e211c-143">A origem de identidade à qual o membro pertence.</span><span class="sxs-lookup"><span data-stu-id="e211c-143">The identity source that the member belongs to.</span></span> <span data-ttu-id="e211c-144">Os valores possíveis são: `azureActiveDirectory` e `external`.</span><span class="sxs-lookup"><span data-stu-id="e211c-144">Possible values are: `azureActiveDirectory`, `external`.</span></span>                                                                                         |

## <a name="response"></a><span data-ttu-id="e211c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e211c-145">Response</span></span>

<span data-ttu-id="e211c-146">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [externalGroupMember](../resources/externalgroupmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e211c-146">If successful, this method returns a `201 Created` response code and an [externalGroupMember](../resources/externalgroupmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e211c-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e211c-147">Examples</span></span>

### <a name="example-1-add-an-azure-active-directory-user-as-a-member"></a><span data-ttu-id="e211c-148">Exemplo 1: adicionar um usuário do Azure Active Directory como membro</span><span class="sxs-lookup"><span data-stu-id="e211c-148">Example 1: Add an Azure Active Directory user as a member</span></span>

### <a name="request"></a><span data-ttu-id="e211c-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e211c-149">Request</span></span>

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

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="e211c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="e211c-150">Response</span></span>

<span data-ttu-id="e211c-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e211c-151">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-add-an-azure-active-directory-group-as-a-member"></a><span data-ttu-id="e211c-152">Exemplo 2: adicionar um grupo do Azure Active Directory como membro</span><span class="sxs-lookup"><span data-stu-id="e211c-152">Example 2: Add an Azure Active Directory group as a member</span></span>

### <a name="request"></a><span data-ttu-id="e211c-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e211c-153">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="e211c-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="e211c-154">Response</span></span>

<span data-ttu-id="e211c-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e211c-155">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-3-add-another-external-group-as-a-member"></a><span data-ttu-id="e211c-156">Exemplo 3: adicionar outro grupo externo como membro</span><span class="sxs-lookup"><span data-stu-id="e211c-156">Example 3: Add another external group as a member</span></span>

### <a name="request"></a><span data-ttu-id="e211c-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e211c-157">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="e211c-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="e211c-158">Response</span></span>

<span data-ttu-id="e211c-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e211c-159">**Note:** The response object shown here might be shortened for readability.</span></span>
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
