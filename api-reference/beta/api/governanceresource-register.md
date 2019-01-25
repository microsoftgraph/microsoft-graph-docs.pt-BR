---
title: Registrar governanceResource
description: Registre um objeto governanceResource não gerenciado no PIM.
localization_priority: Normal
ms.openlocfilehash: f65c8b5884f08377967d3418bade0d5fc70c2063
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519042"
---
# <a name="register-governanceresource"></a><span data-ttu-id="e0b18-103">Registrar governanceResource</span><span class="sxs-lookup"><span data-stu-id="e0b18-103">Register governanceResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0b18-104">Registre um objeto não gerenciado [governanceResource](../resources/governanceresource.md) no gerenciamento de identidades privilegiado.</span><span class="sxs-lookup"><span data-stu-id="e0b18-104">Register an unmanaged [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0b18-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0b18-105">Permissions</span></span>
<span data-ttu-id="e0b18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0b18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="e0b18-108">**Observação:** Essa API também requer que o solicitante tenha pelo menos uma atribuição de função ativa no recurso.</span><span class="sxs-lookup"><span data-stu-id="e0b18-108">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

|<span data-ttu-id="e0b18-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0b18-109">Permission type</span></span>      | <span data-ttu-id="e0b18-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0b18-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0b18-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0b18-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e0b18-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e0b18-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="e0b18-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0b18-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0b18-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0b18-114">Not supported.</span></span>    |
|<span data-ttu-id="e0b18-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0b18-115">Application</span></span> | <span data-ttu-id="e0b18-116">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e0b18-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0b18-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0b18-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a><span data-ttu-id="e0b18-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e0b18-118">Optional query parameters</span></span>
<span data-ttu-id="e0b18-119">Este método **só** oferece suporte a `$select` e `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e0b18-119">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="request-headers"></a><span data-ttu-id="e0b18-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0b18-120">Request headers</span></span>
| <span data-ttu-id="e0b18-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e0b18-121">Name</span></span>      |<span data-ttu-id="e0b18-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0b18-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0b18-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0b18-123">Authorization</span></span>  | <span data-ttu-id="e0b18-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="e0b18-124">Bearer {code}</span></span>|
| <span data-ttu-id="e0b18-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="e0b18-125">Content-type</span></span>  | <span data-ttu-id="e0b18-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0b18-126">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="e0b18-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0b18-127">Request body</span></span>

|<span data-ttu-id="e0b18-128">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="e0b18-128">Parameters</span></span>      |<span data-ttu-id="e0b18-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0b18-129">Type</span></span>                 |<span data-ttu-id="e0b18-130">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="e0b18-130">Required</span></span> |<span data-ttu-id="e0b18-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0b18-131">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="e0b18-132">externalId</span><span class="sxs-lookup"><span data-stu-id="e0b18-132">externalId</span></span>    |<span data-ttu-id="e0b18-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0b18-133">String</span></span>                 |<span data-ttu-id="e0b18-134">✓</span><span class="sxs-lookup"><span data-stu-id="e0b18-134">✓</span></span>        |<span data-ttu-id="e0b18-135">ExternalId do recurso a ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="e0b18-135">The externalId of the resource to be registered in PIM.</span></span>|

### <a name="response"></a><span data-ttu-id="e0b18-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0b18-136">Response</span></span>
<span data-ttu-id="e0b18-137">Se tiver êxito, este método retornará um `200 OK` resposta.</span><span class="sxs-lookup"><span data-stu-id="e0b18-137">If successful, this method returns a `200 OK` response.</span></span>

### <a name="example"></a><span data-ttu-id="e0b18-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0b18-138">Example</span></span>
<span data-ttu-id="e0b18-139">Este exemplo mostra como registrar uma assinatura do Azure Wingtip Toys - produção.</span><span class="sxs-lookup"><span data-stu-id="e0b18-139">This example shows how to register an Azure subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="e0b18-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0b18-140">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a><span data-ttu-id="e0b18-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0b18-141">Response</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/governanceresource-register.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
