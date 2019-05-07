---
title: assignLicense
description: Adicionar ou remover licenças para o usuário habilitar ou desabilitar o uso das ofertas de nuvem da Microsoft. Por exemplo, uma organização pode ter uma assinatura do Office 365 Enterprise E3 com licenças 100 e essa solicitação atribui uma dessas licenças a um usuário específico. Você também pode habilitar e desabilitar planos específicos associados a uma assinatura. Para saber mais sobre assinaturas e licenças, confira este artigo da TechNet.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a6a5b17a31522ee58007b991fe04b5d26fdba188
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637406"
---
# <a name="assignlicense"></a><span data-ttu-id="58e52-106">assignLicense</span><span class="sxs-lookup"><span data-stu-id="58e52-106">assignLicense</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58e52-107">Adicionar ou remover licenças para o usuário habilitar ou desabilitar o uso das ofertas de nuvem da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="58e52-107">Add or remove licenses for the user to enable or disable their use of Microsoft cloud offerings.</span></span> <span data-ttu-id="58e52-108">Por exemplo, uma organização pode ter uma assinatura do Office 365 Enterprise E3 com licenças 100 e essa solicitação atribui uma dessas licenças a um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="58e52-108">For example, an organization can have an Office 365 Enterprise E3 subscription with 100 licenses, and this request assigns one of those licenses to a specific user.</span></span> <span data-ttu-id="58e52-109">Você também pode habilitar e desabilitar planos específicos associados a uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="58e52-109">You can also enable and disable specific plans associated with a subscription.</span></span> <span data-ttu-id="58e52-110">Para saber mais sobre assinaturas e licenças, confira este [artigo da TechNet](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span><span class="sxs-lookup"><span data-stu-id="58e52-110">To learn more about subscriptions and licenses, see this [Technet article](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span></span>

<span data-ttu-id="58e52-111">Para obter as assinaturas disponíveis no diretório, execute uma [solicitação get subscribedSkus](subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="58e52-111">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="58e52-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="58e52-112">Permissions</span></span>
<span data-ttu-id="58e52-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58e52-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58e52-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58e52-115">Permission type</span></span>      | <span data-ttu-id="58e52-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58e52-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58e52-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58e52-117">Delegated (work or school account)</span></span> | <span data-ttu-id="58e52-118">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58e52-118">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="58e52-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58e52-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58e52-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58e52-120">Not supported.</span></span>    |
|<span data-ttu-id="58e52-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58e52-121">Application</span></span> | <span data-ttu-id="58e52-122">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58e52-122">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58e52-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58e52-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="58e52-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58e52-124">Request headers</span></span>
| <span data-ttu-id="58e52-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58e52-125">Header</span></span>       | <span data-ttu-id="58e52-126">Valor</span><span class="sxs-lookup"><span data-stu-id="58e52-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="58e52-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="58e52-127">Authorization</span></span>  | <span data-ttu-id="58e52-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58e52-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="58e52-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="58e52-130">Content-Type</span></span>  | <span data-ttu-id="58e52-131">application/json</span><span class="sxs-lookup"><span data-stu-id="58e52-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="58e52-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58e52-132">Request body</span></span>
<span data-ttu-id="58e52-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58e52-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="58e52-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="58e52-134">Parameter</span></span>    | <span data-ttu-id="58e52-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="58e52-135">Type</span></span>   |<span data-ttu-id="58e52-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="58e52-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58e52-137">addLicenses</span><span class="sxs-lookup"><span data-stu-id="58e52-137">addLicenses</span></span>|<span data-ttu-id="58e52-138">Coleção [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="58e52-138">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="58e52-139">Uma coleção de objetos [assignedLicense](../resources/assignedlicense.md) que especifica as licenças a adicionar.</span><span class="sxs-lookup"><span data-stu-id="58e52-139">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="58e52-140">Você pode desabilitar o onplans associado a uma licença definindo a propriedade **disabledPlans** em um objeto [assignedLicense](../resources/assignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="58e52-140">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="58e52-141">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="58e52-141">removeLicenses</span></span>|<span data-ttu-id="58e52-142">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="58e52-142">Guid collection</span></span>|<span data-ttu-id="58e52-143">Uma coleção de skuIds que identifica as licenças a serem removidas.</span><span class="sxs-lookup"><span data-stu-id="58e52-143">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="58e52-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="58e52-144">Response</span></span>

<span data-ttu-id="58e52-145">Se bem-sucedido, este método retorna `200 OK` o código de resposta e um objeto [User](../resources/user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58e52-145">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58e52-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58e52-146">Example</span></span>
<span data-ttu-id="58e52-147">Adicionar licenças ao usuário.</span><span class="sxs-lookup"><span data-stu-id="58e52-147">Add licenses to the user.</span></span>
##### <a name="request"></a><span data-ttu-id="58e52-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58e52-148">Request</span></span>
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

## <a name="example"></a><span data-ttu-id="58e52-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58e52-149">Example</span></span>
<span data-ttu-id="58e52-150">Remover licenças do usuário.</span><span class="sxs-lookup"><span data-stu-id="58e52-150">Remove licenses from the user.</span></span>

##### <a name="request"></a><span data-ttu-id="58e52-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58e52-151">Request</span></span>
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="58e52-152">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="58e52-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="58e52-153">Basic</span><span class="sxs-lookup"><span data-stu-id="58e52-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_assignlicense-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="58e52-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58e52-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_assignlicense-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="response"></a><span data-ttu-id="58e52-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="58e52-155">Response</span></span>
<span data-ttu-id="58e52-156">Em ambos os exemplos, a resposta é o objeto de usuário atualizado.</span><span class="sxs-lookup"><span data-stu-id="58e52-156">In both examples, the response is the updated user object.</span></span> <span data-ttu-id="58e52-157">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="58e52-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="58e52-158">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58e52-158">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/user-assignlicense.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-assignlicense.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
