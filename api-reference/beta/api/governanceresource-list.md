---
title: Listar governanceResources
description: Recupere uma coleção de Entidadegovernanceresource à qual o solicitante tem acesso.
localization_priority: Normal
ms.openlocfilehash: 998e18a0139f0cbe41901da935faee2f7f24e9eb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457169"
---
# <a name="list-governanceresources"></a><span data-ttu-id="8548e-103">Listar governanceResources</span><span class="sxs-lookup"><span data-stu-id="8548e-103">List governanceResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8548e-104">Recupere uma coleção de [entidadegovernanceresource](../resources/governanceresource.md) à qual o solicitante tem acesso.</span><span class="sxs-lookup"><span data-stu-id="8548e-104">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="8548e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8548e-105">Permissions</span></span>
<span data-ttu-id="8548e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8548e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8548e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8548e-108">Permission type</span></span>      | <span data-ttu-id="8548e-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="8548e-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8548e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8548e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8548e-111">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="8548e-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="8548e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8548e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8548e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8548e-113">Not supported.</span></span>    |
|<span data-ttu-id="8548e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8548e-114">Application</span></span> | <span data-ttu-id="8548e-115">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="8548e-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="8548e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8548e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8548e-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8548e-117">Optional query parameters</span></span>
<span data-ttu-id="8548e-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8548e-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8548e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8548e-119">Request headers</span></span>
| <span data-ttu-id="8548e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8548e-120">Name</span></span>      |<span data-ttu-id="8548e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8548e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8548e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8548e-122">Authorization</span></span>  | <span data-ttu-id="8548e-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="8548e-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8548e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8548e-124">Request body</span></span>
<span data-ttu-id="8548e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8548e-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8548e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="8548e-126">Response</span></span>
<span data-ttu-id="8548e-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [entidadegovernanceresource](../resources/governanceresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8548e-127">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="8548e-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8548e-128">Examples</span></span>

<span data-ttu-id="8548e-129">Este exemplo lista todos os recursos que eu posso acessar no momento.</span><span class="sxs-lookup"><span data-stu-id="8548e-129">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="8548e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8548e-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
##### <a name="response"></a><span data-ttu-id="8548e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8548e-131">Response</span></span>
<span data-ttu-id="8548e-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8548e-132">Here is an example of the response.</span></span> 

><span data-ttu-id="8548e-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8548e-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/governanceresource-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
