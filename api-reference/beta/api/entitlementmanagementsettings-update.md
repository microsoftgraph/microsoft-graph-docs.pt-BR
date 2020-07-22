---
title: Atualizar entitlementManagementSettings
description: Atualize um objeto entitlementManagementSettings para alterar uma ou mais de suas propriedades.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 23d37c089e9c81939ba9342a7f5747dd979b8bec
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2020
ms.locfileid: "45225058"
---
# <a name="update-entitlementmanagementsettings"></a><span data-ttu-id="984fe-103">Atualizar entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="984fe-103">Update entitlementManagementSettings</span></span>

<span data-ttu-id="984fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="984fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="984fe-105">Atualize um objeto [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) existente para alterar uma ou mais de suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="984fe-105">Update an existing [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object to change one or more of its properties.</span></span>


## <a name="permissions"></a><span data-ttu-id="984fe-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="984fe-106">Permissions</span></span>
<span data-ttu-id="984fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="984fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="984fe-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="984fe-109">Permission type</span></span>                        | <span data-ttu-id="984fe-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="984fe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="984fe-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="984fe-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="984fe-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="984fe-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="984fe-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="984fe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="984fe-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="984fe-114">Not supported.</span></span> |
|<span data-ttu-id="984fe-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="984fe-115">Application</span></span>                            | <span data-ttu-id="984fe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="984fe-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="984fe-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="984fe-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/entitlementManagement/settings
```
## <a name="request-headers"></a><span data-ttu-id="984fe-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="984fe-118">Request headers</span></span>
| <span data-ttu-id="984fe-119">Nome</span><span class="sxs-lookup"><span data-stu-id="984fe-119">Name</span></span>         | <span data-ttu-id="984fe-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="984fe-120">Description</span></span> |
|:-------------|:------------|
| <span data-ttu-id="984fe-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="984fe-121">Authorization</span></span> | <span data-ttu-id="984fe-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="984fe-122">Bearer \{token\}.</span></span> <span data-ttu-id="984fe-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="984fe-123">Required.</span></span> |
| <span data-ttu-id="984fe-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="984fe-124">Content-Type</span></span>  | <span data-ttu-id="984fe-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="984fe-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="984fe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="984fe-127">Request body</span></span>
<span data-ttu-id="984fe-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros de um objeto [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="984fe-128">In the request body, supply a JSON representation of the parameters of an [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="984fe-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="984fe-129">Response</span></span>
<span data-ttu-id="984fe-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="984fe-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="984fe-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="984fe-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="984fe-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="984fe-132">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="984fe-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="984fe-133">Response</span></span>

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
