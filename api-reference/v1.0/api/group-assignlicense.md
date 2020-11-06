---
title: 'Grupo: assignLicense'
description: Adicionar ou remover licenças no grupo. As licenças atribuídas ao grupo serão atribuídas a todos os usuários do grupo.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5e36b6507f49444c4bd6a5433544c9f5976b4379
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921757"
---
# <a name="group-assignlicense"></a><span data-ttu-id="72d08-104">Grupo: assignLicense</span><span class="sxs-lookup"><span data-stu-id="72d08-104">group: assignLicense</span></span>

<span data-ttu-id="72d08-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72d08-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="72d08-106">Adicionar ou remover licenças no grupo.</span><span class="sxs-lookup"><span data-stu-id="72d08-106">Add or remove licenses on the group.</span></span> <span data-ttu-id="72d08-107">As licenças atribuídas ao grupo serão atribuídas a todos os usuários do grupo.</span><span class="sxs-lookup"><span data-stu-id="72d08-107">Licenses assigned to the group will be assigned to all users in the group.</span></span> <span data-ttu-id="72d08-108">Para saber mais sobre licenciamento baseado em grupo, confira [o que é licenciamento baseado em grupo no Azure Active Directory](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="72d08-108">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span>

<span data-ttu-id="72d08-109">Para obter as assinaturas disponíveis no diretório, execute uma [solicitação get subscribedSkus](../resources/subscribedsku.md).</span><span class="sxs-lookup"><span data-stu-id="72d08-109">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](../resources/subscribedsku.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="72d08-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="72d08-110">Permissions</span></span>
<span data-ttu-id="72d08-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72d08-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72d08-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72d08-113">Permission type</span></span>      | <span data-ttu-id="72d08-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72d08-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72d08-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72d08-115">Delegated (work or school account)</span></span> | <span data-ttu-id="72d08-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72d08-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="72d08-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72d08-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72d08-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72d08-118">Not supported.</span></span>    |
|<span data-ttu-id="72d08-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72d08-119">Application</span></span> | <span data-ttu-id="72d08-120">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72d08-120">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="72d08-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72d08-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="72d08-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72d08-122">Request headers</span></span>
| <span data-ttu-id="72d08-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72d08-123">Header</span></span>       | <span data-ttu-id="72d08-124">Valor</span><span class="sxs-lookup"><span data-stu-id="72d08-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="72d08-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="72d08-125">Authorization</span></span>  | <span data-ttu-id="72d08-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72d08-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="72d08-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72d08-128">Content-Type</span></span>  | <span data-ttu-id="72d08-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72d08-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="72d08-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72d08-131">Request body</span></span>
<span data-ttu-id="72d08-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72d08-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="72d08-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="72d08-133">Parameter</span></span>    | <span data-ttu-id="72d08-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="72d08-134">Type</span></span>   |<span data-ttu-id="72d08-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="72d08-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72d08-136">addLicenses</span><span class="sxs-lookup"><span data-stu-id="72d08-136">addLicenses</span></span>|<span data-ttu-id="72d08-137">Coleção [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="72d08-137">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="72d08-138">Uma coleção de objetos [assignedLicense](../resources/assignedlicense.md) que especifica as licenças a adicionar.</span><span class="sxs-lookup"><span data-stu-id="72d08-138">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="72d08-139">Você pode desabilitar o onplans associado a uma licença definindo a propriedade **disabledPlans** em um objeto [assignedLicense](../resources/assignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="72d08-139">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="72d08-140">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="72d08-140">removeLicenses</span></span>|<span data-ttu-id="72d08-141">Coleção GUID</span><span class="sxs-lookup"><span data-stu-id="72d08-141">GUID collection</span></span>|<span data-ttu-id="72d08-142">Uma coleção de skuIds que identifica as licenças a serem removidas.</span><span class="sxs-lookup"><span data-stu-id="72d08-142">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="72d08-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="72d08-143">Response</span></span>

<span data-ttu-id="72d08-144">Se tiver êxito, este método retornará um `202 Accepted` código de resposta e um objeto de [grupo](../resources/group.md) de destino no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72d08-144">If successful, this method returns a `202 Accepted` response code and a target [group](../resources/group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72d08-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="72d08-145">Examples</span></span>

### <a name="example-1-add-licenses-to-the-group"></a><span data-ttu-id="72d08-146">Exemplo 1: adicionar licenças ao grupo</span><span class="sxs-lookup"><span data-stu-id="72d08-146">Example 1: Add licenses to the group</span></span>
<span data-ttu-id="72d08-147">O exemplo a seguir adiciona licenças ao grupo.</span><span class="sxs-lookup"><span data-stu-id="72d08-147">The following example adds licenses to the group.</span></span>
#### <a name="request"></a><span data-ttu-id="72d08-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72d08-148">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="72d08-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="72d08-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_assignlicense"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/1ad75eeb-7e5a-4367-a493-9214d90d54d0/assignLicense
Content-type: application/json


{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value-1"
    },
    {
      "disabledPlans": [ "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235" ],
      "skuId": "skuId-value-2"
    }
  ],
  "removeLicenses": []
}
```
# <a name="c"></a>[<span data-ttu-id="72d08-150">C#</span><span class="sxs-lookup"><span data-stu-id="72d08-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72d08-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72d08-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72d08-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72d08-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72d08-153">Java</span><span class="sxs-lookup"><span data-stu-id="72d08-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-assignlicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="72d08-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="72d08-154">Response</span></span>

<span data-ttu-id="72d08-155">A resposta é o objeto de grupo atualizado.</span><span class="sxs-lookup"><span data-stu-id="72d08-155">The response is the updated group object.</span></span>

><span data-ttu-id="72d08-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="72d08-156">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="72d08-157">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72d08-157">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 202 Accepted
Content-type: application/json
location: https://graph.microsoft.com/v2/d056d009-17b3-4106-8173-cd3978ada898/directoryObjects/1ad75eeb-7e5a-4367-a493-9214d90d54d0/Microsoft.DirectoryServices.Group

{
  "id": "1ad75eeb-7e5a-4367-a493-9214d90d54d0",
  "deletedDateTime": null,
  "classification": null,
  "createdDateTime": "2018-04-18T22:05:03Z",
  "securityEnabled": true,

}
```

### <a name="example-2-remove-licenses-from-the-group"></a><span data-ttu-id="72d08-158">Exemplo 2: remover licenças do grupo</span><span class="sxs-lookup"><span data-stu-id="72d08-158">Example 2: Remove licenses from the group</span></span>
<span data-ttu-id="72d08-159">O exemplo a seguir remove licenças do grupo.</span><span class="sxs-lookup"><span data-stu-id="72d08-159">The following example removes licenses from the group.</span></span>

#### <a name="request"></a><span data-ttu-id="72d08-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72d08-160">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="72d08-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="72d08-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_removelicense"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/1ad75eeb-7e5a-4367-a493-9214d90d54d0/assignLicense
Content-type: application/json


{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```
# <a name="c"></a>[<span data-ttu-id="72d08-162">C#</span><span class="sxs-lookup"><span data-stu-id="72d08-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removelicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72d08-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72d08-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removelicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72d08-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72d08-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removelicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72d08-165">Java</span><span class="sxs-lookup"><span data-stu-id="72d08-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-removelicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="72d08-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="72d08-166">Response</span></span>

<span data-ttu-id="72d08-167">A resposta é o objeto de grupo atualizado.</span><span class="sxs-lookup"><span data-stu-id="72d08-167">The response is the updated group object.</span></span>

><span data-ttu-id="72d08-168">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="72d08-168">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="72d08-169">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72d08-169">All the properties will be returned from an actual call..</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 202 Accepted
Content-type: application/json
location: https://graph.microsoft.com/v2/d056d009-17b3-4106-8173-cd3978ada898/directoryObjects/1ad75eeb-7e5a-4367-a493-9214d90d54d0/Microsoft.DirectoryServices.Group


{
  "id": "1ad75eeb-7e5a-4367-a493-9214d90d54d0",
  "deletedDateTime": null,
  "classification": null,
  "createdDateTime": "2018-04-18T22:05:03Z",
  "securityEnabled": true,

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

