---
title: 'governanceResource: register'
description: Registre um objeto governanceResource no PIM.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 363ee47fcded93062b325f3f58df14dfa4a3c625
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350863"
---
# <a name="governanceresource-register"></a><span data-ttu-id="cde36-103">governanceResource: register</span><span class="sxs-lookup"><span data-stu-id="cde36-103">governanceResource: register</span></span>

<span data-ttu-id="cde36-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cde36-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cde36-105">Registre [um objeto governanceResource](../resources/governanceresource.md) no Privileged Identity Management.</span><span class="sxs-lookup"><span data-stu-id="cde36-105">Register a [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="cde36-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cde36-106">Permissions</span></span>

<span data-ttu-id="cde36-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="cde36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="cde36-109">**Observação:** Essa API também exige que o solicitante tenha pelo menos uma atribuição de função ativa no recurso.</span><span class="sxs-lookup"><span data-stu-id="cde36-109">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

### <a name="azure-resources"></a><span data-ttu-id="cde36-110">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="cde36-110">Azure resources</span></span>

| <span data-ttu-id="cde36-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cde36-111">Permission type</span></span> | <span data-ttu-id="cde36-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="cde36-112">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="cde36-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cde36-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cde36-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="cde36-114">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="cde36-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cde36-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cde36-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cde36-116">Not supported.</span></span> |
| <span data-ttu-id="cde36-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cde36-117">Application</span></span> | <span data-ttu-id="cde36-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cde36-118">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="cde36-119">Azure AD</span><span class="sxs-lookup"><span data-stu-id="cde36-119">Azure AD</span></span>

| <span data-ttu-id="cde36-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cde36-120">Permission type</span></span> | <span data-ttu-id="cde36-121">Permissões</span><span class="sxs-lookup"><span data-stu-id="cde36-121">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="cde36-122">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cde36-122">Delegated (work or school account)</span></span> | <span data-ttu-id="cde36-123">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="cde36-123">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="cde36-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cde36-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cde36-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cde36-125">Not supported.</span></span> |
| <span data-ttu-id="cde36-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cde36-126">Application</span></span> | <span data-ttu-id="cde36-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cde36-127">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="cde36-128">Grupos</span><span class="sxs-lookup"><span data-stu-id="cde36-128">Groups</span></span>

|<span data-ttu-id="cde36-129">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cde36-129">Permission type</span></span> | <span data-ttu-id="cde36-130">Permissões</span><span class="sxs-lookup"><span data-stu-id="cde36-130">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="cde36-131">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cde36-131">Delegated (work or school account)</span></span> | <span data-ttu-id="cde36-132">PrivilegedAccess.ReadWrite.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="cde36-132">PrivilegedAccess.ReadWrite.AzureADGroup</span></span> |
| <span data-ttu-id="cde36-133">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cde36-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cde36-134">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cde36-134">Not supported.</span></span> |
| <span data-ttu-id="cde36-135">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cde36-135">Application</span></span> | <span data-ttu-id="cde36-136">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cde36-136">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cde36-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cde36-137">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cde36-138">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cde36-138">Optional query parameters</span></span>

<span data-ttu-id="cde36-139">Esse método **só dá** suporte aos `$select` `$expand` [parâmetros de consulta e OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cde36-139">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cde36-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cde36-140">Request headers</span></span>

| <span data-ttu-id="cde36-141">Nome</span><span class="sxs-lookup"><span data-stu-id="cde36-141">Name</span></span> | <span data-ttu-id="cde36-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="cde36-142">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="cde36-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="cde36-143">Authorization</span></span> | <span data-ttu-id="cde36-144">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="cde36-144">Bearer {token}</span></span> |
| <span data-ttu-id="cde36-145">Content-type</span><span class="sxs-lookup"><span data-stu-id="cde36-145">Content-type</span></span> | <span data-ttu-id="cde36-146">application/json</span><span class="sxs-lookup"><span data-stu-id="cde36-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cde36-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cde36-147">Request body</span></span>

| <span data-ttu-id="cde36-148">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cde36-148">Properties</span></span> | <span data-ttu-id="cde36-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="cde36-149">Type</span></span> | <span data-ttu-id="cde36-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="cde36-150">Description</span></span> |
|:---------- |:---- |:----------- |
| <span data-ttu-id="cde36-151">externalId</span><span class="sxs-lookup"><span data-stu-id="cde36-151">externalId</span></span> | <span data-ttu-id="cde36-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cde36-152">String</span></span> | <span data-ttu-id="cde36-153">O identificador externo do recurso a ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="cde36-153">The external identifier of the resource to be registered in PIM.</span></span> <span data-ttu-id="cde36-154">Se registrar uma assinatura, o identificador será o identificador de assinatura pré-anexado por `/subscriptions/` .</span><span class="sxs-lookup"><span data-stu-id="cde36-154">If registering a subscription, the identifier is the subscription identifier prepended by `/subscriptions/`.</span></span> <span data-ttu-id="cde36-155">Por exemplo, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span><span class="sxs-lookup"><span data-stu-id="cde36-155">For example, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span></span> |

## <a name="response"></a><span data-ttu-id="cde36-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="cde36-156">Response</span></span>

<span data-ttu-id="cde36-157">Se tiver êxito, este método retornará uma `200 OK` resposta.</span><span class="sxs-lookup"><span data-stu-id="cde36-157">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="cde36-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cde36-158">Example</span></span>

<span data-ttu-id="cde36-159">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="cde36-159">The following example shows how to call this API.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a><span data-ttu-id="cde36-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cde36-160">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a><span data-ttu-id="cde36-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="cde36-161">Response</span></span>
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


