---
title: Obter Entidadegovernanceresource
description: Recupere as propriedades e os relacionamentos de um objeto Entidadegovernanceresource.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 58bfab0115fabc835d62bfa02f5da0a96b34a6f3
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635072"
---
# <a name="get-governanceresource"></a><span data-ttu-id="e0817-103">Obter Entidadegovernanceresource</span><span class="sxs-lookup"><span data-stu-id="e0817-103">Get governanceResource</span></span>

<span data-ttu-id="e0817-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0817-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0817-105">Recupere as propriedades e os relacionamentos de um objeto [entidadegovernanceresource](../resources/governanceresource.md) .</span><span class="sxs-lookup"><span data-stu-id="e0817-105">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0817-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0817-106">Permissions</span></span>
<span data-ttu-id="e0817-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="e0817-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="e0817-109">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="e0817-109">Azure resources</span></span>

| <span data-ttu-id="e0817-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0817-110">Permission type</span></span> | <span data-ttu-id="e0817-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0817-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="e0817-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0817-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e0817-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e0817-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="e0817-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0817-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0817-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0817-115">Not supported.</span></span> |
| <span data-ttu-id="e0817-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0817-116">Application</span></span> | <span data-ttu-id="e0817-117">PrivilegedAccess. Read. AzureResources</span><span class="sxs-lookup"><span data-stu-id="e0817-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="e0817-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="e0817-118">Azure AD</span></span>

| <span data-ttu-id="e0817-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0817-119">Permission type</span></span> | <span data-ttu-id="e0817-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0817-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="e0817-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0817-121">Delegated (work or school account)</span></span> | <span data-ttu-id="e0817-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="e0817-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="e0817-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0817-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0817-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0817-124">Not supported.</span></span> |
| <span data-ttu-id="e0817-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0817-125">Application</span></span> | <span data-ttu-id="e0817-126">PrivilegedAccess. Read. AzureAD</span><span class="sxs-lookup"><span data-stu-id="e0817-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="e0817-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="e0817-127">Groups</span></span>

|<span data-ttu-id="e0817-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0817-128">Permission type</span></span> | <span data-ttu-id="e0817-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0817-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="e0817-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0817-130">Delegated (work or school account)</span></span> | <span data-ttu-id="e0817-131">PrivilegedAccess. ReadWrite. AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="e0817-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="e0817-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0817-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0817-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0817-133">Not supported.</span></span> |
| <span data-ttu-id="e0817-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0817-134">Application</span></span> | <span data-ttu-id="e0817-135">PrivilegedAccess. Read. AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="e0817-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="e0817-136">Além do escopo de permissão, essa API exige que o solicitante tenha pelo menos uma atribuição de função no recurso.</span><span class="sxs-lookup"><span data-stu-id="e0817-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="e0817-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0817-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0817-138">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e0817-138">Optional query parameters</span></span>
<span data-ttu-id="e0817-139">Este método **só** oferece suporte a  `$select` `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e0817-139">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0817-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0817-140">Request headers</span></span>
| <span data-ttu-id="e0817-141">Nome</span><span class="sxs-lookup"><span data-stu-id="e0817-141">Name</span></span>      |<span data-ttu-id="e0817-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0817-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0817-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0817-143">Authorization</span></span>  | <span data-ttu-id="e0817-144">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="e0817-144">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0817-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0817-145">Request body</span></span>
<span data-ttu-id="e0817-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e0817-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e0817-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0817-147">Response</span></span>
<span data-ttu-id="e0817-148">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [entidadegovernanceresource](../resources/governanceresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0817-148">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0817-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0817-149">Example</span></span>
<span data-ttu-id="e0817-150">Este exemplo mostra como obter os detalhes da assinatura Wingtip Toys-prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span><span class="sxs-lookup"><span data-stu-id="e0817-150">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="e0817-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0817-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="e0817-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0817-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 459

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceResources/$entity",
    "id": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",
    "type": "subscription",
    "displayName": "Wingtip Toys - Prod",
    "status": "Active",
    "registeredDateTime": "2018-04-05T22:30:37.13Z",
    "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


