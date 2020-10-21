---
title: 'Entidadegovernanceresource: Register'
description: Registrar um objeto Entidadegovernanceresource no PIM.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: df5e9a2d63c6a49a8eb7b8ab9b5ed88b4f50c577
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635055"
---
# <a name="governanceresource-register"></a><span data-ttu-id="1d80e-103">Entidadegovernanceresource: Register</span><span class="sxs-lookup"><span data-stu-id="1d80e-103">governanceResource: register</span></span>

<span data-ttu-id="1d80e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d80e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d80e-105">Registre um objeto [entidadegovernanceresource](../resources/governanceresource.md) no gerenciamento de identidade privilegiado.</span><span class="sxs-lookup"><span data-stu-id="1d80e-105">Register a [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d80e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d80e-106">Permissions</span></span>

<span data-ttu-id="1d80e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="1d80e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="1d80e-109">**Observação:** Essa API também exige que o solicitante tenha pelo menos uma atribuição de função ativa no recurso.</span><span class="sxs-lookup"><span data-stu-id="1d80e-109">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

### <a name="azure-resources"></a><span data-ttu-id="1d80e-110">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="1d80e-110">Azure resources</span></span>

| <span data-ttu-id="1d80e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d80e-111">Permission type</span></span> | <span data-ttu-id="1d80e-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d80e-112">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="1d80e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d80e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1d80e-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="1d80e-114">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="1d80e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d80e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d80e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d80e-116">Not supported.</span></span> |
| <span data-ttu-id="1d80e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d80e-117">Application</span></span> | <span data-ttu-id="1d80e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d80e-118">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="1d80e-119">Azure AD</span><span class="sxs-lookup"><span data-stu-id="1d80e-119">Azure AD</span></span>

| <span data-ttu-id="1d80e-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d80e-120">Permission type</span></span> | <span data-ttu-id="1d80e-121">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d80e-121">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="1d80e-122">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d80e-122">Delegated (work or school account)</span></span> | <span data-ttu-id="1d80e-123">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="1d80e-123">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="1d80e-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d80e-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d80e-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d80e-125">Not supported.</span></span> |
| <span data-ttu-id="1d80e-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d80e-126">Application</span></span> | <span data-ttu-id="1d80e-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d80e-127">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="1d80e-128">Grupos</span><span class="sxs-lookup"><span data-stu-id="1d80e-128">Groups</span></span>

|<span data-ttu-id="1d80e-129">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d80e-129">Permission type</span></span> | <span data-ttu-id="1d80e-130">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d80e-130">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="1d80e-131">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d80e-131">Delegated (work or school account)</span></span> | <span data-ttu-id="1d80e-132">PrivilegedAccess. ReadWrite. AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="1d80e-132">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="1d80e-133">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d80e-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d80e-134">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d80e-134">Not supported.</span></span> |
| <span data-ttu-id="1d80e-135">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d80e-135">Application</span></span> | <span data-ttu-id="1d80e-136">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d80e-136">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d80e-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d80e-137">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1d80e-138">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1d80e-138">Optional query parameters</span></span>

<span data-ttu-id="1d80e-139">Este método **só** oferece suporte `$select` a `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1d80e-139">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d80e-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d80e-140">Request headers</span></span>

| <span data-ttu-id="1d80e-141">Nome</span><span class="sxs-lookup"><span data-stu-id="1d80e-141">Name</span></span> | <span data-ttu-id="1d80e-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d80e-142">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="1d80e-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d80e-143">Authorization</span></span> | <span data-ttu-id="1d80e-144">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="1d80e-144">Bearer {token}</span></span> |
| <span data-ttu-id="1d80e-145">Content-type</span><span class="sxs-lookup"><span data-stu-id="1d80e-145">Content-type</span></span> | <span data-ttu-id="1d80e-146">application/json</span><span class="sxs-lookup"><span data-stu-id="1d80e-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d80e-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d80e-147">Request body</span></span>

| <span data-ttu-id="1d80e-148">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d80e-148">Properties</span></span> | <span data-ttu-id="1d80e-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d80e-149">Type</span></span> | <span data-ttu-id="1d80e-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d80e-150">Description</span></span> |
|:---------- |:---- |:----------- |
| <span data-ttu-id="1d80e-151">externalId</span><span class="sxs-lookup"><span data-stu-id="1d80e-151">externalId</span></span> | <span data-ttu-id="1d80e-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d80e-152">String</span></span> | <span data-ttu-id="1d80e-153">O identificador externo do recurso a ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="1d80e-153">The external identifier of the resource to be registered in PIM.</span></span> <span data-ttu-id="1d80e-154">Se estiver registrando uma assinatura, o identificador será o identificador de assinatura precedida por `/subscriptions/` .</span><span class="sxs-lookup"><span data-stu-id="1d80e-154">If registering a subscription, the identifier is the subscription identifier prepended by `/subscriptions/`.</span></span> <span data-ttu-id="1d80e-155">Por exemplo, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span><span class="sxs-lookup"><span data-stu-id="1d80e-155">For example, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span></span> |

## <a name="response"></a><span data-ttu-id="1d80e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d80e-156">Response</span></span>

<span data-ttu-id="1d80e-157">Se tiver êxito, este método retornará uma `200 OK` resposta.</span><span class="sxs-lookup"><span data-stu-id="1d80e-157">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="1d80e-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d80e-158">Example</span></span>

<span data-ttu-id="1d80e-159">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="1d80e-159">The following example shows how to call this API.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a><span data-ttu-id="1d80e-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d80e-160">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a><span data-ttu-id="1d80e-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d80e-161">Response</span></span>
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


