---
title: Obter governanceRoleDefinition
description: Recupere as propriedades e os relacionamentos de um governanceRoleDefinition.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 1e9a2f52ea264f7bbcf3353e68deb9f51378efd1
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634974"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="e130f-103">Obter governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e130f-103">Get governanceRoleDefinition</span></span>

<span data-ttu-id="e130f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e130f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e130f-105">Recupere as propriedades e os relacionamentos de um [governanceRoleDefinition](../resources/governanceroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e130f-105">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e130f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e130f-106">Permissions</span></span>
<span data-ttu-id="e130f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="e130f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="e130f-109">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="e130f-109">Azure resources</span></span>

| <span data-ttu-id="e130f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e130f-110">Permission type</span></span> | <span data-ttu-id="e130f-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="e130f-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="e130f-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e130f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e130f-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e130f-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="e130f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e130f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e130f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e130f-115">Not supported.</span></span> |
| <span data-ttu-id="e130f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e130f-116">Application</span></span> | <span data-ttu-id="e130f-117">PrivilegedAccess. Read. AzureResources</span><span class="sxs-lookup"><span data-stu-id="e130f-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="e130f-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="e130f-118">Azure AD</span></span>

| <span data-ttu-id="e130f-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e130f-119">Permission type</span></span> | <span data-ttu-id="e130f-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="e130f-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="e130f-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e130f-121">Delegated (work or school account)</span></span> | <span data-ttu-id="e130f-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="e130f-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="e130f-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e130f-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e130f-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e130f-124">Not supported.</span></span> |
| <span data-ttu-id="e130f-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e130f-125">Application</span></span> | <span data-ttu-id="e130f-126">PrivilegedAccess. Read. AzureAD</span><span class="sxs-lookup"><span data-stu-id="e130f-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="e130f-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="e130f-127">Groups</span></span>

|<span data-ttu-id="e130f-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e130f-128">Permission type</span></span> | <span data-ttu-id="e130f-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="e130f-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="e130f-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e130f-130">Delegated (work or school account)</span></span> | <span data-ttu-id="e130f-131">PrivilegedAccess. ReadWrite. AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="e130f-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="e130f-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e130f-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e130f-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e130f-133">Not supported.</span></span> |
| <span data-ttu-id="e130f-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e130f-134">Application</span></span> | <span data-ttu-id="e130f-135">PrivilegedAccess. Read. AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="e130f-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="e130f-136">Além do escopo de permissão, essa API exige que o solicitante tenha pelo menos uma atribuição de função no recurso ao qual o [governanceRoleDefinition](../resources/governanceroledefinition.md) pertence.</span><span class="sxs-lookup"><span data-stu-id="e130f-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="e130f-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e130f-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e130f-138">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e130f-138">Optional query parameters</span></span>
<span data-ttu-id="e130f-139">Este **método não oferece suporte** aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e130f-139">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e130f-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e130f-140">Request headers</span></span>
| <span data-ttu-id="e130f-141">Nome</span><span class="sxs-lookup"><span data-stu-id="e130f-141">Name</span></span>      |<span data-ttu-id="e130f-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="e130f-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e130f-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="e130f-143">Authorization</span></span>  | <span data-ttu-id="e130f-144">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="e130f-144">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="e130f-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e130f-145">Request body</span></span>
<span data-ttu-id="e130f-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e130f-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e130f-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e130f-147">Response</span></span>
<span data-ttu-id="e130f-148">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [governanceRoleDefinition](../resources/governanceroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e130f-148">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e130f-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e130f-149">Example</span></span>
<span data-ttu-id="e130f-150">Este exemplo mostra como obter detalhes da definição de função colaborador da zona DNS na assinatura Wingtip Toys-prod.</span><span class="sxs-lookup"><span data-stu-id="e130f-150">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="e130f-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e130f-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="e130f-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="e130f-152">Response</span></span>
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


