---
title: Listar governançaRoleDefinitions
description: Obter uma coleção de governanceRoleDefinitions em um recurso.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 6e7d6876a9877a1bf8d146086e3aac3ec74ad60d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435809"
---
# <a name="list-governanceroledefinitions"></a><span data-ttu-id="808e8-103">Listar governançaRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="808e8-103">List governanceRoleDefinitions</span></span>

<span data-ttu-id="808e8-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="808e8-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="808e8-105">Obter uma coleção de [governanceRoleDefinitions](../resources/governanceroledefinition.md) em um recurso.</span><span class="sxs-lookup"><span data-stu-id="808e8-105">Get a collection of [governanceRoleDefinitions](../resources/governanceroledefinition.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="808e8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="808e8-106">Permissions</span></span>
<span data-ttu-id="808e8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="808e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="808e8-109">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="808e8-109">Azure resources</span></span>

| <span data-ttu-id="808e8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="808e8-110">Permission type</span></span> | <span data-ttu-id="808e8-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="808e8-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="808e8-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="808e8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="808e8-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="808e8-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="808e8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="808e8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="808e8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="808e8-115">Not supported.</span></span> |
| <span data-ttu-id="808e8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="808e8-116">Application</span></span> | <span data-ttu-id="808e8-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="808e8-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="808e8-118">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="808e8-118">Azure AD</span></span>

| <span data-ttu-id="808e8-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="808e8-119">Permission type</span></span> | <span data-ttu-id="808e8-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="808e8-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="808e8-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="808e8-121">Delegated (work or school account)</span></span> | <span data-ttu-id="808e8-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="808e8-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="808e8-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="808e8-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="808e8-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="808e8-124">Not supported.</span></span> |
| <span data-ttu-id="808e8-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="808e8-125">Application</span></span> | <span data-ttu-id="808e8-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="808e8-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="808e8-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="808e8-127">Groups</span></span>

|<span data-ttu-id="808e8-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="808e8-128">Permission type</span></span> | <span data-ttu-id="808e8-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="808e8-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="808e8-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="808e8-130">Delegated (work or school account)</span></span> | <span data-ttu-id="808e8-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="808e8-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="808e8-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="808e8-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="808e8-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="808e8-133">Not supported.</span></span> |
| <span data-ttu-id="808e8-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="808e8-134">Application</span></span> | <span data-ttu-id="808e8-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="808e8-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="808e8-136">Além do escopo de permissão, essa API exige que o solicitante tenha pelo menos uma atribuição de função no recurso.</span><span class="sxs-lookup"><span data-stu-id="808e8-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="808e8-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="808e8-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions
GET /privilegedAccess/azureResources/roleDefinitions?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="808e8-138">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="808e8-138">Optional query parameters</span></span>
<span data-ttu-id="808e8-139">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="808e8-139">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="808e8-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="808e8-140">Request headers</span></span>
| <span data-ttu-id="808e8-141">Nome</span><span class="sxs-lookup"><span data-stu-id="808e8-141">Name</span></span>      |<span data-ttu-id="808e8-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="808e8-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="808e8-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="808e8-143">Authorization</span></span>  | <span data-ttu-id="808e8-144">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="808e8-144">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="808e8-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="808e8-145">Request body</span></span>
<span data-ttu-id="808e8-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="808e8-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="808e8-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="808e8-147">Response</span></span>
<span data-ttu-id="808e8-148">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos governanceRoleDefinition](../resources/governanceroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="808e8-148">If successful, this method returns a `200 OK` response code and collection of [governanceRoleDefinition](../resources/governanceroledefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="808e8-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="808e8-149">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinitions"
}-->
<span data-ttu-id="808e8-150">Este exemplo mostra como obter todas as definições de função da assinatura Wingtip Toys - Prod.</span><span class="sxs-lookup"><span data-stu-id="808e8-150">This example shows how to get all role definitions of the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="808e8-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="808e8-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions  
```
##### <a name="response"></a><span data-ttu-id="808e8-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="808e8-152">Response</span></span>
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


