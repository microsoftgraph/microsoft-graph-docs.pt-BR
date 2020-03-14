---
title: Obter Entidadegovernanceresource
description: Recupere as propriedades e os relacionamentos de um objeto Entidadegovernanceresource.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identitiy-platform
ms.openlocfilehash: 235b4cdfffd5573af5a5470ee5687e4a17ec42c6
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639874"
---
# <a name="get-governanceresource"></a><span data-ttu-id="ae693-103">Obter Entidadegovernanceresource</span><span class="sxs-lookup"><span data-stu-id="ae693-103">Get governanceResource</span></span>

<span data-ttu-id="ae693-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae693-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae693-105">Recupere as propriedades e os relacionamentos de um objeto [entidadegovernanceresource](../resources/governanceresource.md) .</span><span class="sxs-lookup"><span data-stu-id="ae693-105">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae693-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ae693-106">Permissions</span></span>
<span data-ttu-id="ae693-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae693-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae693-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae693-109">Permission type</span></span>      | <span data-ttu-id="ae693-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="ae693-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae693-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae693-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ae693-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="ae693-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="ae693-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae693-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae693-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae693-114">Not supported.</span></span>    |
|<span data-ttu-id="ae693-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae693-115">Application</span></span> | <span data-ttu-id="ae693-116">PrivilegedAccess. Read. AzureResources</span><span class="sxs-lookup"><span data-stu-id="ae693-116">PrivilegedAccess.Read.AzureResources</span></span> |

<span data-ttu-id="ae693-117">Além do escopo de permissão, essa API exige que o solicitante tenha pelo menos uma atribuição de função no recurso.</span><span class="sxs-lookup"><span data-stu-id="ae693-117">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="ae693-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae693-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae693-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ae693-119">Optional query parameters</span></span>
<span data-ttu-id="ae693-120">Este método **só** oferece `$select` suporte `$expand` a [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ae693-120">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae693-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae693-121">Request headers</span></span>
| <span data-ttu-id="ae693-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ae693-122">Name</span></span>      |<span data-ttu-id="ae693-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae693-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ae693-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae693-124">Authorization</span></span>  | <span data-ttu-id="ae693-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="ae693-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae693-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae693-126">Request body</span></span>
<span data-ttu-id="ae693-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ae693-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ae693-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae693-128">Response</span></span>
<span data-ttu-id="ae693-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [entidadegovernanceresource](../resources/governanceresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae693-129">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae693-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae693-130">Example</span></span>
<span data-ttu-id="ae693-131">Este exemplo mostra como obter os detalhes da assinatura Wingtip Toys-prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span><span class="sxs-lookup"><span data-stu-id="ae693-131">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="ae693-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae693-132">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="ae693-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae693-133">Response</span></span>
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
