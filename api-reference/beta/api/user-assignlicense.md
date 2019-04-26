---
title: assignLicense
description: Adicionar ou remover licenças para o usuário habilitar ou desabilitar o uso das ofertas de nuvem da Microsoft. Por exemplo, uma organização pode ter uma assinatura do Office 365 Enterprise E3 com licenças 100 e essa solicitação atribui uma dessas licenças a um usuário específico. Você também pode habilitar e desabilitar planos específicos associados a uma assinatura. Para saber mais sobre assinaturas e licenças, confira este artigo da TechNet.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ef9946a7ac53a0e0e8b90a31fd4767bcc0549468
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547988"
---
# <a name="assignlicense"></a><span data-ttu-id="cdfae-106">assignLicense</span><span class="sxs-lookup"><span data-stu-id="cdfae-106">assignLicense</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdfae-107">Adicionar ou remover licenças para o usuário habilitar ou desabilitar o uso das ofertas de nuvem da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="cdfae-107">Add or remove licenses for the user to enable or disable their use of Microsoft cloud offerings.</span></span> <span data-ttu-id="cdfae-108">Por exemplo, uma organização pode ter uma assinatura do Office 365 Enterprise E3 com licenças 100 e essa solicitação atribui uma dessas licenças a um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="cdfae-108">For example, an organization can have an Office 365 Enterprise E3 subscription with 100 licenses, and this request assigns one of those licenses to a specific user.</span></span> <span data-ttu-id="cdfae-109">Você também pode habilitar e desabilitar planos específicos associados a uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="cdfae-109">You can also enable and disable specific plans associated with a subscription.</span></span> <span data-ttu-id="cdfae-110">Para saber mais sobre assinaturas e licenças, confira este [artigo da TechNet](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span><span class="sxs-lookup"><span data-stu-id="cdfae-110">To learn more about subscriptions and licenses, see this [Technet article](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span></span>

<span data-ttu-id="cdfae-111">Para obter as assinaturas disponíveis no diretório, execute uma [solicitação get subscribedSkus](subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="cdfae-111">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="cdfae-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="cdfae-112">Permissions</span></span>
<span data-ttu-id="cdfae-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdfae-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdfae-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdfae-115">Permission type</span></span>      | <span data-ttu-id="cdfae-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cdfae-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdfae-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdfae-117">Delegated (work or school account)</span></span> | <span data-ttu-id="cdfae-118">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdfae-118">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="cdfae-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdfae-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdfae-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdfae-120">Not supported.</span></span>    |
|<span data-ttu-id="cdfae-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdfae-121">Application</span></span> | <span data-ttu-id="cdfae-122">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdfae-122">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdfae-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdfae-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="cdfae-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdfae-124">Request headers</span></span>
| <span data-ttu-id="cdfae-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cdfae-125">Header</span></span>       | <span data-ttu-id="cdfae-126">Valor</span><span class="sxs-lookup"><span data-stu-id="cdfae-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cdfae-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdfae-127">Authorization</span></span>  | <span data-ttu-id="cdfae-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdfae-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cdfae-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cdfae-130">Content-Type</span></span>  | <span data-ttu-id="cdfae-131">application/json</span><span class="sxs-lookup"><span data-stu-id="cdfae-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cdfae-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdfae-132">Request body</span></span>
<span data-ttu-id="cdfae-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cdfae-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cdfae-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cdfae-134">Parameter</span></span>    | <span data-ttu-id="cdfae-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdfae-135">Type</span></span>   |<span data-ttu-id="cdfae-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdfae-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cdfae-137">addLicenses</span><span class="sxs-lookup"><span data-stu-id="cdfae-137">addLicenses</span></span>|<span data-ttu-id="cdfae-138">Coleção [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="cdfae-138">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="cdfae-139">Uma coleção de objetos [assignedLicense](../resources/assignedlicense.md) que especifica as licenças a adicionar.</span><span class="sxs-lookup"><span data-stu-id="cdfae-139">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="cdfae-140">Você pode desabilitar o onPlans associado a uma licença definindo a propriedade **disabledPlans** em um objeto [assignedLicense](../resources/assignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="cdfae-140">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="cdfae-141">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="cdfae-141">removeLicenses</span></span>|<span data-ttu-id="cdfae-142">Guid</span><span class="sxs-lookup"><span data-stu-id="cdfae-142">Guid</span></span>|<span data-ttu-id="cdfae-143">Uma coleção de skuIds que identifica as licenças a serem removidas.</span><span class="sxs-lookup"><span data-stu-id="cdfae-143">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="cdfae-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdfae-144">Response</span></span>

<span data-ttu-id="cdfae-145">Se bem-sucedido, este método retorna `200 OK` o código de resposta e um objeto [User](../resources/user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdfae-145">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdfae-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdfae-146">Example</span></span>
<span data-ttu-id="cdfae-147">Adicionar licenças ao usuário.</span><span class="sxs-lookup"><span data-stu-id="cdfae-147">Add licenses to the user.</span></span>
##### <a name="request"></a><span data-ttu-id="cdfae-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdfae-148">Request</span></span>
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

## <a name="example"></a><span data-ttu-id="cdfae-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdfae-149">Example</span></span>
<span data-ttu-id="cdfae-150">Remover licenças do usuário.</span><span class="sxs-lookup"><span data-stu-id="cdfae-150">Remove licenses from the user.</span></span>

##### <a name="request"></a><span data-ttu-id="cdfae-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdfae-151">Request</span></span>
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```

##### <a name="response"></a><span data-ttu-id="cdfae-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdfae-152">Response</span></span>
<span data-ttu-id="cdfae-153">Em ambos os exemplos, a resposta é o objeto de usuário atualizado.</span><span class="sxs-lookup"><span data-stu-id="cdfae-153">In both examples, the response is the updated user object.</span></span> <span data-ttu-id="cdfae-154">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="cdfae-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cdfae-155">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cdfae-155">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/user-assignlicense.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
