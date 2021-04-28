---
title: 'group: assignLicense'
description: Adicione ou remova licenças no grupo. As licenças atribuídas ao grupo serão atribuídas a todos os usuários do grupo.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e78e9bdcd2cc0383251a7fe6fde2b38aedee2a80
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035474"
---
# <a name="group-assignlicense"></a><span data-ttu-id="40ea3-104">group: assignLicense</span><span class="sxs-lookup"><span data-stu-id="40ea3-104">group: assignLicense</span></span>

<span data-ttu-id="40ea3-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40ea3-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="40ea3-106">Adicione ou remova licenças no grupo.</span><span class="sxs-lookup"><span data-stu-id="40ea3-106">Add or remove licenses on the group.</span></span> <span data-ttu-id="40ea3-107">As licenças atribuídas ao grupo serão atribuídas a todos os usuários do grupo.</span><span class="sxs-lookup"><span data-stu-id="40ea3-107">Licenses assigned to the group will be assigned to all users in the group.</span></span> <span data-ttu-id="40ea3-108">Para saber mais sobre o licenciamento baseado em grupo, consulte O que é licenciamento baseado em [grupo em Azure Active Directory](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="40ea3-108">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span>

<span data-ttu-id="40ea3-109">Para obter as assinaturas disponíveis no diretório, execute uma [solicitação GET subscribedSkus](../resources/subscribedsku.md).</span><span class="sxs-lookup"><span data-stu-id="40ea3-109">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](../resources/subscribedsku.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="40ea3-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="40ea3-110">Permissions</span></span>
<span data-ttu-id="40ea3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40ea3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40ea3-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40ea3-113">Permission type</span></span>      | <span data-ttu-id="40ea3-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40ea3-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40ea3-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40ea3-115">Delegated (work or school account)</span></span> | <span data-ttu-id="40ea3-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40ea3-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="40ea3-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40ea3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40ea3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40ea3-118">Not supported.</span></span>    |
|<span data-ttu-id="40ea3-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40ea3-119">Application</span></span> | <span data-ttu-id="40ea3-120">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40ea3-120">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40ea3-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40ea3-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="40ea3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40ea3-122">Request headers</span></span>
| <span data-ttu-id="40ea3-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40ea3-123">Header</span></span>       | <span data-ttu-id="40ea3-124">Valor</span><span class="sxs-lookup"><span data-stu-id="40ea3-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="40ea3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="40ea3-125">Authorization</span></span>  | <span data-ttu-id="40ea3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40ea3-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="40ea3-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40ea3-128">Content-Type</span></span>  | <span data-ttu-id="40ea3-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40ea3-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="40ea3-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40ea3-131">Request body</span></span>
<span data-ttu-id="40ea3-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40ea3-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="40ea3-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="40ea3-133">Parameter</span></span>    | <span data-ttu-id="40ea3-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="40ea3-134">Type</span></span>   |<span data-ttu-id="40ea3-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="40ea3-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40ea3-136">addLicenses</span><span class="sxs-lookup"><span data-stu-id="40ea3-136">addLicenses</span></span>|<span data-ttu-id="40ea3-137">Coleção [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="40ea3-137">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="40ea3-138">Uma coleção de objetos [assignedLicense](../resources/assignedlicense.md) que especifica as licenças a adicionar.</span><span class="sxs-lookup"><span data-stu-id="40ea3-138">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="40ea3-139">Você pode desabilitar servicePlans associado a uma licença definindo a propriedade **disabledPlans** em [um objeto assignedLicense.](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="40ea3-139">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="40ea3-140">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="40ea3-140">removeLicenses</span></span>|<span data-ttu-id="40ea3-141">Coleção GUID</span><span class="sxs-lookup"><span data-stu-id="40ea3-141">GUID collection</span></span>|<span data-ttu-id="40ea3-142">Uma coleção de skuIds que identificam as licenças a remover.</span><span class="sxs-lookup"><span data-stu-id="40ea3-142">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="40ea3-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="40ea3-143">Response</span></span>

<span data-ttu-id="40ea3-144">Se tiver êxito, este método retornará `202 Accepted` um código de resposta e um objeto [de](../resources/group.md) grupo de destino no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40ea3-144">If successful, this method returns a `202 Accepted` response code and a target [group](../resources/group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="40ea3-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="40ea3-145">Examples</span></span>

### <a name="example-1-add-licenses-to-the-group"></a><span data-ttu-id="40ea3-146">Exemplo 1: Adicionar licenças ao grupo</span><span class="sxs-lookup"><span data-stu-id="40ea3-146">Example 1: Add licenses to the group</span></span>
<span data-ttu-id="40ea3-147">O exemplo a seguir adiciona licenças ao grupo.</span><span class="sxs-lookup"><span data-stu-id="40ea3-147">The following example adds licenses to the group.</span></span>
#### <a name="request"></a><span data-ttu-id="40ea3-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40ea3-148">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="40ea3-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="40ea3-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="40ea3-150">C#</span><span class="sxs-lookup"><span data-stu-id="40ea3-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40ea3-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40ea3-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40ea3-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40ea3-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40ea3-153">Java</span><span class="sxs-lookup"><span data-stu-id="40ea3-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-assignlicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="40ea3-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="40ea3-154">Response</span></span>

<span data-ttu-id="40ea3-155">A resposta é o objeto de grupo atualizado.</span><span class="sxs-lookup"><span data-stu-id="40ea3-155">The response is the updated group object.</span></span>

><span data-ttu-id="40ea3-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="40ea3-156">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-remove-licenses-from-the-group"></a><span data-ttu-id="40ea3-157">Exemplo 2: Remover licenças do grupo</span><span class="sxs-lookup"><span data-stu-id="40ea3-157">Example 2: Remove licenses from the group</span></span>
<span data-ttu-id="40ea3-158">O exemplo a seguir remove licenças do grupo.</span><span class="sxs-lookup"><span data-stu-id="40ea3-158">The following example removes licenses from the group.</span></span>

#### <a name="request"></a><span data-ttu-id="40ea3-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40ea3-159">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="40ea3-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="40ea3-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="40ea3-161">C#</span><span class="sxs-lookup"><span data-stu-id="40ea3-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removelicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40ea3-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40ea3-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removelicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40ea3-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40ea3-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removelicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40ea3-164">Java</span><span class="sxs-lookup"><span data-stu-id="40ea3-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-removelicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="40ea3-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="40ea3-165">Response</span></span>

<span data-ttu-id="40ea3-166">A resposta é o objeto de grupo atualizado.</span><span class="sxs-lookup"><span data-stu-id="40ea3-166">The response is the updated group object.</span></span>

><span data-ttu-id="40ea3-167">**Observação:** O objeto de resposta mostrado aqui pode ser reduzido para a capacidade de leitura..</span><span class="sxs-lookup"><span data-stu-id="40ea3-167">**Note:** The response object shown here might be shortened for readability..</span></span>
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

