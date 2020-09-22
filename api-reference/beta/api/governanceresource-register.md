---
title: 'Entidadegovernanceresource: Register'
description: Registrar um objeto Entidadegovernanceresource no PIM.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 207a733e72dcf7c05c6cdf81dddb3cecf37e3bdd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991170"
---
# <a name="governanceresource-register"></a><span data-ttu-id="abda3-103">Entidadegovernanceresource: Register</span><span class="sxs-lookup"><span data-stu-id="abda3-103">governanceResource: register</span></span>

<span data-ttu-id="abda3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abda3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abda3-105">Registre um objeto [entidadegovernanceresource](../resources/governanceresource.md) no gerenciamento de identidade privilegiado.</span><span class="sxs-lookup"><span data-stu-id="abda3-105">Register a [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="abda3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="abda3-106">Permissions</span></span>

<span data-ttu-id="abda3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abda3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="abda3-109">**Observação:** Essa API também exige que o solicitante tenha pelo menos uma atribuição de função ativa no recurso.</span><span class="sxs-lookup"><span data-stu-id="abda3-109">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

| <span data-ttu-id="abda3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abda3-110">Permission type</span></span> | <span data-ttu-id="abda3-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="abda3-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="abda3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abda3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="abda3-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="abda3-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="abda3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abda3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abda3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abda3-115">Not supported.</span></span> |
| <span data-ttu-id="abda3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abda3-116">Application</span></span> | <span data-ttu-id="abda3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abda3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="abda3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abda3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a><span data-ttu-id="abda3-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="abda3-119">Optional query parameters</span></span>

<span data-ttu-id="abda3-120">Este método **só** oferece suporte `$select` a `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="abda3-120">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="abda3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abda3-121">Request headers</span></span>

| <span data-ttu-id="abda3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="abda3-122">Name</span></span> | <span data-ttu-id="abda3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="abda3-123">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="abda3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="abda3-124">Authorization</span></span> | <span data-ttu-id="abda3-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="abda3-125">Bearer {token}</span></span> |
| <span data-ttu-id="abda3-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="abda3-126">Content-type</span></span> | <span data-ttu-id="abda3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="abda3-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="abda3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abda3-128">Request body</span></span>

| <span data-ttu-id="abda3-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="abda3-129">Properties</span></span> | <span data-ttu-id="abda3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="abda3-130">Type</span></span> | <span data-ttu-id="abda3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="abda3-131">Description</span></span> |
|:---------- |:---- |:----------- |
| <span data-ttu-id="abda3-132">externalId</span><span class="sxs-lookup"><span data-stu-id="abda3-132">externalId</span></span> | <span data-ttu-id="abda3-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abda3-133">String</span></span> | <span data-ttu-id="abda3-134">O identificador externo do recurso a ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="abda3-134">The external identifier of the resource to be registered in PIM.</span></span> <span data-ttu-id="abda3-135">Se estiver registrando uma assinatura, o identificador será o identificador de assinatura precedida por `/subscriptions/` .</span><span class="sxs-lookup"><span data-stu-id="abda3-135">If registering a subscription, the identifier is the subscription identifier prepended by `/subscriptions/`.</span></span> <span data-ttu-id="abda3-136">Por exemplo, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span><span class="sxs-lookup"><span data-stu-id="abda3-136">For example, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span></span> |

## <a name="response"></a><span data-ttu-id="abda3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="abda3-137">Response</span></span>

<span data-ttu-id="abda3-138">Se tiver êxito, este método retornará uma `200 OK` resposta.</span><span class="sxs-lookup"><span data-stu-id="abda3-138">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="abda3-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abda3-139">Example</span></span>

<span data-ttu-id="abda3-140">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="abda3-140">The following example shows how to call this API.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a><span data-ttu-id="abda3-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abda3-141">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a><span data-ttu-id="abda3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="abda3-142">Response</span></span>
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


