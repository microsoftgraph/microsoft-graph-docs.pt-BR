---
title: assignLicense
description: Adicionar ou remover licenças para o usuário habilitar ou desabilitar o uso das ofertas de nuvem da Microsoft. Por exemplo, uma organização pode ter uma assinatura do Office 365 Enterprise E3 com licenças 100 e essa solicitação atribui uma dessas licenças a um usuário específico. Você também pode habilitar e desabilitar planos específicos associados a uma assinatura. Para saber mais sobre assinaturas e licenças, confira este artigo da TechNet.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: eea6d5b838eb3f5d2169d98b0a258befe27a74ab
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421174"
---
# <a name="assignlicense"></a><span data-ttu-id="79842-106">assignLicense</span><span class="sxs-lookup"><span data-stu-id="79842-106">assignLicense</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79842-107">Adicionar ou remover licenças para o usuário habilitar ou desabilitar o uso das ofertas de nuvem da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="79842-107">Add or remove licenses for the user to enable or disable their use of Microsoft cloud offerings.</span></span> <span data-ttu-id="79842-108">Por exemplo, uma organização pode ter uma assinatura do Office 365 Enterprise E3 com licenças 100 e essa solicitação atribui uma dessas licenças a um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="79842-108">For example, an organization can have an Office 365 Enterprise E3 subscription with 100 licenses, and this request assigns one of those licenses to a specific user.</span></span> <span data-ttu-id="79842-109">Você também pode habilitar e desabilitar planos específicos associados a uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="79842-109">You can also enable and disable specific plans associated with a subscription.</span></span> <span data-ttu-id="79842-110">Para saber mais sobre assinaturas e licenças, confira este [artigo da TechNet](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span><span class="sxs-lookup"><span data-stu-id="79842-110">To learn more about subscriptions and licenses, see this [Technet article](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span></span>

<span data-ttu-id="79842-111">Para obter as assinaturas disponíveis no diretório, execute uma [solicitação get subscribedSkus](subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="79842-111">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="79842-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="79842-112">Permissions</span></span>
<span data-ttu-id="79842-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79842-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79842-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79842-115">Permission type</span></span>      | <span data-ttu-id="79842-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79842-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79842-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79842-117">Delegated (work or school account)</span></span> | <span data-ttu-id="79842-118">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79842-118">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="79842-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79842-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79842-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79842-120">Not supported.</span></span>    |
|<span data-ttu-id="79842-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79842-121">Application</span></span> | <span data-ttu-id="79842-122">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79842-122">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79842-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79842-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="79842-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79842-124">Request headers</span></span>
| <span data-ttu-id="79842-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79842-125">Header</span></span>       | <span data-ttu-id="79842-126">Valor</span><span class="sxs-lookup"><span data-stu-id="79842-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="79842-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="79842-127">Authorization</span></span>  | <span data-ttu-id="79842-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79842-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="79842-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79842-130">Content-Type</span></span>  | <span data-ttu-id="79842-131">application/json</span><span class="sxs-lookup"><span data-stu-id="79842-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="79842-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79842-132">Request body</span></span>
<span data-ttu-id="79842-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79842-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="79842-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="79842-134">Parameter</span></span>    | <span data-ttu-id="79842-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="79842-135">Type</span></span>   |<span data-ttu-id="79842-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="79842-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79842-137">addLicenses</span><span class="sxs-lookup"><span data-stu-id="79842-137">addLicenses</span></span>|<span data-ttu-id="79842-138">Coleção [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="79842-138">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="79842-139">Uma coleção de objetos [assignedLicense](../resources/assignedlicense.md) que especifica as licenças a adicionar.</span><span class="sxs-lookup"><span data-stu-id="79842-139">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="79842-140">Você pode desabilitar o onplans associado a uma licença definindo a propriedade **disabledPlans** em um objeto [assignedLicense](../resources/assignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="79842-140">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="79842-141">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="79842-141">removeLicenses</span></span>|<span data-ttu-id="79842-142">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="79842-142">Guid collection</span></span>|<span data-ttu-id="79842-143">Uma coleção de skuIds que identifica as licenças a serem removidas.</span><span class="sxs-lookup"><span data-stu-id="79842-143">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="79842-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="79842-144">Response</span></span>

<span data-ttu-id="79842-145">Se bem-sucedido, este método retorna `200 OK` o código de resposta e um objeto [User](../resources/user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79842-145">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79842-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79842-146">Example</span></span>
<span data-ttu-id="79842-147">Adicionar licenças ao usuário.</span><span class="sxs-lookup"><span data-stu-id="79842-147">Add licenses to the user.</span></span>
##### <a name="request"></a><span data-ttu-id="79842-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79842-148">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="79842-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="79842-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="79842-150">C#</span><span class="sxs-lookup"><span data-stu-id="79842-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79842-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79842-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79842-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="79842-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="example"></a><span data-ttu-id="79842-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79842-153">Example</span></span>
<span data-ttu-id="79842-154">Remover licenças do usuário.</span><span class="sxs-lookup"><span data-stu-id="79842-154">Remove licenses from the user.</span></span>

##### <a name="request"></a><span data-ttu-id="79842-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79842-155">Request</span></span>
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```

##### <a name="response"></a><span data-ttu-id="79842-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="79842-156">Response</span></span>
<span data-ttu-id="79842-157">Em ambos os exemplos, a resposta é o objeto de usuário atualizado.</span><span class="sxs-lookup"><span data-stu-id="79842-157">In both examples, the response is the updated user object.</span></span> <span data-ttu-id="79842-158">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="79842-158">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="79842-159">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79842-159">All of the properties will be returned from an actual call.</span></span>
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
