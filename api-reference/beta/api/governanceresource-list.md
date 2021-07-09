---
title: Listar governançaResources
description: Recupere uma coleção de governanceResource à que o solicitante tem acesso.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 575b28e799036c138318269accab1ae9ccbb0f1a
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350891"
---
# <a name="list-governanceresources"></a><span data-ttu-id="b8217-103">Listar governançaResources</span><span class="sxs-lookup"><span data-stu-id="b8217-103">List governanceResources</span></span>

<span data-ttu-id="b8217-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8217-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8217-105">Recupere uma coleção [de governanceResource](../resources/governanceresource.md) à que o solicitante tem acesso.</span><span class="sxs-lookup"><span data-stu-id="b8217-105">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8217-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8217-106">Permissions</span></span>
<span data-ttu-id="b8217-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="b8217-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="b8217-109">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="b8217-109">Azure resources</span></span>

| <span data-ttu-id="b8217-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8217-110">Permission type</span></span> | <span data-ttu-id="b8217-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8217-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="b8217-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8217-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b8217-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b8217-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="b8217-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8217-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8217-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8217-115">Not supported.</span></span> |
| <span data-ttu-id="b8217-116">Application</span><span class="sxs-lookup"><span data-stu-id="b8217-116">Application</span></span> | <span data-ttu-id="b8217-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b8217-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="b8217-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="b8217-118">Azure AD</span></span>

| <span data-ttu-id="b8217-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8217-119">Permission type</span></span> | <span data-ttu-id="b8217-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8217-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="b8217-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8217-121">Delegated (work or school account)</span></span> | <span data-ttu-id="b8217-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="b8217-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="b8217-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8217-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8217-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8217-124">Not supported.</span></span> |
| <span data-ttu-id="b8217-125">Application</span><span class="sxs-lookup"><span data-stu-id="b8217-125">Application</span></span> | <span data-ttu-id="b8217-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="b8217-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="b8217-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="b8217-127">Groups</span></span>

|<span data-ttu-id="b8217-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8217-128">Permission type</span></span> | <span data-ttu-id="b8217-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8217-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="b8217-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8217-130">Delegated (work or school account)</span></span> | <span data-ttu-id="b8217-131">PrivilegedAccess.ReadWrite.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="b8217-131">PrivilegedAccess.ReadWrite.AzureADGroup</span></span> |
| <span data-ttu-id="b8217-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8217-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8217-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8217-133">Not supported.</span></span> |
| <span data-ttu-id="b8217-134">Application</span><span class="sxs-lookup"><span data-stu-id="b8217-134">Application</span></span> | <span data-ttu-id="b8217-135">PrivilegedAccess.Read.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="b8217-135">PrivilegedAccess.Read.AzureADGroup</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8217-136">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8217-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b8217-137">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b8217-137">Optional query parameters</span></span>
<span data-ttu-id="b8217-138">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b8217-138">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8217-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8217-139">Request headers</span></span>
| <span data-ttu-id="b8217-140">Nome</span><span class="sxs-lookup"><span data-stu-id="b8217-140">Name</span></span>      |<span data-ttu-id="b8217-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8217-141">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b8217-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8217-142">Authorization</span></span>  | <span data-ttu-id="b8217-143">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="b8217-143">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8217-144">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8217-144">Request body</span></span>
<span data-ttu-id="b8217-145">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8217-145">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b8217-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8217-146">Response</span></span>
<span data-ttu-id="b8217-147">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos governanceResource](../resources/governanceresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8217-147">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="b8217-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b8217-148">Examples</span></span>

<span data-ttu-id="b8217-149">Este exemplo lista todos os recursos que posso acessar no momento.</span><span class="sxs-lookup"><span data-stu-id="b8217-149">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="b8217-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8217-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b8217-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8217-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
# <a name="c"></a>[<span data-ttu-id="b8217-152">C#</span><span class="sxs-lookup"><span data-stu-id="b8217-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-governanceresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8217-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8217-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-governanceresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8217-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8217-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-governanceresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b8217-155">Java</span><span class="sxs-lookup"><span data-stu-id="b8217-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-governanceresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b8217-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8217-156">Response</span></span>
<span data-ttu-id="b8217-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8217-157">Here is an example of the response.</span></span> 

><span data-ttu-id="b8217-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b8217-158">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1289

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceResources",
    "value":[
        {
            "id": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/resourceGroups/AnujRG/providers/Microsoft.Storage/storageAccounts/anujstoragefimdev",
            "type": "Microsoft.Storage/storageAccounts",
            "displayName": "anujstoragefimdev",
            "status": "Active",
            "registeredDateTime": "2018-04-05T22:30:37.13Z",
            "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",  
        },
        {
            "id": "0e0e4461-0c46-4d13-bf69-7cacbec75471",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/resourceGroups/ARPJ-TESTRG-01/providers/Microsoft.Compute/virtualMachines/APRJ-VM-01-T",
            "type": "Microsoft.Compute/virtualMachines",
            "displayName": "APRJ-VM-01-T",
            "status": "Active",
            "registeredDateTime": "2018-04-05T22:30:37.13Z",
            "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",  
        },
        {
            "id": "c072eb85-e47b-4627-81cb-5af82a8fc9fb",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/resourceGroups/ARPJ-TESTRG-01/providers/Microsoft.Compute/virtualMachines/APRJ-VM-01-T/extensions/IaaSAntimalware",
            "type": "Microsoft.Compute/virtualMachines/extensions",
            "displayName": "APRJ-VM-01-T/IaaSAntimalware",
            "status": "Active",
            "registeredDateTime": "2018-04-05T22:30:37.13Z",
            "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",  
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List governanceResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


