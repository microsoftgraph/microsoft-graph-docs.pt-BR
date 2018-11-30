---
title: Obter governanceResource
description: Recupere as propriedades e relacionamentos de um objeto governanceResource.
ms.openlocfilehash: d871dbe91b82cebc01a8c282c0afdfbd8701c8f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033591"
---
# <a name="get-governanceresource"></a><span data-ttu-id="c31fd-103">Obter governanceResource</span><span class="sxs-lookup"><span data-stu-id="c31fd-103">Get governanceResource</span></span>

> <span data-ttu-id="c31fd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c31fd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c31fd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c31fd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c31fd-106">Recupere as propriedades e relacionamentos de um objeto [governanceResource](../resources/governanceresource.md) .</span><span class="sxs-lookup"><span data-stu-id="c31fd-106">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c31fd-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="c31fd-107">Permissions</span></span>
<span data-ttu-id="c31fd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c31fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c31fd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c31fd-110">Permission type</span></span>      | <span data-ttu-id="c31fd-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="c31fd-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c31fd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c31fd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c31fd-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c31fd-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="c31fd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c31fd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c31fd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c31fd-115">Not supported.</span></span>    |
|<span data-ttu-id="c31fd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c31fd-116">Application</span></span> | <span data-ttu-id="c31fd-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c31fd-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="c31fd-118">Além do escopo de permissão, essa API requer o solicitante ter pelo menos uma atribuição no recurso.</span><span class="sxs-lookup"><span data-stu-id="c31fd-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="c31fd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c31fd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c31fd-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c31fd-120">Optional query parameters</span></span>
<span data-ttu-id="c31fd-121">Este método **só** oferece suporte a `$select` e `$expand` [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c31fd-121">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c31fd-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c31fd-122">Request headers</span></span>
| <span data-ttu-id="c31fd-123">Nome</span><span class="sxs-lookup"><span data-stu-id="c31fd-123">Name</span></span>      |<span data-ttu-id="c31fd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c31fd-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c31fd-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c31fd-125">Authorization</span></span>  | <span data-ttu-id="c31fd-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="c31fd-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c31fd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c31fd-127">Request body</span></span>
<span data-ttu-id="c31fd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c31fd-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c31fd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c31fd-129">Response</span></span>
<span data-ttu-id="c31fd-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [governanceResource](../resources/governanceresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c31fd-130">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c31fd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c31fd-131">Example</span></span>
<span data-ttu-id="c31fd-132">Este exemplo mostra como obter os detalhes da assinatura Wingtip Toys - produção (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span><span class="sxs-lookup"><span data-stu-id="c31fd-132">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="c31fd-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c31fd-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="c31fd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c31fd-134">Response</span></span>
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
    "onboardDateTime": "2018-04-05T22:30:37.13Z"
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
