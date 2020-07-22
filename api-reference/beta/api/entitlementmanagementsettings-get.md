---
title: Obter entitlementManagementSettings
description: Recupere as propriedades do objeto entitlementManagementSettings.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c731de0929aa7d5dfe0197526468a7b87a6a31b0
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2020
ms.locfileid: "45225057"
---
# <a name="get-entitlementmanagementsettings"></a><span data-ttu-id="05a7b-103">Obter entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="05a7b-103">Get entitlementManagementSettings</span></span>

<span data-ttu-id="05a7b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05a7b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05a7b-105">Recupere as propriedades de um objeto [entitlementManagementSettings](../resources/entitlementManagementSettings.md) .</span><span class="sxs-lookup"><span data-stu-id="05a7b-105">Retrieve the properties of an [entitlementManagementSettings](../resources/entitlementManagementSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="05a7b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="05a7b-106">Permissions</span></span>

<span data-ttu-id="05a7b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05a7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05a7b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05a7b-109">Permission type</span></span>                        | <span data-ttu-id="05a7b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05a7b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="05a7b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05a7b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="05a7b-112">EntitlementManagement. Read. All, EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="05a7b-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="05a7b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05a7b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05a7b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05a7b-114">Not supported.</span></span> |
| <span data-ttu-id="05a7b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05a7b-115">Application</span></span>                            | <span data-ttu-id="05a7b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05a7b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="05a7b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05a7b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="05a7b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="05a7b-118">Optional query parameters</span></span>

<span data-ttu-id="05a7b-119">Este método não oferece suporte aos parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="05a7b-119">This method does not support the OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="05a7b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05a7b-120">Request headers</span></span>

| <span data-ttu-id="05a7b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="05a7b-121">Name</span></span>      |<span data-ttu-id="05a7b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="05a7b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="05a7b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="05a7b-123">Authorization</span></span> | <span data-ttu-id="05a7b-124">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="05a7b-124">Bearer \{token\}.</span></span> <span data-ttu-id="05a7b-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05a7b-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="05a7b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05a7b-126">Request body</span></span>

<span data-ttu-id="05a7b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="05a7b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05a7b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="05a7b-128">Response</span></span>

<span data-ttu-id="05a7b-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [entitlementManagementSettings](../resources/entitlementManagementSettings.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05a7b-129">If successful, this method returns a `200 OK` response code and the requested [entitlementManagementSettings](../resources/entitlementManagementSettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="05a7b-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="05a7b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="05a7b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05a7b-131">Request</span></span>

<span data-ttu-id="05a7b-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="05a7b-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_entitlementManagementSettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/settings
```


### <a name="response"></a><span data-ttu-id="05a7b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="05a7b-133">Response</span></span>

<span data-ttu-id="05a7b-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="05a7b-134">The following is an example of the response.</span></span>

> <span data-ttu-id="05a7b-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05a7b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
