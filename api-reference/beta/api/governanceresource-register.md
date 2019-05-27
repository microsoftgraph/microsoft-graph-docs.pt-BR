---
title: Registrar Entidadegovernanceresource
description: Registre um objeto Entidadegovernanceresource não gerenciado no PIM.
localization_priority: Normal
ms.openlocfilehash: 814ccd84d449f20882e1febbf0d48216ba3f5b89
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422455"
---
# <a name="register-governanceresource"></a><span data-ttu-id="a5335-103">Registrar Entidadegovernanceresource</span><span class="sxs-lookup"><span data-stu-id="a5335-103">Register governanceResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5335-104">Registre um objeto [entidadegovernanceresource](../resources/governanceresource.md) não gerenciado no gerenciamento de identidade privilegiado.</span><span class="sxs-lookup"><span data-stu-id="a5335-104">Register an unmanaged [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5335-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5335-105">Permissions</span></span>
<span data-ttu-id="a5335-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5335-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="a5335-108">**Observação:** Essa API também exige que o solicitante tenha pelo menos uma atribuição de função ativa no recurso.</span><span class="sxs-lookup"><span data-stu-id="a5335-108">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

|<span data-ttu-id="a5335-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5335-109">Permission type</span></span>      | <span data-ttu-id="a5335-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5335-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5335-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5335-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a5335-112">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="a5335-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="a5335-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5335-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5335-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5335-114">Not supported.</span></span>    |
|<span data-ttu-id="a5335-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5335-115">Application</span></span> | <span data-ttu-id="a5335-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5335-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5335-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5335-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a><span data-ttu-id="a5335-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a5335-118">Optional query parameters</span></span>
<span data-ttu-id="a5335-119">Este método **só** oferece suporte `$select` a `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a5335-119">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="request-headers"></a><span data-ttu-id="a5335-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5335-120">Request headers</span></span>
| <span data-ttu-id="a5335-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a5335-121">Name</span></span>      |<span data-ttu-id="a5335-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5335-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a5335-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5335-123">Authorization</span></span>  | <span data-ttu-id="a5335-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a5335-124">Bearer {code}</span></span>|
| <span data-ttu-id="a5335-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="a5335-125">Content-type</span></span>  | <span data-ttu-id="a5335-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5335-126">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="a5335-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5335-127">Request body</span></span>

|<span data-ttu-id="a5335-128">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="a5335-128">Parameters</span></span>      |<span data-ttu-id="a5335-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5335-129">Type</span></span>                 |<span data-ttu-id="a5335-130">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="a5335-130">Required</span></span> |<span data-ttu-id="a5335-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5335-131">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="a5335-132">externalId</span><span class="sxs-lookup"><span data-stu-id="a5335-132">externalId</span></span>    |<span data-ttu-id="a5335-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5335-133">String</span></span>                 |<span data-ttu-id="a5335-134">✓</span><span class="sxs-lookup"><span data-stu-id="a5335-134">✓</span></span>        |<span data-ttu-id="a5335-135">ExternalId do recurso a ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="a5335-135">The externalId of the resource to be registered in PIM.</span></span>|

### <a name="response"></a><span data-ttu-id="a5335-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5335-136">Response</span></span>
<span data-ttu-id="a5335-137">Se tiver êxito, este método retornará `200 OK` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="a5335-137">If successful, this method returns a `200 OK` response.</span></span>

### <a name="example"></a><span data-ttu-id="a5335-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5335-138">Example</span></span>
<span data-ttu-id="a5335-139">Este exemplo mostra como registrar uma assinatura do Azure na Wingtip Toys-prod.</span><span class="sxs-lookup"><span data-stu-id="a5335-139">This example shows how to register an Azure subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="a5335-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5335-140">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a><span data-ttu-id="a5335-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5335-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
