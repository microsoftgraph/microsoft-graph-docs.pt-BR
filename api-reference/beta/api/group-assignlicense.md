---
title: 'Grupo: assignLicense'
description: Adicionar ou remover licenças no grupo. As licenças atribuídas ao grupo serão atribuídas a todos os usuários do grupo.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1d014be80c99a6f9c39b0dc67f65a5b940c8cd67
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535573"
---
# <a name="group-assignlicense"></a><span data-ttu-id="7a3ef-104">Grupo: assignLicense</span><span class="sxs-lookup"><span data-stu-id="7a3ef-104">group: assignLicense</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a3ef-105">Adicionar ou remover licenças no grupo.</span><span class="sxs-lookup"><span data-stu-id="7a3ef-105">Add or remove licenses on the group.</span></span> <span data-ttu-id="7a3ef-106">As licenças atribuídas ao grupo serão atribuídas a todos os usuários do grupo.</span><span class="sxs-lookup"><span data-stu-id="7a3ef-106">Licenses assigned to the group will be assigned to all users in the group.</span></span> <span data-ttu-id="7a3ef-107">Para saber mais sobre licenciamento baseado em grupo, confira [o que é licenciamento baseado em grupo no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="7a3ef-107">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span>

<span data-ttu-id="7a3ef-108">Para obter as assinaturas disponíveis no diretório, execute uma [solicitação get subscribedSkus](subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="7a3ef-108">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7a3ef-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a3ef-109">Permissions</span></span>
<span data-ttu-id="7a3ef-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a3ef-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a3ef-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a3ef-112">Permission type</span></span>      | <span data-ttu-id="7a3ef-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a3ef-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a3ef-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a3ef-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7a3ef-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a3ef-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="7a3ef-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a3ef-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a3ef-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a3ef-117">Not supported.</span></span>    |
|<span data-ttu-id="7a3ef-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a3ef-118">Application</span></span> | <span data-ttu-id="7a3ef-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a3ef-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a3ef-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a3ef-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="7a3ef-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a3ef-121">Request headers</span></span>
| <span data-ttu-id="7a3ef-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7a3ef-122">Header</span></span>       | <span data-ttu-id="7a3ef-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7a3ef-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7a3ef-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a3ef-124">Authorization</span></span>  | <span data-ttu-id="7a3ef-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a3ef-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7a3ef-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7a3ef-127">Content-Type</span></span>  | <span data-ttu-id="7a3ef-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a3ef-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7a3ef-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a3ef-130">Request body</span></span>
<span data-ttu-id="7a3ef-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a3ef-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7a3ef-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7a3ef-132">Parameter</span></span>    | <span data-ttu-id="7a3ef-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a3ef-133">Type</span></span>   |<span data-ttu-id="7a3ef-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a3ef-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a3ef-135">addLicenses</span><span class="sxs-lookup"><span data-stu-id="7a3ef-135">addLicenses</span></span>|<span data-ttu-id="7a3ef-136">Coleção [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="7a3ef-136">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="7a3ef-137">Uma coleção de objetos [assignedLicense](../resources/assignedlicense.md) que especifica as licenças a adicionar.</span><span class="sxs-lookup"><span data-stu-id="7a3ef-137">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="7a3ef-138">Você pode desabilitar o onplans associado a uma licença definindo a propriedade **disabledPlans** em um objeto [assignedLicense](../resources/assignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="7a3ef-138">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="7a3ef-139">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="7a3ef-139">removeLicenses</span></span>|<span data-ttu-id="7a3ef-140">Coleção GUID</span><span class="sxs-lookup"><span data-stu-id="7a3ef-140">GUID collection</span></span>|<span data-ttu-id="7a3ef-141">Uma coleção de skuIds que identifica as licenças a serem removidas.</span><span class="sxs-lookup"><span data-stu-id="7a3ef-141">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="7a3ef-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a3ef-142">Response</span></span>

<span data-ttu-id="7a3ef-143">Se tiver êxito, este método retornará `202 Accepted` um código de resposta e um objeto de [grupo](../resources/group.md) de destino no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a3ef-143">If successful, this method returns a `202 Accepted` response code and a target [group](../resources/group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7a3ef-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7a3ef-144">Examples</span></span>

### <a name="example-1-add-licenses-to-the-group"></a><span data-ttu-id="7a3ef-145">Exemplo 1: adicionar licenças ao grupo</span><span class="sxs-lookup"><span data-stu-id="7a3ef-145">Example 1: Add licenses to the group</span></span>
<span data-ttu-id="7a3ef-146">O exemplo a seguir adiciona licenças ao grupo.</span><span class="sxs-lookup"><span data-stu-id="7a3ef-146">The following example adds licenses to the group.</span></span>
#### <a name="request"></a><span data-ttu-id="7a3ef-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a3ef-147">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7a3ef-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a3ef-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_assignlicense"
}-->
```http
POST https://graph.microsoft.com/beta/groups/1ad75eeb-7e5a-4367-a493-9214d90d54d0/assignLicense
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7a3ef-149">C#</span><span class="sxs-lookup"><span data-stu-id="7a3ef-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a3ef-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a3ef-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7a3ef-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a3ef-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7a3ef-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a3ef-152">Response</span></span>
<span data-ttu-id="7a3ef-153">A resposta é o objeto de grupo atualizado.</span><span class="sxs-lookup"><span data-stu-id="7a3ef-153">The response is the updated group object.</span></span>

><span data-ttu-id="7a3ef-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7a3ef-154">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7a3ef-155">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a3ef-155">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-remove-licenses-from-the-group"></a><span data-ttu-id="7a3ef-156">Exemplo 2: remover licenças do grupo</span><span class="sxs-lookup"><span data-stu-id="7a3ef-156">Example 2: Remove licenses from the group</span></span>
<span data-ttu-id="7a3ef-157">O exemplo a seguir remove licenças do grupo.</span><span class="sxs-lookup"><span data-stu-id="7a3ef-157">The following example removes licenses from the group.</span></span>

#### <a name="request"></a><span data-ttu-id="7a3ef-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a3ef-158">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7a3ef-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a3ef-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_removelicense"
}-->

```http
POST https://graph.microsoft.com/beta/groups/1ad75eeb-7e5a-4367-a493-9214d90d54d0/assignLicense
Content-type: application/json


{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7a3ef-160">C#</span><span class="sxs-lookup"><span data-stu-id="7a3ef-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removelicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a3ef-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a3ef-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removelicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7a3ef-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a3ef-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removelicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7a3ef-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a3ef-163">Response</span></span>
<span data-ttu-id="7a3ef-164">A resposta é o objeto de grupo atualizado.</span><span class="sxs-lookup"><span data-stu-id="7a3ef-164">The response is the updated group object.</span></span>

><span data-ttu-id="7a3ef-165">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7a3ef-165">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7a3ef-166">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a3ef-166">All the properties will be returned from an actual call..</span></span>
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
