---
title: Obter governanceResource
description: Recupere as propriedades e relacionamentos de um objeto governanceResource.
ms.openlocfilehash: 55fcea026a2816f33ab6064ea5828d3af4526690
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191078"
---
# <a name="get-governanceresource"></a><span data-ttu-id="80160-103">Obter governanceResource</span><span class="sxs-lookup"><span data-stu-id="80160-103">Get governanceResource</span></span>

> <span data-ttu-id="80160-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="80160-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80160-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="80160-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="80160-106">Recupere as propriedades e relacionamentos de um objeto [governanceResource](../resources/governanceresource.md) .</span><span class="sxs-lookup"><span data-stu-id="80160-106">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="80160-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="80160-107">Permissions</span></span>
<span data-ttu-id="80160-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80160-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80160-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80160-110">Permission type</span></span>      | <span data-ttu-id="80160-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="80160-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80160-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80160-112">Delegated (work or school account)</span></span> | <span data-ttu-id="80160-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="80160-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="80160-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80160-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80160-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80160-115">Not supported.</span></span>    |
|<span data-ttu-id="80160-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80160-116">Application</span></span> | <span data-ttu-id="80160-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="80160-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="80160-118">Além do escopo de permissão, essa API requer o solicitante ter pelo menos uma atribuição no recurso.</span><span class="sxs-lookup"><span data-stu-id="80160-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="80160-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80160-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="80160-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="80160-120">Optional query parameters</span></span>
<span data-ttu-id="80160-121">Este método **só** oferece suporte a `$select` e `$expand` [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="80160-121">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80160-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80160-122">Request headers</span></span>
| <span data-ttu-id="80160-123">Nome</span><span class="sxs-lookup"><span data-stu-id="80160-123">Name</span></span>      |<span data-ttu-id="80160-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="80160-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="80160-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="80160-125">Authorization</span></span>  | <span data-ttu-id="80160-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="80160-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="80160-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80160-127">Request body</span></span>
<span data-ttu-id="80160-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="80160-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="80160-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="80160-129">Response</span></span>
<span data-ttu-id="80160-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [governanceResource](../resources/governanceresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80160-130">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80160-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80160-131">Example</span></span>
<span data-ttu-id="80160-132">Este exemplo mostra como obter os detalhes da assinatura Wingtip Toys - produção (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span><span class="sxs-lookup"><span data-stu-id="80160-132">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="80160-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80160-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="80160-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="80160-134">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
