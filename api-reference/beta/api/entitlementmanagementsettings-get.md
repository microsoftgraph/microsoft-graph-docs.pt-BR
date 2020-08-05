---
title: Obter entitlementManagementSettings
description: Recupere as propriedades do objeto entitlementManagementSettings.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e5a0e77a41ef3517eb55ab9669ab994f871024e1
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566884"
---
# <a name="get-entitlementmanagementsettings"></a><span data-ttu-id="220df-103">Obter entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="220df-103">Get entitlementManagementSettings</span></span>

<span data-ttu-id="220df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="220df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="220df-105">Recupere as propriedades de um objeto [entitlementManagementSettings](../resources/entitlementManagementSettings.md) .</span><span class="sxs-lookup"><span data-stu-id="220df-105">Retrieve the properties of an [entitlementManagementSettings](../resources/entitlementManagementSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="220df-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="220df-106">Permissions</span></span>

<span data-ttu-id="220df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="220df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="220df-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="220df-109">Permission type</span></span>                        | <span data-ttu-id="220df-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="220df-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="220df-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="220df-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="220df-112">EntitlementManagement. Read. All, EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="220df-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="220df-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="220df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="220df-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="220df-114">Not supported.</span></span> |
| <span data-ttu-id="220df-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="220df-115">Application</span></span>                            | <span data-ttu-id="220df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="220df-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="220df-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="220df-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="220df-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="220df-118">Optional query parameters</span></span>

<span data-ttu-id="220df-119">Este método não oferece suporte aos parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="220df-119">This method does not support the OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="220df-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="220df-120">Request headers</span></span>

| <span data-ttu-id="220df-121">Nome</span><span class="sxs-lookup"><span data-stu-id="220df-121">Name</span></span>      |<span data-ttu-id="220df-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="220df-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="220df-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="220df-123">Authorization</span></span> | <span data-ttu-id="220df-124">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="220df-124">Bearer \{token\}.</span></span> <span data-ttu-id="220df-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="220df-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="220df-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="220df-126">Request body</span></span>

<span data-ttu-id="220df-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="220df-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="220df-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="220df-128">Response</span></span>

<span data-ttu-id="220df-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [entitlementManagementSettings](../resources/entitlementManagementSettings.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="220df-129">If successful, this method returns a `200 OK` response code and the requested [entitlementManagementSettings](../resources/entitlementManagementSettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="220df-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="220df-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="220df-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="220df-131">Request</span></span>

<span data-ttu-id="220df-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="220df-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="220df-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="220df-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_entitlementManagementSettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/settings
```
# <a name="c"></a>[<span data-ttu-id="220df-134">C#</span><span class="sxs-lookup"><span data-stu-id="220df-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-entitlementmanagementsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="220df-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="220df-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-entitlementmanagementsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="220df-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="220df-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-entitlementmanagementsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="220df-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="220df-137">Response</span></span>

<span data-ttu-id="220df-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="220df-138">The following is an example of the response.</span></span>

> <span data-ttu-id="220df-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="220df-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entitlementManagementSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "externalUserLifecycleAction": "None",
  "daysUntilExternalUserDeletedAfterBlocked": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get entitlementManagementSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
