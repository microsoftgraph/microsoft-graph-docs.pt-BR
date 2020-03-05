---
title: 'Entidadegovernanceresource: Register'
description: Registrar um objeto Entidadegovernanceresource no PIM.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9edd34e7d8bd0fc2bd94f7d6afc0f038d8a250fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421344"
---
# <a name="governanceresource-register"></a><span data-ttu-id="44cea-103">Entidadegovernanceresource: Register</span><span class="sxs-lookup"><span data-stu-id="44cea-103">governanceResource: register</span></span>

<span data-ttu-id="44cea-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="44cea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44cea-105">Registre um objeto [entidadegovernanceresource](../resources/governanceresource.md) no gerenciamento de identidade privilegiado.</span><span class="sxs-lookup"><span data-stu-id="44cea-105">Register a [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="44cea-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="44cea-106">Permissions</span></span>

<span data-ttu-id="44cea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44cea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="44cea-109">**Observação:** Essa API também exige que o solicitante tenha pelo menos uma atribuição de função ativa no recurso.</span><span class="sxs-lookup"><span data-stu-id="44cea-109">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

| <span data-ttu-id="44cea-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44cea-110">Permission type</span></span> | <span data-ttu-id="44cea-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="44cea-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="44cea-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44cea-112">Delegated (work or school account)</span></span> | <span data-ttu-id="44cea-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="44cea-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="44cea-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44cea-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44cea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44cea-115">Not supported.</span></span> |
| <span data-ttu-id="44cea-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44cea-116">Application</span></span> | <span data-ttu-id="44cea-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44cea-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44cea-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44cea-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a><span data-ttu-id="44cea-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="44cea-119">Optional query parameters</span></span>

<span data-ttu-id="44cea-120">Este método **só** oferece suporte `$select` a `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="44cea-120">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44cea-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44cea-121">Request headers</span></span>

| <span data-ttu-id="44cea-122">Nome</span><span class="sxs-lookup"><span data-stu-id="44cea-122">Name</span></span> | <span data-ttu-id="44cea-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="44cea-123">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="44cea-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="44cea-124">Authorization</span></span> | <span data-ttu-id="44cea-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="44cea-125">Bearer {token}</span></span> |
| <span data-ttu-id="44cea-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="44cea-126">Content-type</span></span> | <span data-ttu-id="44cea-127">application/json</span><span class="sxs-lookup"><span data-stu-id="44cea-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="44cea-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44cea-128">Request body</span></span>

| <span data-ttu-id="44cea-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44cea-129">Properties</span></span> | <span data-ttu-id="44cea-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="44cea-130">Type</span></span> | <span data-ttu-id="44cea-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="44cea-131">Description</span></span> |
|:---------- |:---- |:----------- |
| <span data-ttu-id="44cea-132">externalId</span><span class="sxs-lookup"><span data-stu-id="44cea-132">externalId</span></span> | <span data-ttu-id="44cea-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44cea-133">String</span></span> | <span data-ttu-id="44cea-134">O identificador externo do recurso a ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="44cea-134">The external identifier of the resource to be registered in PIM.</span></span> <span data-ttu-id="44cea-135">Se estiver registrando uma assinatura, o identificador será o identificador de assinatura precedida por `/subscriptions/`.</span><span class="sxs-lookup"><span data-stu-id="44cea-135">If registering a subscription, the identifier is the subscription identifier prepended by `/subscriptions/`.</span></span> <span data-ttu-id="44cea-136">Por exemplo, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span><span class="sxs-lookup"><span data-stu-id="44cea-136">For example, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span></span> |

## <a name="response"></a><span data-ttu-id="44cea-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="44cea-137">Response</span></span>

<span data-ttu-id="44cea-138">Se tiver êxito, este método retornará `200 OK` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="44cea-138">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="44cea-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44cea-139">Example</span></span>

<span data-ttu-id="44cea-140">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="44cea-140">The following example shows how to call this API.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a><span data-ttu-id="44cea-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44cea-141">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a><span data-ttu-id="44cea-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="44cea-142">Response</span></span>
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
