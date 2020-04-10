---
title: 'Entidadegovernanceresource: Register'
description: Registrar um objeto Entidadegovernanceresource no PIM.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: d92b061dd726dcbcacf18213a303fac8f415c46e
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218910"
---
# <a name="governanceresource-register"></a><span data-ttu-id="f6a2a-103">Entidadegovernanceresource: Register</span><span class="sxs-lookup"><span data-stu-id="f6a2a-103">governanceResource: register</span></span>

<span data-ttu-id="f6a2a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6a2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6a2a-105">Registre um objeto [entidadegovernanceresource](../resources/governanceresource.md) no gerenciamento de identidade privilegiado.</span><span class="sxs-lookup"><span data-stu-id="f6a2a-105">Register a [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6a2a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f6a2a-106">Permissions</span></span>

<span data-ttu-id="f6a2a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6a2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="f6a2a-109">**Observação:** Essa API também exige que o solicitante tenha pelo menos uma atribuição de função ativa no recurso.</span><span class="sxs-lookup"><span data-stu-id="f6a2a-109">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

| <span data-ttu-id="f6a2a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6a2a-110">Permission type</span></span> | <span data-ttu-id="f6a2a-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="f6a2a-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="f6a2a-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6a2a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f6a2a-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f6a2a-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="f6a2a-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6a2a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6a2a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6a2a-115">Not supported.</span></span> |
| <span data-ttu-id="f6a2a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6a2a-116">Application</span></span> | <span data-ttu-id="f6a2a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6a2a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6a2a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6a2a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6a2a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f6a2a-119">Optional query parameters</span></span>

<span data-ttu-id="f6a2a-120">Este método **só** oferece suporte `$select` a `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f6a2a-120">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6a2a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6a2a-121">Request headers</span></span>

| <span data-ttu-id="f6a2a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f6a2a-122">Name</span></span> | <span data-ttu-id="f6a2a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6a2a-123">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="f6a2a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6a2a-124">Authorization</span></span> | <span data-ttu-id="f6a2a-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="f6a2a-125">Bearer {token}</span></span> |
| <span data-ttu-id="f6a2a-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="f6a2a-126">Content-type</span></span> | <span data-ttu-id="f6a2a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f6a2a-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6a2a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6a2a-128">Request body</span></span>

| <span data-ttu-id="f6a2a-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6a2a-129">Properties</span></span> | <span data-ttu-id="f6a2a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6a2a-130">Type</span></span> | <span data-ttu-id="f6a2a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6a2a-131">Description</span></span> |
|:---------- |:---- |:----------- |
| <span data-ttu-id="f6a2a-132">externalId</span><span class="sxs-lookup"><span data-stu-id="f6a2a-132">externalId</span></span> | <span data-ttu-id="f6a2a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6a2a-133">String</span></span> | <span data-ttu-id="f6a2a-134">O identificador externo do recurso a ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="f6a2a-134">The external identifier of the resource to be registered in PIM.</span></span> <span data-ttu-id="f6a2a-135">Se estiver registrando uma assinatura, o identificador será o identificador de assinatura precedida por `/subscriptions/`.</span><span class="sxs-lookup"><span data-stu-id="f6a2a-135">If registering a subscription, the identifier is the subscription identifier prepended by `/subscriptions/`.</span></span> <span data-ttu-id="f6a2a-136">Por exemplo, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span><span class="sxs-lookup"><span data-stu-id="f6a2a-136">For example, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span></span> |

## <a name="response"></a><span data-ttu-id="f6a2a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6a2a-137">Response</span></span>

<span data-ttu-id="f6a2a-138">Se tiver êxito, este método retornará `200 OK` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="f6a2a-138">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="f6a2a-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6a2a-139">Example</span></span>

<span data-ttu-id="f6a2a-140">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f6a2a-140">The following example shows how to call this API.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a><span data-ttu-id="f6a2a-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6a2a-141">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a><span data-ttu-id="f6a2a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6a2a-142">Response</span></span>
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
