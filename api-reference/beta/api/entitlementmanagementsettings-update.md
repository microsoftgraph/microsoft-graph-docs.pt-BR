---
title: Atualizar entitlementManagementSettings
description: Atualize um objeto entitlementManagementSettings para alterar uma ou mais de suas propriedades.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 87d9440424b5fe857e24fe9a9eefea109b424dd3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981040"
---
# <a name="update-entitlementmanagementsettings"></a><span data-ttu-id="1902d-103">Atualizar entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="1902d-103">Update entitlementManagementSettings</span></span>

<span data-ttu-id="1902d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1902d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1902d-105">Atualize um objeto [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) existente para alterar uma ou mais de suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="1902d-105">Update an existing [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object to change one or more of its properties.</span></span>


## <a name="permissions"></a><span data-ttu-id="1902d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1902d-106">Permissions</span></span>
<span data-ttu-id="1902d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1902d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1902d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1902d-109">Permission type</span></span>                        | <span data-ttu-id="1902d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1902d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1902d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1902d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1902d-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1902d-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="1902d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1902d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1902d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1902d-114">Not supported.</span></span> |
|<span data-ttu-id="1902d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1902d-115">Application</span></span>                            | <span data-ttu-id="1902d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1902d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1902d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1902d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/entitlementManagement/settings
```
## <a name="request-headers"></a><span data-ttu-id="1902d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1902d-118">Request headers</span></span>
| <span data-ttu-id="1902d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1902d-119">Name</span></span>         | <span data-ttu-id="1902d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1902d-120">Description</span></span> |
|:-------------|:------------|
| <span data-ttu-id="1902d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1902d-121">Authorization</span></span> | <span data-ttu-id="1902d-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="1902d-122">Bearer \{token\}.</span></span> <span data-ttu-id="1902d-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1902d-123">Required.</span></span> |
| <span data-ttu-id="1902d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1902d-124">Content-Type</span></span>  | <span data-ttu-id="1902d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1902d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1902d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1902d-127">Request body</span></span>
<span data-ttu-id="1902d-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros de um objeto [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="1902d-128">In the request body, supply a JSON representation of the parameters of an [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1902d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1902d-129">Response</span></span>
<span data-ttu-id="1902d-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1902d-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1902d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1902d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1902d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1902d-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1902d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1902d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_entitlementManagementSettings"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/settings
Content-type: application/json

{
  "externalUserLifecycleAction": "None"
}
```
# <a name="c"></a>[<span data-ttu-id="1902d-134">C#</span><span class="sxs-lookup"><span data-stu-id="1902d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-entitlementmanagementsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1902d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1902d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-entitlementmanagementsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1902d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1902d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-entitlementmanagementsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1902d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1902d-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entitlementManagementSettings"
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Update entitlementManagementSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


