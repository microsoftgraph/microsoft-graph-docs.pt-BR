---
title: Obter direitosManagementSettings
description: Recupere as propriedades do objeto entitlementManagementSettings.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 398a0f75fd4cbf606cbc5c54c509ade4191fb9f2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042622"
---
# <a name="get-entitlementmanagementsettings"></a><span data-ttu-id="22433-103">Obter direitosManagementSettings</span><span class="sxs-lookup"><span data-stu-id="22433-103">Get entitlementManagementSettings</span></span>

<span data-ttu-id="22433-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22433-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22433-105">Recupere as propriedades de [um objeto entitlementManagementSettings.](../resources/entitlementManagementSettings.md)</span><span class="sxs-lookup"><span data-stu-id="22433-105">Retrieve the properties of an [entitlementManagementSettings](../resources/entitlementManagementSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22433-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="22433-106">Permissions</span></span>

<span data-ttu-id="22433-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22433-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22433-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22433-109">Permission type</span></span>                        | <span data-ttu-id="22433-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22433-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="22433-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22433-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="22433-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22433-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="22433-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22433-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22433-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22433-114">Not supported.</span></span> |
| <span data-ttu-id="22433-115">Application</span><span class="sxs-lookup"><span data-stu-id="22433-115">Application</span></span>                            | <span data-ttu-id="22433-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22433-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="22433-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22433-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22433-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="22433-118">Optional query parameters</span></span>

<span data-ttu-id="22433-119">Este método não é compatível com os Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="22433-119">This method does not support the OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22433-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22433-120">Request headers</span></span>

| <span data-ttu-id="22433-121">Nome</span><span class="sxs-lookup"><span data-stu-id="22433-121">Name</span></span>      |<span data-ttu-id="22433-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="22433-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="22433-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="22433-123">Authorization</span></span> | <span data-ttu-id="22433-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22433-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22433-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22433-126">Request body</span></span>

<span data-ttu-id="22433-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22433-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22433-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="22433-128">Response</span></span>

<span data-ttu-id="22433-129">Se tiver êxito, este método retornará um código de resposta e o objeto `200 OK` [requested entitlementManagementSettings](../resources/entitlementManagementSettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22433-129">If successful, this method returns a `200 OK` response code and the requested [entitlementManagementSettings](../resources/entitlementManagementSettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22433-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="22433-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="22433-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22433-131">Request</span></span>

<span data-ttu-id="22433-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="22433-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="22433-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="22433-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_entitlementManagementSettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/settings
```
# <a name="c"></a>[<span data-ttu-id="22433-134">C#</span><span class="sxs-lookup"><span data-stu-id="22433-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-entitlementmanagementsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22433-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22433-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-entitlementmanagementsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22433-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22433-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-entitlementmanagementsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22433-137">Java</span><span class="sxs-lookup"><span data-stu-id="22433-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-entitlementmanagementsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="22433-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="22433-138">Response</span></span>

<span data-ttu-id="22433-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="22433-139">The following is an example of the response.</span></span>

> <span data-ttu-id="22433-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="22433-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


