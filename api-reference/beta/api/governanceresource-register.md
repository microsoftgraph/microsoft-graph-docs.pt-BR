---
title: Registrar governanceResource
description: Registre um objeto governanceResource não gerenciado no PIM.
ms.openlocfilehash: 53452202b58c2d2187b6876eabfaae1ae646710d
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2018
ms.locfileid: "27195285"
---
# <a name="register-governanceresource"></a><span data-ttu-id="b1c78-103">Registrar governanceResource</span><span class="sxs-lookup"><span data-stu-id="b1c78-103">Register governanceResource</span></span>

> <span data-ttu-id="b1c78-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b1c78-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1c78-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b1c78-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1c78-106">Registre um objeto não gerenciado [governanceResource](../resources/governanceresource.md) no gerenciamento de identidades privilegiado.</span><span class="sxs-lookup"><span data-stu-id="b1c78-106">Register an unmanaged [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1c78-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1c78-107">Permissions</span></span>
<span data-ttu-id="b1c78-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1c78-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="b1c78-110">**Observação:** Essa API também requer que o solicitante tenha pelo menos uma atribuição de função ativa no recurso.</span><span class="sxs-lookup"><span data-stu-id="b1c78-110">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

|<span data-ttu-id="b1c78-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1c78-111">Permission type</span></span>      | <span data-ttu-id="b1c78-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1c78-112">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1c78-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1c78-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b1c78-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b1c78-114">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="b1c78-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1c78-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1c78-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1c78-116">Not supported.</span></span>    |
|<span data-ttu-id="b1c78-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1c78-117">Application</span></span> | <span data-ttu-id="b1c78-118">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b1c78-118">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1c78-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1c78-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a><span data-ttu-id="b1c78-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b1c78-120">Optional query parameters</span></span>
<span data-ttu-id="b1c78-121">Este método **só** oferece suporte a `$select` e `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b1c78-121">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="request-headers"></a><span data-ttu-id="b1c78-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1c78-122">Request headers</span></span>
| <span data-ttu-id="b1c78-123">Nome</span><span class="sxs-lookup"><span data-stu-id="b1c78-123">Name</span></span>      |<span data-ttu-id="b1c78-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1c78-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b1c78-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1c78-125">Authorization</span></span>  | <span data-ttu-id="b1c78-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="b1c78-126">Bearer {code}</span></span>|
| <span data-ttu-id="b1c78-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="b1c78-127">Content-type</span></span>  | <span data-ttu-id="b1c78-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b1c78-128">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="b1c78-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1c78-129">Request body</span></span>

|<span data-ttu-id="b1c78-130">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="b1c78-130">Parameters</span></span>      |<span data-ttu-id="b1c78-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1c78-131">Type</span></span>                 |<span data-ttu-id="b1c78-132">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="b1c78-132">Required</span></span> |<span data-ttu-id="b1c78-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1c78-133">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="b1c78-134">externalId</span><span class="sxs-lookup"><span data-stu-id="b1c78-134">externalId</span></span>    |<span data-ttu-id="b1c78-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1c78-135">String</span></span>                 |<span data-ttu-id="b1c78-136">✓</span><span class="sxs-lookup"><span data-stu-id="b1c78-136">✓</span></span>        |<span data-ttu-id="b1c78-137">ExternalId do recurso a ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="b1c78-137">The externalId of the resource to be registered in PIM.</span></span>|

### <a name="response"></a><span data-ttu-id="b1c78-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1c78-138">Response</span></span>
<span data-ttu-id="b1c78-139">Se tiver êxito, este método retornará um `200 OK` resposta.</span><span class="sxs-lookup"><span data-stu-id="b1c78-139">If successful, this method returns a `200 OK` response.</span></span>

### <a name="example"></a><span data-ttu-id="b1c78-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1c78-140">Example</span></span>
<span data-ttu-id="b1c78-141">Este exemplo mostra como registrar uma assinatura do Azure Wingtip Toys - produção.</span><span class="sxs-lookup"><span data-stu-id="b1c78-141">This example shows how to register an Azure subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="b1c78-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1c78-142">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a><span data-ttu-id="b1c78-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1c78-143">Response</span></span>
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
