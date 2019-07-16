---
title: 'Entidadegovernanceresource: Register'
description: Registrar um objeto Entidadegovernanceresource no PIM.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2b8457f7ddee4564ca6b6b300121ddb7b8247e34
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713916"
---
# <a name="governanceresource-register"></a><span data-ttu-id="f4714-103">Entidadegovernanceresource: Register</span><span class="sxs-lookup"><span data-stu-id="f4714-103">governanceResource: register</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4714-104">Registre um objeto [entidadegovernanceresource](../resources/governanceresource.md) no gerenciamento de identidade privilegiado.</span><span class="sxs-lookup"><span data-stu-id="f4714-104">Register a [governanceResource](../resources/governanceresource.md) object in Privileged Identity Management.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4714-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f4714-105">Permissions</span></span>

<span data-ttu-id="f4714-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4714-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="f4714-108">**Observação:** Essa API também exige que o solicitante tenha pelo menos uma atribuição de função ativa no recurso.</span><span class="sxs-lookup"><span data-stu-id="f4714-108">**Note:** This API also requires that the requester have at least one active role assignment on the resource.</span></span>

| <span data-ttu-id="f4714-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4714-109">Permission type</span></span> | <span data-ttu-id="f4714-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="f4714-110">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="f4714-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4714-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f4714-112">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="f4714-112">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="f4714-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4714-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4714-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4714-114">Not supported.</span></span> |
| <span data-ttu-id="f4714-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4714-115">Application</span></span> | <span data-ttu-id="f4714-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4714-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4714-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4714-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4714-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f4714-118">Optional query parameters</span></span>

<span data-ttu-id="f4714-119">Este método **só** oferece suporte `$select` a `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f4714-119">This method **only** supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4714-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4714-120">Request headers</span></span>

| <span data-ttu-id="f4714-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f4714-121">Name</span></span> | <span data-ttu-id="f4714-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4714-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="f4714-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4714-123">Authorization</span></span> | <span data-ttu-id="f4714-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="f4714-124">Bearer {token}</span></span> |
| <span data-ttu-id="f4714-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="f4714-125">Content-type</span></span> | <span data-ttu-id="f4714-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4714-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4714-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4714-127">Request body</span></span>

| <span data-ttu-id="f4714-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4714-128">Properties</span></span> | <span data-ttu-id="f4714-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4714-129">Type</span></span> | <span data-ttu-id="f4714-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4714-130">Description</span></span> |
|:---------- |:---- |:----------- |
| <span data-ttu-id="f4714-131">externalId</span><span class="sxs-lookup"><span data-stu-id="f4714-131">externalId</span></span> | <span data-ttu-id="f4714-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4714-132">String</span></span> | <span data-ttu-id="f4714-133">O identificador externo do recurso a ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="f4714-133">The external identifier of the resource to be registered in PIM.</span></span> <span data-ttu-id="f4714-134">Se estiver registrando uma assinatura, o identificador será o identificador de assinatura precedida por `/subscriptions/`.</span><span class="sxs-lookup"><span data-stu-id="f4714-134">If registering a subscription, the identifier is the subscription identifier prepended by `/subscriptions/`.</span></span> <span data-ttu-id="f4714-135">Por exemplo, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span><span class="sxs-lookup"><span data-stu-id="f4714-135">For example, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`.</span></span> |

## <a name="response"></a><span data-ttu-id="f4714-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4714-136">Response</span></span>

<span data-ttu-id="f4714-137">Se tiver êxito, este método retornará `200 OK` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="f4714-137">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="f4714-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4714-138">Example</span></span>

<span data-ttu-id="f4714-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f4714-139">The following example shows how to call this API.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a><span data-ttu-id="f4714-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4714-140">Request</span></span>
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a><span data-ttu-id="f4714-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4714-141">Response</span></span>
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
