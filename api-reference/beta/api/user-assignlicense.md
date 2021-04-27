---
title: assignLicense
description: Adicione ou remova licenças para o usuário habilitar ou desabilitar o uso de ofertas de nuvem da Microsoft. Por exemplo, uma organização pode ter uma assinatura Microsoft 365 Enterprise E3 com 100 licenças e essa solicitação atribui uma dessas licenças a um usuário específico. Você também pode habilitar e desabilitar planos específicos associados a uma assinatura. Para saber mais sobre assinaturas e licenças, consulte este artigo do Technet.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 6efe1bf90e48677070d7aa5b1a7b4feb57a162d3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053388"
---
# <a name="user-assignlicense"></a><span data-ttu-id="95eb7-106">usuário: assignLicense</span><span class="sxs-lookup"><span data-stu-id="95eb7-106">user: assignLicense</span></span>

<span data-ttu-id="95eb7-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95eb7-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95eb7-108">Adicione ou remova licenças para o usuário habilitar ou desabilitar o uso de ofertas de nuvem da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="95eb7-108">Add or remove licenses for the user to enable or disable their use of Microsoft cloud offerings.</span></span> <span data-ttu-id="95eb7-109">Por exemplo, uma organização pode ter uma assinatura Microsoft 365 Enterprise E3 com 100 licenças e essa solicitação atribui uma dessas licenças a um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="95eb7-109">For example, an organization can have a Microsoft 365 Enterprise E3 subscription with 100 licenses, and this request assigns one of those licenses to a specific user.</span></span> <span data-ttu-id="95eb7-110">Você também pode habilitar e desabilitar planos específicos associados a uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="95eb7-110">You can also enable and disable specific plans associated with a subscription.</span></span> <span data-ttu-id="95eb7-111">Para saber mais sobre assinaturas e licenças, consulte este [artigo do Technet](/microsoft-365/enterprise/subscriptions-licenses-accounts-and-tenants-for-microsoft-cloud-offerings).</span><span class="sxs-lookup"><span data-stu-id="95eb7-111">To learn more about subscriptions and licenses, see this [Technet article](/microsoft-365/enterprise/subscriptions-licenses-accounts-and-tenants-for-microsoft-cloud-offerings).</span></span>

<span data-ttu-id="95eb7-112">Para obter as assinaturas disponíveis no diretório, execute uma [solicitação GET subscribedSkus](subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="95eb7-112">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="95eb7-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="95eb7-113">Permissions</span></span>
<span data-ttu-id="95eb7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95eb7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95eb7-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95eb7-116">Permission type</span></span>      | <span data-ttu-id="95eb7-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95eb7-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95eb7-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95eb7-118">Delegated (work or school account)</span></span> | <span data-ttu-id="95eb7-119">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95eb7-119">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="95eb7-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95eb7-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95eb7-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95eb7-121">Not supported.</span></span>    |
|<span data-ttu-id="95eb7-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95eb7-122">Application</span></span> | <span data-ttu-id="95eb7-123">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95eb7-123">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="95eb7-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95eb7-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="95eb7-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95eb7-125">Request headers</span></span>
| <span data-ttu-id="95eb7-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95eb7-126">Header</span></span>       | <span data-ttu-id="95eb7-127">Valor</span><span class="sxs-lookup"><span data-stu-id="95eb7-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="95eb7-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="95eb7-128">Authorization</span></span>  | <span data-ttu-id="95eb7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95eb7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="95eb7-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="95eb7-131">Content-Type</span></span>  | <span data-ttu-id="95eb7-132">application/json</span><span class="sxs-lookup"><span data-stu-id="95eb7-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="95eb7-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95eb7-133">Request body</span></span>
<span data-ttu-id="95eb7-134">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95eb7-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="95eb7-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="95eb7-135">Parameter</span></span>    | <span data-ttu-id="95eb7-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="95eb7-136">Type</span></span>   |<span data-ttu-id="95eb7-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="95eb7-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95eb7-138">addLicenses</span><span class="sxs-lookup"><span data-stu-id="95eb7-138">addLicenses</span></span>|<span data-ttu-id="95eb7-139">Coleção [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="95eb7-139">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="95eb7-140">Uma coleção de objetos [assignedLicense](../resources/assignedlicense.md) que especifica as licenças a adicionar.</span><span class="sxs-lookup"><span data-stu-id="95eb7-140">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="95eb7-141">Você pode desabilitar servicePlans associado a uma licença definindo a propriedade **disabledPlans** em [um objeto assignedLicense.](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="95eb7-141">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="95eb7-142">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="95eb7-142">removeLicenses</span></span>|<span data-ttu-id="95eb7-143">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="95eb7-143">Guid collection</span></span>|<span data-ttu-id="95eb7-144">Uma coleção de skuIds que identificam as licenças a remover.</span><span class="sxs-lookup"><span data-stu-id="95eb7-144">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="95eb7-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="95eb7-145">Response</span></span>

<span data-ttu-id="95eb7-146">Se tiver êxito, este método retornará `200 OK` o código de resposta e um objeto de [usuário](../resources/user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95eb7-146">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95eb7-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95eb7-147">Example</span></span>
<span data-ttu-id="95eb7-148">Adicione licenças ao usuário.</span><span class="sxs-lookup"><span data-stu-id="95eb7-148">Add licenses to the user.</span></span>
##### <a name="request"></a><span data-ttu-id="95eb7-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95eb7-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="95eb7-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="95eb7-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

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
# <a name="c"></a>[<span data-ttu-id="95eb7-151">C#</span><span class="sxs-lookup"><span data-stu-id="95eb7-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95eb7-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95eb7-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95eb7-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95eb7-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="95eb7-154">Java</span><span class="sxs-lookup"><span data-stu-id="95eb7-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-assignlicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="example"></a><span data-ttu-id="95eb7-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95eb7-155">Example</span></span>
<span data-ttu-id="95eb7-156">Remover licenças do usuário.</span><span class="sxs-lookup"><span data-stu-id="95eb7-156">Remove licenses from the user.</span></span>

##### <a name="request"></a><span data-ttu-id="95eb7-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95eb7-157">Request</span></span>
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```

##### <a name="response"></a><span data-ttu-id="95eb7-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="95eb7-158">Response</span></span>
<span data-ttu-id="95eb7-159">Em ambos os exemplos, a resposta é o objeto de usuário atualizado.</span><span class="sxs-lookup"><span data-stu-id="95eb7-159">In both examples, the response is the updated user object.</span></span> <span data-ttu-id="95eb7-160">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="95eb7-160">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-19T10:37:00Z",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
