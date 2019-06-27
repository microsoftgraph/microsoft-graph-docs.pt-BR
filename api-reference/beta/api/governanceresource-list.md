---
title: Listar governanceResources
description: Recupere uma coleção de Entidadegovernanceresource à qual o solicitante tem acesso.
localization_priority: Normal
ms.openlocfilehash: d4ecd7c1b9c7ae3dcaa00ce22042efcf97deaccb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263522"
---
# <a name="list-governanceresources"></a><span data-ttu-id="3f219-103">Listar governanceResources</span><span class="sxs-lookup"><span data-stu-id="3f219-103">List governanceResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f219-104">Recupere uma coleção de [entidadegovernanceresource](../resources/governanceresource.md) à qual o solicitante tem acesso.</span><span class="sxs-lookup"><span data-stu-id="3f219-104">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f219-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3f219-105">Permissions</span></span>
<span data-ttu-id="3f219-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f219-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f219-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f219-108">Permission type</span></span>      | <span data-ttu-id="3f219-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="3f219-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f219-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f219-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3f219-111">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="3f219-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="3f219-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f219-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f219-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f219-113">Not supported.</span></span>    |
|<span data-ttu-id="3f219-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f219-114">Application</span></span> | <span data-ttu-id="3f219-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f219-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f219-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f219-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3f219-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3f219-117">Optional query parameters</span></span>
<span data-ttu-id="3f219-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3f219-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f219-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f219-119">Request headers</span></span>
| <span data-ttu-id="3f219-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3f219-120">Name</span></span>      |<span data-ttu-id="3f219-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f219-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3f219-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f219-122">Authorization</span></span>  | <span data-ttu-id="3f219-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="3f219-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f219-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f219-124">Request body</span></span>
<span data-ttu-id="3f219-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3f219-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3f219-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f219-126">Response</span></span>
<span data-ttu-id="3f219-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [entidadegovernanceresource](../resources/governanceresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f219-127">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="3f219-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3f219-128">Examples</span></span>

<span data-ttu-id="3f219-129">Este exemplo lista todos os recursos que eu posso acessar no momento.</span><span class="sxs-lookup"><span data-stu-id="3f219-129">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="3f219-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f219-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
##### <a name="response"></a><span data-ttu-id="3f219-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f219-131">Response</span></span>
<span data-ttu-id="3f219-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f219-132">Here is an example of the response.</span></span> 

><span data-ttu-id="3f219-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3f219-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3f219-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3f219-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3f219-136">C#</span><span class="sxs-lookup"><span data-stu-id="3f219-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_governanceresources-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3f219-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="3f219-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_governanceresources-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3f219-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3f219-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_governanceresources-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/governanceresource-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/governanceresource-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceresource-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
