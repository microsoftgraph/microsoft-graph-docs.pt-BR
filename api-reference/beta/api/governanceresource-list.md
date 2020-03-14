---
title: Listar governanceResources
description: Recupere uma coleção de Entidadegovernanceresource à qual o solicitante tem acesso.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identitiy-platform
ms.openlocfilehash: 98c19e86b80a95d23e12508740f082370997f147
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639867"
---
# <a name="list-governanceresources"></a><span data-ttu-id="2e107-103">Listar governanceResources</span><span class="sxs-lookup"><span data-stu-id="2e107-103">List governanceResources</span></span>

<span data-ttu-id="2e107-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e107-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e107-105">Recupere uma coleção de [entidadegovernanceresource](../resources/governanceresource.md) à qual o solicitante tem acesso.</span><span class="sxs-lookup"><span data-stu-id="2e107-105">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e107-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e107-106">Permissions</span></span>
<span data-ttu-id="2e107-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e107-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e107-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e107-109">Permission type</span></span>      | <span data-ttu-id="2e107-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e107-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e107-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e107-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2e107-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="2e107-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="2e107-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e107-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e107-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e107-114">Not supported.</span></span>    |
|<span data-ttu-id="2e107-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e107-115">Application</span></span> | <span data-ttu-id="2e107-116">PrivilegedAccess. Read. AzureResources</span><span class="sxs-lookup"><span data-stu-id="2e107-116">PrivilegedAccess.Read.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e107-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e107-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2e107-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2e107-118">Optional query parameters</span></span>
<span data-ttu-id="2e107-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2e107-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e107-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e107-120">Request headers</span></span>
| <span data-ttu-id="2e107-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2e107-121">Name</span></span>      |<span data-ttu-id="2e107-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e107-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2e107-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e107-123">Authorization</span></span>  | <span data-ttu-id="2e107-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="2e107-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e107-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e107-125">Request body</span></span>
<span data-ttu-id="2e107-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2e107-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2e107-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e107-127">Response</span></span>
<span data-ttu-id="2e107-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [entidadegovernanceresource](../resources/governanceresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e107-128">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="2e107-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2e107-129">Examples</span></span>

<span data-ttu-id="2e107-130">Este exemplo lista todos os recursos que eu posso acessar no momento.</span><span class="sxs-lookup"><span data-stu-id="2e107-130">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="2e107-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e107-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2e107-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e107-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
# <a name="c"></a>[<span data-ttu-id="2e107-133">C#</span><span class="sxs-lookup"><span data-stu-id="2e107-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-governanceresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e107-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e107-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-governanceresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e107-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e107-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-governanceresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2e107-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e107-136">Response</span></span>
<span data-ttu-id="2e107-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e107-137">Here is an example of the response.</span></span> 

><span data-ttu-id="2e107-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e107-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
