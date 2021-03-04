---
title: Obter direitosManagementSettings
description: Recupere as propriedades do objeto entitlementManagementSettings.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1bc8fd3682fbe365ee083eec369957f197c3feea
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436299"
---
# <a name="get-entitlementmanagementsettings"></a><span data-ttu-id="c2eca-103">Obter direitosManagementSettings</span><span class="sxs-lookup"><span data-stu-id="c2eca-103">Get entitlementManagementSettings</span></span>

<span data-ttu-id="c2eca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2eca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2eca-105">Recupere as propriedades de [um objeto entitlementManagementSettings.](../resources/entitlementManagementSettings.md)</span><span class="sxs-lookup"><span data-stu-id="c2eca-105">Retrieve the properties of an [entitlementManagementSettings](../resources/entitlementManagementSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2eca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2eca-106">Permissions</span></span>

<span data-ttu-id="c2eca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2eca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2eca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2eca-109">Permission type</span></span>                        | <span data-ttu-id="c2eca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2eca-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c2eca-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2eca-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2eca-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2eca-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="c2eca-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2eca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2eca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2eca-114">Not supported.</span></span> |
| <span data-ttu-id="c2eca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2eca-115">Application</span></span>                            | <span data-ttu-id="c2eca-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2eca-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2eca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2eca-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c2eca-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c2eca-118">Optional query parameters</span></span>

<span data-ttu-id="c2eca-119">Este método não é compatível com os Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c2eca-119">This method does not support the OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2eca-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2eca-120">Request headers</span></span>

| <span data-ttu-id="c2eca-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c2eca-121">Name</span></span>      |<span data-ttu-id="c2eca-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2eca-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c2eca-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2eca-123">Authorization</span></span> | <span data-ttu-id="c2eca-124">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="c2eca-124">Bearer \{token\}.</span></span> <span data-ttu-id="c2eca-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2eca-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2eca-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2eca-126">Request body</span></span>

<span data-ttu-id="c2eca-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2eca-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2eca-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2eca-128">Response</span></span>

<span data-ttu-id="c2eca-129">Se tiver êxito, este método retornará um código de resposta e o objeto `200 OK` [requested entitlementManagementSettings](../resources/entitlementManagementSettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2eca-129">If successful, this method returns a `200 OK` response code and the requested [entitlementManagementSettings](../resources/entitlementManagementSettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c2eca-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c2eca-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c2eca-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2eca-131">Request</span></span>

<span data-ttu-id="c2eca-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2eca-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c2eca-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2eca-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_entitlementManagementSettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/settings
```
# <a name="c"></a>[<span data-ttu-id="c2eca-134">C#</span><span class="sxs-lookup"><span data-stu-id="c2eca-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-entitlementmanagementsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2eca-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2eca-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-entitlementmanagementsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2eca-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2eca-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-entitlementmanagementsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2eca-137">Java</span><span class="sxs-lookup"><span data-stu-id="c2eca-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-entitlementmanagementsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c2eca-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2eca-138">Response</span></span>

<span data-ttu-id="c2eca-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c2eca-139">The following is an example of the response.</span></span>

> <span data-ttu-id="c2eca-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2eca-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


