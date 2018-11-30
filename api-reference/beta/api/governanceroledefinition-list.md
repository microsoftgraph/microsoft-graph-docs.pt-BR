---
title: Lista governanceRoleDefinitions
description: Obtenha uma coleção de governanceRoleDefinitions em um recurso.
ms.openlocfilehash: ed1d4e7b51d20ed6687c52364399385054db9912
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037777"
---
# <a name="list-governanceroledefinitions"></a><span data-ttu-id="740aa-103">Lista governanceRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="740aa-103">List governanceRoleDefinitions</span></span>
> <span data-ttu-id="740aa-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="740aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="740aa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="740aa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="740aa-106">Obtenha uma coleção de [governanceRoleDefinitions](../resources/governanceroledefinition.md) em um recurso.</span><span class="sxs-lookup"><span data-stu-id="740aa-106">Get a collection of [governanceRoleDefinitions](../resources/governanceroledefinition.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="740aa-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="740aa-107">Permissions</span></span>
<span data-ttu-id="740aa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="740aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="740aa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="740aa-110">Permission type</span></span>      | <span data-ttu-id="740aa-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="740aa-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="740aa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="740aa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="740aa-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="740aa-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="740aa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="740aa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="740aa-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="740aa-115">Not supported.</span></span>    |
|<span data-ttu-id="740aa-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="740aa-116">Application</span></span> | <span data-ttu-id="740aa-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="740aa-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="740aa-118">Além do escopo de permissão, essa API requer o solicitante ter pelo menos uma atribuição no recurso.</span><span class="sxs-lookup"><span data-stu-id="740aa-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="740aa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="740aa-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions
GET /privilegedAccess/azureResources/roleDefinitions?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="740aa-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="740aa-120">Optional query parameters</span></span>
<span data-ttu-id="740aa-121">Este método oferece suporte para os [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="740aa-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="740aa-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="740aa-122">Request headers</span></span>
| <span data-ttu-id="740aa-123">Nome</span><span class="sxs-lookup"><span data-stu-id="740aa-123">Name</span></span>      |<span data-ttu-id="740aa-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="740aa-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="740aa-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="740aa-125">Authorization</span></span>  | <span data-ttu-id="740aa-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="740aa-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="740aa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="740aa-127">Request body</span></span>
<span data-ttu-id="740aa-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="740aa-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="740aa-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="740aa-129">Response</span></span>
<span data-ttu-id="740aa-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [governanceRoleDefinition](../resources/governanceroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="740aa-130">If successful, this method returns a `200 OK` response code and collection of [governanceRoleDefinition](../resources/governanceroledefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="740aa-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="740aa-131">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinitions"
}-->
<span data-ttu-id="740aa-132">Este exemplo mostra como obter todas as definições de função da assinatura Wingtip Toys - produção.</span><span class="sxs-lookup"><span data-stu-id="740aa-132">This example shows how to get all role definitions of the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="740aa-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="740aa-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions  
```
##### <a name="response"></a><span data-ttu-id="740aa-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="740aa-134">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List governanceRoleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
