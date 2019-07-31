---
title: 'Entidadegovernanceresource: Register'
description: Registrar um objeto Entidadegovernanceresource no PIM.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fc6f2dd3ab6ba4cddc1ba3b3cde0e80ff268bb70
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954274"
---
# <a name="governanceresource-register"></a><span data-ttu-id="aed0f-103">Entidadegovernanceresource: Register</span><span class="sxs-lookup"><span data-stu-id="aed0f-103">governanceResource: register</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aed0f-104">Registre um objeto [entidadegovernanceresource](../resources/governanceresource.md) no gerenciamento de identidade privilegiado.</span><span class="sxs-lookup"><span data-stu-id="aed0f-104">Register a [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="aed0f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="aed0f-105">Permissions</span></span>

<span data-ttu-id="aed0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aed0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="aed0f-108">**Observação:** Essa API também exige que o solicitante tenha pelo menos uma atribuição de função ativa no recurso.</span><span class="sxs-lookup"><span data-stu-id="aed0f-108">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

| <span data-ttu-id="aed0f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aed0f-109">Permission type</span></span> | <span data-ttu-id="aed0f-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="aed0f-110">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="aed0f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aed0f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aed0f-112">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="aed0f-112">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="aed0f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aed0f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aed0f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aed0f-114">Not supported.</span></span> |
| <span data-ttu-id="aed0f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aed0f-115">Application</span></span> | <span data-ttu-id="aed0f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aed0f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aed0f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aed0f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aed0f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aed0f-118">Optional query parameters</span></span>

<span data-ttu-id="aed0f-119">Este método **só** oferece suporte `$select` a `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aed0f-119">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aed0f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aed0f-120">Request headers</span></span>

| <span data-ttu-id="aed0f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="aed0f-121">Name</span></span> | <span data-ttu-id="aed0f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="aed0f-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="aed0f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aed0f-123">Authorization</span></span> | <span data-ttu-id="aed0f-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="aed0f-124">Bearer {token}</span></span> |
| <span data-ttu-id="aed0f-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="aed0f-125">Content-type</span></span> | <span data-ttu-id="aed0f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aed0f-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="aed0f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aed0f-127">Request body</span></span>

| <span data-ttu-id="aed0f-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aed0f-128">Properties</span></span> | <span data-ttu-id="aed0f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="aed0f-129">Type</span></span> | <span data-ttu-id="aed0f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="aed0f-130">Description</span></span> |
|:---------- |:---- |:----------- |
| <span data-ttu-id="aed0f-131">externalId</span><span class="sxs-lookup"><span data-stu-id="aed0f-131">externalId</span></span> | <span data-ttu-id="aed0f-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aed0f-132">String</span></span> | <span data-ttu-id="aed0f-133">O identificador externo do recurso a ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="aed0f-133">The external identifier of the resource to be registered in PIM.</span></span> <span data-ttu-id="aed0f-134">Se estiver registrando uma assinatura, o identificador será o identificador de assinatura precedida por `/subscriptions/`.</span><span class="sxs-lookup"><span data-stu-id="aed0f-134">If registering a subscription, the identifier is the subscription identifier prepended by `/subscriptions/`.</span></span> <span data-ttu-id="aed0f-135">Por exemplo, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span><span class="sxs-lookup"><span data-stu-id="aed0f-135">For example, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span></span> |

## <a name="response"></a><span data-ttu-id="aed0f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="aed0f-136">Response</span></span>

<span data-ttu-id="aed0f-137">Se tiver êxito, este método retornará `200 OK` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="aed0f-137">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="aed0f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aed0f-138">Example</span></span>

<span data-ttu-id="aed0f-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="aed0f-139">The following example shows how to call this API.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a><span data-ttu-id="aed0f-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aed0f-140">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a><span data-ttu-id="aed0f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="aed0f-141">Response</span></span>
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
