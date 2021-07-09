---
title: Listar governançaRoleDefinitions
description: Obter uma coleção de governanceRoleDefinitions em um recurso.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 7684d3593015d7320c955e4465aacd21c62faae8
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350681"
---
# <a name="list-governanceroledefinitions"></a><span data-ttu-id="ac750-103">Listar governançaRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="ac750-103">List governanceRoleDefinitions</span></span>

<span data-ttu-id="ac750-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="ac750-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="ac750-105">Obter uma coleção de [governanceRoleDefinitions](../resources/governanceroledefinition.md) em um recurso.</span><span class="sxs-lookup"><span data-stu-id="ac750-105">Get a collection of [governanceRoleDefinitions](../resources/governanceroledefinition.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac750-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac750-106">Permissions</span></span>
<span data-ttu-id="ac750-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="ac750-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="ac750-109">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="ac750-109">Azure resources</span></span>

| <span data-ttu-id="ac750-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac750-110">Permission type</span></span> | <span data-ttu-id="ac750-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac750-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="ac750-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac750-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ac750-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="ac750-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="ac750-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac750-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac750-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac750-115">Not supported.</span></span> |
| <span data-ttu-id="ac750-116">Application</span><span class="sxs-lookup"><span data-stu-id="ac750-116">Application</span></span> | <span data-ttu-id="ac750-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="ac750-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="ac750-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="ac750-118">Azure AD</span></span>

| <span data-ttu-id="ac750-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac750-119">Permission type</span></span> | <span data-ttu-id="ac750-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac750-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="ac750-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac750-121">Delegated (work or school account)</span></span> | <span data-ttu-id="ac750-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="ac750-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="ac750-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac750-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac750-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac750-124">Not supported.</span></span> |
| <span data-ttu-id="ac750-125">Application</span><span class="sxs-lookup"><span data-stu-id="ac750-125">Application</span></span> | <span data-ttu-id="ac750-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="ac750-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="ac750-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="ac750-127">Groups</span></span>

|<span data-ttu-id="ac750-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac750-128">Permission type</span></span> | <span data-ttu-id="ac750-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac750-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="ac750-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac750-130">Delegated (work or school account)</span></span> | <span data-ttu-id="ac750-131">PrivilegedAccess.ReadWrite.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="ac750-131">PrivilegedAccess.ReadWrite.AzureADGroup</span></span> |
| <span data-ttu-id="ac750-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac750-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac750-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac750-133">Not supported.</span></span> |
| <span data-ttu-id="ac750-134">Application</span><span class="sxs-lookup"><span data-stu-id="ac750-134">Application</span></span> | <span data-ttu-id="ac750-135">PrivilegedAccess.Read.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="ac750-135">PrivilegedAccess.Read.AzureADGroup</span></span> |

<span data-ttu-id="ac750-136">Além do escopo de permissão, essa API exige que o solicitante tenha pelo menos uma atribuição de função no recurso.</span><span class="sxs-lookup"><span data-stu-id="ac750-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="ac750-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac750-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions
GET /privilegedAccess/azureResources/roleDefinitions?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ac750-138">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ac750-138">Optional query parameters</span></span>
<span data-ttu-id="ac750-139">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ac750-139">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac750-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac750-140">Request headers</span></span>
| <span data-ttu-id="ac750-141">Nome</span><span class="sxs-lookup"><span data-stu-id="ac750-141">Name</span></span>      |<span data-ttu-id="ac750-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac750-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ac750-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac750-143">Authorization</span></span>  | <span data-ttu-id="ac750-144">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="ac750-144">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac750-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac750-145">Request body</span></span>
<span data-ttu-id="ac750-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ac750-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ac750-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac750-147">Response</span></span>
<span data-ttu-id="ac750-148">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos governanceRoleDefinition](../resources/governanceroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac750-148">If successful, this method returns a `200 OK` response code and collection of [governanceRoleDefinition](../resources/governanceroledefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ac750-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac750-149">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinitions"
}-->
<span data-ttu-id="ac750-150">Este exemplo mostra como obter todas as definições de função da assinatura Wingtip Toys - Prod.</span><span class="sxs-lookup"><span data-stu-id="ac750-150">This example shows how to get all role definitions of the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="ac750-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac750-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions  
```
##### <a name="response"></a><span data-ttu-id="ac750-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac750-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleDefinition",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 21906

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleDefinitions",
    "value": [
        {
            "id": "00efc9e0-1b96-4e9a-99a3-a3df0735cf88",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/befefa01-2a29-4197-83a8-272ff33ce314",
            "templateId": "befefa01-2a29-4197-83a8-272ff33ce314",
            "displayName": "DNS Zone Contributor"
        },
        {
            "id": "051f7264-a992-429a-b345-90415af9f917",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/c12c1c16-33a1-487b-954d-41c89c60f349",
            "templateId": "c12c1c16-33a1-487b-954d-41c89c60f349",
            "displayName": "Reader and Data Access"
        },
        {
            "id": "0789c03d-445d-40ab-aed3-d110a98146c7",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/5d28c62d-5b37-4476-8438-e587778df237",
            "templateId": "5d28c62d-5b37-4476-8438-e587778df237",
            "displayName": "New Relic APM Account Contributor"
        },
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List governanceRoleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


