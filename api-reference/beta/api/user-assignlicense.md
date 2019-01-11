---
title: assignLicense
description: Adicionar ou remover licenças do usuário habilitar ou desabilitar o uso de ofertas de nuvem da Microsoft. Por exemplo, uma organização pode ter uma assinatura do Office 365 Enterprise E3 com 100 licenças e essa solicitação atribui uma dessas licenças a usuários específicos. Você também pode ativar e desativar os planos de específicos associados a uma assinatura. Para saber mais sobre licenças e assinaturas, consulte este artigo do Technet.
localization_priority: Normal
ms.openlocfilehash: 71287b47a0a42ce4f89635fe6a1769c78874ae36
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876199"
---
# <a name="assignlicense"></a><span data-ttu-id="fbd84-106">assignLicense</span><span class="sxs-lookup"><span data-stu-id="fbd84-106">assignLicense</span></span>

> <span data-ttu-id="fbd84-107">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fbd84-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbd84-108">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fbd84-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fbd84-109">Adicionar ou remover licenças do usuário habilitar ou desabilitar o uso de ofertas de nuvem da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fbd84-109">Add or remove licenses for the user to enable or disable their use of Microsoft cloud offerings.</span></span> <span data-ttu-id="fbd84-110">Por exemplo, uma organização pode ter uma assinatura do Office 365 Enterprise E3 com 100 licenças e essa solicitação atribui uma dessas licenças a usuários específicos.</span><span class="sxs-lookup"><span data-stu-id="fbd84-110">For example, an organization can have an Office 365 Enterprise E3 subscription with 100 licenses, and this request assigns one of those licenses to a specific user.</span></span> <span data-ttu-id="fbd84-111">Você também pode ativar e desativar os planos de específicos associados a uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="fbd84-111">You can also enable and disable specific plans associated with a subscription.</span></span> <span data-ttu-id="fbd84-112">Para saber mais sobre licenças e assinaturas, consulte este [artigo do Technet](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span><span class="sxs-lookup"><span data-stu-id="fbd84-112">To learn more about subscriptions and licenses, see this [Technet article](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span></span>

<span data-ttu-id="fbd84-113">Para obter as assinaturas disponíveis no diretório, execute um [obter subscribedSkus solicitação](subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="fbd84-113">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="fbd84-114">Permissions</span><span class="sxs-lookup"><span data-stu-id="fbd84-114">Permissions</span></span>
<span data-ttu-id="fbd84-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbd84-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbd84-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbd84-117">Permission type</span></span>      | <span data-ttu-id="fbd84-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fbd84-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbd84-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbd84-119">Delegated (work or school account)</span></span> | <span data-ttu-id="fbd84-120">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbd84-120">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="fbd84-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbd84-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbd84-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbd84-122">Not supported.</span></span>    |
|<span data-ttu-id="fbd84-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbd84-123">Application</span></span> | <span data-ttu-id="fbd84-124">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbd84-124">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbd84-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbd84-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="fbd84-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbd84-126">Request headers</span></span>
| <span data-ttu-id="fbd84-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fbd84-127">Header</span></span>       | <span data-ttu-id="fbd84-128">Valor</span><span class="sxs-lookup"><span data-stu-id="fbd84-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fbd84-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbd84-129">Authorization</span></span>  | <span data-ttu-id="fbd84-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbd84-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fbd84-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fbd84-132">Content-Type</span></span>  | <span data-ttu-id="fbd84-133">application/json</span><span class="sxs-lookup"><span data-stu-id="fbd84-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fbd84-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbd84-134">Request body</span></span>
<span data-ttu-id="fbd84-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbd84-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fbd84-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fbd84-136">Parameter</span></span>    | <span data-ttu-id="fbd84-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbd84-137">Type</span></span>   |<span data-ttu-id="fbd84-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbd84-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbd84-139">addLicenses</span><span class="sxs-lookup"><span data-stu-id="fbd84-139">addLicenses</span></span>|<span data-ttu-id="fbd84-140">Coleção [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="fbd84-140">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="fbd84-141">Uma coleção de objetos [assignedLicense](../resources/assignedlicense.md) que especificam as licenças para adicionar.</span><span class="sxs-lookup"><span data-stu-id="fbd84-141">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="fbd84-142">Você pode desabilitar servicePlans associados com uma licença, definindo a propriedade **disabledPlans** em um objeto [assignedLicense](../resources/assignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="fbd84-142">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="fbd84-143">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="fbd84-143">removeLicenses</span></span>|<span data-ttu-id="fbd84-144">Guid</span><span class="sxs-lookup"><span data-stu-id="fbd84-144">Guid</span></span>|<span data-ttu-id="fbd84-145">Uma coleção de skuIds que identificam as licenças para remover.</span><span class="sxs-lookup"><span data-stu-id="fbd84-145">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="fbd84-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbd84-146">Response</span></span>

<span data-ttu-id="fbd84-147">Se tiver êxito, este método retornará `200 OK` código de resposta e um objeto de [usuário](../resources/user.md) de atualizada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbd84-147">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbd84-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbd84-148">Example</span></span>
<span data-ttu-id="fbd84-149">Adicione licenças ao usuário.</span><span class="sxs-lookup"><span data-stu-id="fbd84-149">Add licenses to the user.</span></span>
##### <a name="request"></a><span data-ttu-id="fbd84-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbd84-150">Request</span></span>
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

## <a name="example"></a><span data-ttu-id="fbd84-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbd84-151">Example</span></span>
<span data-ttu-id="fbd84-152">Remova licenças de usuário.</span><span class="sxs-lookup"><span data-stu-id="fbd84-152">Remove licenses from the user.</span></span>

#####<a name="request"></a><span data-ttu-id="fbd84-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbd84-153">Request</span></span>
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```

##### <a name="response"></a><span data-ttu-id="fbd84-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbd84-154">Response</span></span>
<span data-ttu-id="fbd84-155">Nos dois exemplos, a resposta é o objeto de usuário atualizada.</span><span class="sxs-lookup"><span data-stu-id="fbd84-155">In both examples, the response is the updated user object.</span></span> <span data-ttu-id="fbd84-156">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="fbd84-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fbd84-157">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbd84-157">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
