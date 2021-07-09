---
title: Obter governanceResource
description: Recupere as propriedades e as relações de um objeto governanceResource.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: fe69275c46b46406f67cecadc3cf3eb01a60d8f0
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350695"
---
# <a name="get-governanceresource"></a><span data-ttu-id="8545d-103">Obter governanceResource</span><span class="sxs-lookup"><span data-stu-id="8545d-103">Get governanceResource</span></span>

<span data-ttu-id="8545d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8545d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8545d-105">Recupere as propriedades e as relações de um [objeto governanceResource.](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="8545d-105">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8545d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8545d-106">Permissions</span></span>
<span data-ttu-id="8545d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="8545d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="8545d-109">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="8545d-109">Azure resources</span></span>

| <span data-ttu-id="8545d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8545d-110">Permission type</span></span> | <span data-ttu-id="8545d-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="8545d-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="8545d-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8545d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8545d-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="8545d-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="8545d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8545d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8545d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8545d-115">Not supported.</span></span> |
| <span data-ttu-id="8545d-116">Application</span><span class="sxs-lookup"><span data-stu-id="8545d-116">Application</span></span> | <span data-ttu-id="8545d-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="8545d-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="8545d-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="8545d-118">Azure AD</span></span>

| <span data-ttu-id="8545d-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8545d-119">Permission type</span></span> | <span data-ttu-id="8545d-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="8545d-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="8545d-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8545d-121">Delegated (work or school account)</span></span> | <span data-ttu-id="8545d-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="8545d-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="8545d-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8545d-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8545d-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8545d-124">Not supported.</span></span> |
| <span data-ttu-id="8545d-125">Application</span><span class="sxs-lookup"><span data-stu-id="8545d-125">Application</span></span> | <span data-ttu-id="8545d-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="8545d-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="8545d-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="8545d-127">Groups</span></span>

|<span data-ttu-id="8545d-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8545d-128">Permission type</span></span> | <span data-ttu-id="8545d-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="8545d-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="8545d-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8545d-130">Delegated (work or school account)</span></span> | <span data-ttu-id="8545d-131">PrivilegedAccess.ReadWrite.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="8545d-131">PrivilegedAccess.ReadWrite.AzureADGroup</span></span> |
| <span data-ttu-id="8545d-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8545d-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8545d-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8545d-133">Not supported.</span></span> |
| <span data-ttu-id="8545d-134">Application</span><span class="sxs-lookup"><span data-stu-id="8545d-134">Application</span></span> | <span data-ttu-id="8545d-135">PrivilegedAccess.Read.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="8545d-135">PrivilegedAccess.Read.AzureADGroup</span></span> |

<span data-ttu-id="8545d-136">Além do escopo de permissão, essa API exige que o solicitante tenha pelo menos uma atribuição de função no recurso.</span><span class="sxs-lookup"><span data-stu-id="8545d-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="8545d-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8545d-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8545d-138">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8545d-138">Optional query parameters</span></span>
<span data-ttu-id="8545d-139">Esse método **só dá** suporte  `$select` a `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8545d-139">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8545d-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8545d-140">Request headers</span></span>
| <span data-ttu-id="8545d-141">Nome</span><span class="sxs-lookup"><span data-stu-id="8545d-141">Name</span></span>      |<span data-ttu-id="8545d-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="8545d-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8545d-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="8545d-143">Authorization</span></span>  | <span data-ttu-id="8545d-144">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="8545d-144">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8545d-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8545d-145">Request body</span></span>
<span data-ttu-id="8545d-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8545d-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8545d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="8545d-147">Response</span></span>
<span data-ttu-id="8545d-148">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [governanceResource](../resources/governanceresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8545d-148">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8545d-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8545d-149">Example</span></span>
<span data-ttu-id="8545d-150">Este exemplo mostra como obter os detalhes da assinatura Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span><span class="sxs-lookup"><span data-stu-id="8545d-150">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="8545d-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8545d-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="8545d-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="8545d-152">Response</span></span>
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


