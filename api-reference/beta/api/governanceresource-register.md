---
title: Registrar governanceResource
description: Registre um objeto governanceResource não gerenciado no PIM.
localization_priority: Normal
ms.openlocfilehash: ce439d53eb9f017340f561ca509e8da43dbafbfc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837748"
---
# <a name="register-governanceresource"></a><span data-ttu-id="d246d-103">Registrar governanceResource</span><span class="sxs-lookup"><span data-stu-id="d246d-103">Register governanceResource</span></span>

> <span data-ttu-id="d246d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d246d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d246d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d246d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d246d-106">Registre um objeto não gerenciado [governanceResource](../resources/governanceresource.md) no gerenciamento de identidades privilegiado.</span><span class="sxs-lookup"><span data-stu-id="d246d-106">Register an unmanaged [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="d246d-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="d246d-107">Permissions</span></span>
<span data-ttu-id="d246d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d246d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="d246d-110">**Observação:** Essa API também requer que o solicitante tenha pelo menos uma atribuição de função ativa no recurso.</span><span class="sxs-lookup"><span data-stu-id="d246d-110">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

|<span data-ttu-id="d246d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d246d-111">Permission type</span></span>      | <span data-ttu-id="d246d-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="d246d-112">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d246d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d246d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d246d-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="d246d-114">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="d246d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d246d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d246d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d246d-116">Not supported.</span></span>    |
|<span data-ttu-id="d246d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d246d-117">Application</span></span> | <span data-ttu-id="d246d-118">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="d246d-118">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="d246d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d246d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a><span data-ttu-id="d246d-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d246d-120">Optional query parameters</span></span>
<span data-ttu-id="d246d-121">Este método **só** oferece suporte a `$select` e `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d246d-121">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="request-headers"></a><span data-ttu-id="d246d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d246d-122">Request headers</span></span>
| <span data-ttu-id="d246d-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d246d-123">Name</span></span>      |<span data-ttu-id="d246d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d246d-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d246d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d246d-125">Authorization</span></span>  | <span data-ttu-id="d246d-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d246d-126">Bearer {code}</span></span>|
| <span data-ttu-id="d246d-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="d246d-127">Content-type</span></span>  | <span data-ttu-id="d246d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d246d-128">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="d246d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d246d-129">Request body</span></span>

|<span data-ttu-id="d246d-130">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="d246d-130">Parameters</span></span>      |<span data-ttu-id="d246d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d246d-131">Type</span></span>                 |<span data-ttu-id="d246d-132">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="d246d-132">Required</span></span> |<span data-ttu-id="d246d-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d246d-133">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="d246d-134">externalId</span><span class="sxs-lookup"><span data-stu-id="d246d-134">externalId</span></span>    |<span data-ttu-id="d246d-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d246d-135">String</span></span>                 |<span data-ttu-id="d246d-136">✓</span><span class="sxs-lookup"><span data-stu-id="d246d-136">✓</span></span>        |<span data-ttu-id="d246d-137">ExternalId do recurso a ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="d246d-137">The externalId of the resource to be registered in PIM.</span></span>|

### <a name="response"></a><span data-ttu-id="d246d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d246d-138">Response</span></span>
<span data-ttu-id="d246d-139">Se tiver êxito, este método retornará um `200 OK` resposta.</span><span class="sxs-lookup"><span data-stu-id="d246d-139">If successful, this method returns a `200 OK` response.</span></span>

### <a name="example"></a><span data-ttu-id="d246d-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d246d-140">Example</span></span>
<span data-ttu-id="d246d-141">Este exemplo mostra como registrar uma assinatura do Azure Wingtip Toys - produção.</span><span class="sxs-lookup"><span data-stu-id="d246d-141">This example shows how to register an Azure subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="d246d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d246d-142">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a><span data-ttu-id="d246d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d246d-143">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
