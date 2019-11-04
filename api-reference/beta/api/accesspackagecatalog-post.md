---
title: Criar accessPackageCatalog
description: Criar um novo accessPackageCatalog.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 38f0683a1160b9deaf30b4ebc782b405417ef4db
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935074"
---
# <a name="create-accesspackagecatalog"></a><span data-ttu-id="4aaa6-103">Criar accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="4aaa6-103">Create accessPackageCatalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4aaa6-104">Criar um novo objeto [accessPackageCatalog](../resources/accesspackagecatalog.md) .</span><span class="sxs-lookup"><span data-stu-id="4aaa6-104">Create a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4aaa6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4aaa6-105">Permissions</span></span>

<span data-ttu-id="4aaa6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4aaa6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4aaa6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4aaa6-108">Permission type</span></span>                        | <span data-ttu-id="4aaa6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4aaa6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4aaa6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4aaa6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4aaa6-111">EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4aaa6-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="4aaa6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4aaa6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4aaa6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4aaa6-113">Not supported.</span></span> |
| <span data-ttu-id="4aaa6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4aaa6-114">Application</span></span>                            | <span data-ttu-id="4aaa6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4aaa6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4aaa6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4aaa6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="request-headers"></a><span data-ttu-id="4aaa6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4aaa6-117">Request headers</span></span>

| <span data-ttu-id="4aaa6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4aaa6-118">Name</span></span>          | <span data-ttu-id="4aaa6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4aaa6-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4aaa6-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="4aaa6-120">Authorization</span></span> | <span data-ttu-id="4aaa6-121">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="4aaa6-121">Bearer \{token\}.</span></span> <span data-ttu-id="4aaa6-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4aaa6-122">Required.</span></span> |
| <span data-ttu-id="4aaa6-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4aaa6-123">Content-Type</span></span>  | <span data-ttu-id="4aaa6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4aaa6-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4aaa6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4aaa6-125">Request body</span></span>

<span data-ttu-id="4aaa6-126">No corpo da solicitação, forneça uma representação JSON de um objeto [accessPackageCatalog](../resources/accesspackagecatalog.md) .</span><span class="sxs-lookup"><span data-stu-id="4aaa6-126">In the request body, supply a JSON representation of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>  <span data-ttu-id="4aaa6-127">Inclua as propriedades **DisplayName**, **Description**e **isExternallyVisible** .</span><span class="sxs-lookup"><span data-stu-id="4aaa6-127">Include the **displayname**, **description**, and **isExternallyVisible** properties.</span></span>

## <a name="response"></a><span data-ttu-id="4aaa6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4aaa6-128">Response</span></span>

<span data-ttu-id="4aaa6-129">Se tiver êxito, este método retornará um código de resposta de série 200 e um novo objeto [accessPackageCatalog](../resources/accesspackagecatalog.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4aaa6-129">If successful, this method returns a 200-series response code and a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4aaa6-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4aaa6-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4aaa6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4aaa6-131">Request</span></span>

<span data-ttu-id="4aaa6-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4aaa6-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_accesspackagecatalog_from_accesspackagecatalogs"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs
Content-type: application/json

{
  "displayName": "sales",
  "description": "for employees working with sales and outside sales partners",
  "isExternallyVisible": true
}
```

### <a name="response"></a><span data-ttu-id="4aaa6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4aaa6-133">Response</span></span>

<span data-ttu-id="4aaa6-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4aaa6-134">The following is an example of the response.</span></span>

> <span data-ttu-id="4aaa6-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4aaa6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageCatalog"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
  "displayName": "sales",
  "description": "for employees working with sales and outside sales partners",
  "catalogType": "UserManaged",
  "catalogStatus": "Published",
  "isExternallyVisible": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
