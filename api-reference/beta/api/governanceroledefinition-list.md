---
title: Listar governanceRoleDefinitions
description: Obtenha uma coleção de governanceRoleDefinitions em um recurso.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identitiy-platform
ms.openlocfilehash: 93702d24229f0e3a86c5b999cdbd2074c6a357e8
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639671"
---
# <a name="list-governanceroledefinitions"></a><span data-ttu-id="fe178-103">Listar governanceRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="fe178-103">List governanceRoleDefinitions</span></span>

<span data-ttu-id="fe178-104">Namespace: Microsoft. Graph[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="fe178-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="fe178-105">Obtenha uma coleção de [governanceRoleDefinitions](../resources/governanceroledefinition.md) em um recurso.</span><span class="sxs-lookup"><span data-stu-id="fe178-105">Get a collection of [governanceRoleDefinitions](../resources/governanceroledefinition.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe178-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe178-106">Permissions</span></span>
<span data-ttu-id="fe178-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe178-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe178-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe178-109">Permission type</span></span>      | <span data-ttu-id="fe178-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe178-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe178-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe178-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fe178-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="fe178-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="fe178-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe178-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe178-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe178-114">Not supported.</span></span>    |
|<span data-ttu-id="fe178-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe178-115">Application</span></span> | <span data-ttu-id="fe178-116">PrivilegedAccess. Read. AzureResources</span><span class="sxs-lookup"><span data-stu-id="fe178-116">PrivilegedAccess.Read.AzureResources</span></span> |

<span data-ttu-id="fe178-117">Além do escopo de permissão, essa API exige que o solicitante tenha pelo menos uma atribuição de função no recurso.</span><span class="sxs-lookup"><span data-stu-id="fe178-117">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="fe178-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe178-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions
GET /privilegedAccess/azureResources/roleDefinitions?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fe178-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fe178-119">Optional query parameters</span></span>
<span data-ttu-id="fe178-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fe178-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe178-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe178-121">Request headers</span></span>
| <span data-ttu-id="fe178-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fe178-122">Name</span></span>      |<span data-ttu-id="fe178-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe178-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fe178-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe178-124">Authorization</span></span>  | <span data-ttu-id="fe178-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="fe178-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe178-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe178-126">Request body</span></span>
<span data-ttu-id="fe178-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe178-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fe178-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe178-128">Response</span></span>
<span data-ttu-id="fe178-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [governanceRoleDefinition](../resources/governanceroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe178-129">If successful, this method returns a `200 OK` response code and collection of [governanceRoleDefinition](../resources/governanceroledefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fe178-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe178-130">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinitions"
}-->
<span data-ttu-id="fe178-131">Este exemplo mostra como obter todas as definições de função da assinatura Wingtip Toys-prod.</span><span class="sxs-lookup"><span data-stu-id="fe178-131">This example shows how to get all role definitions of the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="fe178-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe178-132">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions  
```
##### <a name="response"></a><span data-ttu-id="fe178-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe178-133">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List governanceRoleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
