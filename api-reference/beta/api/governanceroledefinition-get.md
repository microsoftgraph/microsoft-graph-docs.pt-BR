---
title: Obter governanceRoleDefinition
description: Recupere as propriedades e relacionamentos de um governanceRoleDefinition.
localization_priority: Normal
ms.openlocfilehash: 99f19e1942c198259d9df7dd6e0f9e5a7685bc09
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865062"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="d1583-103">Obter governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d1583-103">Get governanceRoleDefinition</span></span>

> <span data-ttu-id="d1583-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d1583-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1583-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d1583-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1583-106">Recupere as propriedades e relacionamentos de um [governanceRoleDefinition](../resources/governanceroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d1583-106">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d1583-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="d1583-107">Permissions</span></span>
<span data-ttu-id="d1583-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1583-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1583-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1583-110">Permission type</span></span>      | <span data-ttu-id="d1583-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="d1583-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1583-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1583-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d1583-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="d1583-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="d1583-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1583-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1583-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1583-115">Not supported.</span></span>    |
|<span data-ttu-id="d1583-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1583-116">Application</span></span> | <span data-ttu-id="d1583-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="d1583-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="d1583-118">Além do escopo de permissão, essa API requer o solicitante ter pelo menos uma atribuição do recurso, que pertence a [governanceRoleDefinition](../resources/governanceroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="d1583-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="d1583-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1583-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d1583-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d1583-120">Optional query parameters</span></span>
<span data-ttu-id="d1583-121">Esse método não **suporte os [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta** .</span><span class="sxs-lookup"><span data-stu-id="d1583-121">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1583-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1583-122">Request headers</span></span>
| <span data-ttu-id="d1583-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d1583-123">Name</span></span>      |<span data-ttu-id="d1583-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1583-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d1583-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1583-125">Authorization</span></span>  | <span data-ttu-id="d1583-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d1583-126">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="d1583-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1583-127">Request body</span></span>
<span data-ttu-id="d1583-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1583-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d1583-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1583-129">Response</span></span>
<span data-ttu-id="d1583-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [governanceRoleDefinition](../resources/governanceroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1583-130">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d1583-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1583-131">Example</span></span>
<span data-ttu-id="d1583-132">Este exemplo mostra como obter os detalhes da definição de função de Colaborador de zona de DNS na assinatura Wingtip Toys - produção.</span><span class="sxs-lookup"><span data-stu-id="d1583-132">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="d1583-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1583-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="d1583-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1583-134">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
