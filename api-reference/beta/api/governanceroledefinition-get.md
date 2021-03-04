---
title: Obter governançaRoleDefinition
description: Recupere as propriedades e as relações de um governanceRoleDefinition.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 97d3ed248d5a808cf57edf5f18cc37cc07e44bf7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435837"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="caf04-103">Obter governançaRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="caf04-103">Get governanceRoleDefinition</span></span>

<span data-ttu-id="caf04-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="caf04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="caf04-105">Recupere as propriedades e as relações de um [governanceRoleDefinition](../resources/governanceroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="caf04-105">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="caf04-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="caf04-106">Permissions</span></span>
<span data-ttu-id="caf04-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="caf04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="caf04-109">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="caf04-109">Azure resources</span></span>

| <span data-ttu-id="caf04-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="caf04-110">Permission type</span></span> | <span data-ttu-id="caf04-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="caf04-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="caf04-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="caf04-112">Delegated (work or school account)</span></span> | <span data-ttu-id="caf04-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="caf04-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="caf04-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="caf04-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="caf04-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="caf04-115">Not supported.</span></span> |
| <span data-ttu-id="caf04-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="caf04-116">Application</span></span> | <span data-ttu-id="caf04-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="caf04-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="caf04-118">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="caf04-118">Azure AD</span></span>

| <span data-ttu-id="caf04-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="caf04-119">Permission type</span></span> | <span data-ttu-id="caf04-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="caf04-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="caf04-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="caf04-121">Delegated (work or school account)</span></span> | <span data-ttu-id="caf04-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="caf04-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="caf04-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="caf04-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="caf04-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="caf04-124">Not supported.</span></span> |
| <span data-ttu-id="caf04-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="caf04-125">Application</span></span> | <span data-ttu-id="caf04-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="caf04-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="caf04-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="caf04-127">Groups</span></span>

|<span data-ttu-id="caf04-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="caf04-128">Permission type</span></span> | <span data-ttu-id="caf04-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="caf04-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="caf04-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="caf04-130">Delegated (work or school account)</span></span> | <span data-ttu-id="caf04-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="caf04-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="caf04-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="caf04-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="caf04-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="caf04-133">Not supported.</span></span> |
| <span data-ttu-id="caf04-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="caf04-134">Application</span></span> | <span data-ttu-id="caf04-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="caf04-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="caf04-136">Além do escopo de permissão, essa API exige que o solicitante tenha pelo menos uma atribuição de função no recurso, à qual a [governanceRoleDefinition](../resources/governanceroledefinition.md) pertence.</span><span class="sxs-lookup"><span data-stu-id="caf04-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="caf04-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="caf04-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="caf04-138">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="caf04-138">Optional query parameters</span></span>
<span data-ttu-id="caf04-139">Este método não **dá suporte** aos [Parâmetros de Consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="caf04-139">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="caf04-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="caf04-140">Request headers</span></span>
| <span data-ttu-id="caf04-141">Nome</span><span class="sxs-lookup"><span data-stu-id="caf04-141">Name</span></span>      |<span data-ttu-id="caf04-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="caf04-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="caf04-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="caf04-143">Authorization</span></span>  | <span data-ttu-id="caf04-144">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="caf04-144">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="caf04-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="caf04-145">Request body</span></span>
<span data-ttu-id="caf04-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="caf04-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="caf04-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="caf04-147">Response</span></span>
<span data-ttu-id="caf04-148">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto governanceRoleDefinition](../resources/governanceroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="caf04-148">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="caf04-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="caf04-149">Example</span></span>
<span data-ttu-id="caf04-150">Este exemplo mostra como obter detalhes da definição de função DNS Zone Contributor na assinatura Wingtip Toys - Prod.</span><span class="sxs-lookup"><span data-stu-id="caf04-150">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="caf04-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="caf04-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="caf04-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="caf04-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 174

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleDefinitions/$entity",
    "id": "00efc9e0-1b96-4e9a-99a3-a3df0735cf88",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/befefa01-2a29-4197-83a8-272ff33ce314",
    "templateId": "befefa01-2a29-4197-83a8-272ff33ce314",
    "displayName": "DNS Zone Contributor"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


