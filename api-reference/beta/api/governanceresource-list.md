---
title: Lista governanceResources
description: Recupere uma coleção de governanceResource que o solicitante tem acesso.
localization_priority: Normal
ms.openlocfilehash: 4527c7a5f59832fe69181a815af40a0e0e073c90
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838294"
---
# <a name="list-governanceresources"></a><span data-ttu-id="9d442-103">Lista governanceResources</span><span class="sxs-lookup"><span data-stu-id="9d442-103">List governanceResources</span></span>

> <span data-ttu-id="9d442-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9d442-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d442-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9d442-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d442-106">Recupere uma coleção de [governanceResource](../resources/governanceresource.md) que o solicitante tem acesso.</span><span class="sxs-lookup"><span data-stu-id="9d442-106">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d442-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="9d442-107">Permissions</span></span>
<span data-ttu-id="9d442-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d442-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d442-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d442-110">Permission type</span></span>      | <span data-ttu-id="9d442-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="9d442-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d442-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d442-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9d442-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9d442-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="9d442-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d442-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d442-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d442-115">Not supported.</span></span>    |
|<span data-ttu-id="9d442-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d442-116">Application</span></span> | <span data-ttu-id="9d442-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9d442-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d442-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d442-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9d442-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9d442-119">Optional query parameters</span></span>
<span data-ttu-id="9d442-120">Este método oferece suporte para os [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9d442-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d442-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d442-121">Request headers</span></span>
| <span data-ttu-id="9d442-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9d442-122">Name</span></span>      |<span data-ttu-id="9d442-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d442-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9d442-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d442-124">Authorization</span></span>  | <span data-ttu-id="9d442-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9d442-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d442-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d442-126">Request body</span></span>
<span data-ttu-id="9d442-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9d442-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9d442-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d442-128">Response</span></span>
<span data-ttu-id="9d442-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [governanceResource](../resources/governanceresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d442-129">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="9d442-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9d442-130">Examples</span></span>

<span data-ttu-id="9d442-131">Este exemplo lista todos os recursos que podem acessar no momento.</span><span class="sxs-lookup"><span data-stu-id="9d442-131">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="9d442-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d442-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
##### <a name="response"></a><span data-ttu-id="9d442-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d442-133">Response</span></span>
<span data-ttu-id="9d442-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d442-134">Here is an example of the response.</span></span> 

><span data-ttu-id="9d442-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d442-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List governanceResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
