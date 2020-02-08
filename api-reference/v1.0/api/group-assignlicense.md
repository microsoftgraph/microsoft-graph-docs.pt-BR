---
title: 'Grupo: assignLicense'
description: Adicionar ou remover licenças no grupo. As licenças atribuídas ao grupo serão atribuídas a todos os usuários do grupo.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 43fa0a9346ccecc704c49ffc7528b71a58763fbc
ms.sourcegitcommit: cea768f767cf27a938b72bb26892d70e3dedaf2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/08/2020
ms.locfileid: "41865765"
---
# <a name="group-assignlicense"></a><span data-ttu-id="1b300-104">Grupo: assignLicense</span><span class="sxs-lookup"><span data-stu-id="1b300-104">group: assignLicense</span></span>

<span data-ttu-id="1b300-105">Adicionar ou remover licenças no grupo.</span><span class="sxs-lookup"><span data-stu-id="1b300-105">Add or remove licenses on the group.</span></span> <span data-ttu-id="1b300-106">As licenças atribuídas ao grupo serão atribuídas a todos os usuários do grupo.</span><span class="sxs-lookup"><span data-stu-id="1b300-106">Licenses assigned to the group will be assigned to all users in the group.</span></span> <span data-ttu-id="1b300-107">Para saber mais sobre licenciamento baseado em grupo, confira [o que é licenciamento baseado em grupo no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="1b300-107">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span>

<span data-ttu-id="1b300-108">Para obter as assinaturas disponíveis no diretório, execute uma [solicitação get subscribedSkus](../resources/subscribedsku.md).</span><span class="sxs-lookup"><span data-stu-id="1b300-108">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](../resources/subscribedsku.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1b300-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b300-109">Permissions</span></span>
<span data-ttu-id="1b300-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b300-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b300-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b300-112">Permission type</span></span>      | <span data-ttu-id="1b300-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b300-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b300-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b300-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1b300-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b300-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="1b300-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b300-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b300-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b300-117">Not supported.</span></span>    |
|<span data-ttu-id="1b300-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b300-118">Application</span></span> | <span data-ttu-id="1b300-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b300-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b300-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b300-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="1b300-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b300-121">Request headers</span></span>
| <span data-ttu-id="1b300-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1b300-122">Header</span></span>       | <span data-ttu-id="1b300-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1b300-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1b300-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b300-124">Authorization</span></span>  | <span data-ttu-id="1b300-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b300-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1b300-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b300-127">Content-Type</span></span>  | <span data-ttu-id="1b300-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b300-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1b300-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b300-130">Request body</span></span>
<span data-ttu-id="1b300-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b300-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1b300-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1b300-132">Parameter</span></span>    | <span data-ttu-id="1b300-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b300-133">Type</span></span>   |<span data-ttu-id="1b300-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b300-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b300-135">addLicenses</span><span class="sxs-lookup"><span data-stu-id="1b300-135">addLicenses</span></span>|<span data-ttu-id="1b300-136">Coleção [assignedLicense](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="1b300-136">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="1b300-137">Uma coleção de objetos [assignedLicense](../resources/assignedlicense.md) que especifica as licenças a adicionar.</span><span class="sxs-lookup"><span data-stu-id="1b300-137">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="1b300-138">Você pode desabilitar o onplans associado a uma licença definindo a propriedade **disabledPlans** em um objeto [assignedLicense](../resources/assignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="1b300-138">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="1b300-139">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="1b300-139">removeLicenses</span></span>|<span data-ttu-id="1b300-140">Coleção GUID</span><span class="sxs-lookup"><span data-stu-id="1b300-140">GUID collection</span></span>|<span data-ttu-id="1b300-141">Uma coleção de skuIds que identifica as licenças a serem removidas.</span><span class="sxs-lookup"><span data-stu-id="1b300-141">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="1b300-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b300-142">Response</span></span>

<span data-ttu-id="1b300-143">Se tiver êxito, este método retornará `202 Accepted` um código de resposta e um objeto de [grupo](../resources/group.md) de destino no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b300-143">If successful, this method returns a `202 Accepted` response code and a target [group](../resources/group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b300-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1b300-144">Examples</span></span>

### <a name="example-1-add-licenses-to-the-group"></a><span data-ttu-id="1b300-145">Exemplo 1: adicionar licenças ao grupo</span><span class="sxs-lookup"><span data-stu-id="1b300-145">Example 1: Add licenses to the group</span></span>
<span data-ttu-id="1b300-146">O exemplo a seguir adiciona licenças ao grupo.</span><span class="sxs-lookup"><span data-stu-id="1b300-146">The following example adds licenses to the group.</span></span>
#### <a name="request"></a><span data-ttu-id="1b300-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b300-147">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1b300-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b300-148">HTTP</span></span>](#tab/http)
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

#### <a name="response"></a><span data-ttu-id="1b300-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b300-149">Response</span></span>

<span data-ttu-id="1b300-150">A resposta é o objeto de grupo atualizado.</span><span class="sxs-lookup"><span data-stu-id="1b300-150">The response is the updated group object.</span></span>

><span data-ttu-id="1b300-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1b300-151">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1b300-152">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b300-152">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-remove-licenses-from-the-group"></a><span data-ttu-id="1b300-153">Exemplo 2: remover licenças do grupo</span><span class="sxs-lookup"><span data-stu-id="1b300-153">Example 2: Remove licenses from the group</span></span>
<span data-ttu-id="1b300-154">O exemplo a seguir remove licenças do grupo.</span><span class="sxs-lookup"><span data-stu-id="1b300-154">The following example removes licenses from the group.</span></span>

#### <a name="request"></a><span data-ttu-id="1b300-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b300-155">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1b300-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b300-156">HTTP</span></span>](#tab/http)
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

#### <a name="response"></a><span data-ttu-id="1b300-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b300-157">Response</span></span>

<span data-ttu-id="1b300-158">A resposta é o objeto de grupo atualizado.</span><span class="sxs-lookup"><span data-stu-id="1b300-158">The response is the updated group object.</span></span>

><span data-ttu-id="1b300-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1b300-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1b300-160">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b300-160">All the properties will be returned from an actual call..</span></span>
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
