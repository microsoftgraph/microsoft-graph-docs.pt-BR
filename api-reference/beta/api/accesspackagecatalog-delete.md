---
title: Excluir accessPackageCatalog
description: Exclua accessPackageCatalog.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f6ab9df54690c93453e3fd030c37978d42db7da9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935082"
---
# <a name="delete-accesspackagecatalog"></a><span data-ttu-id="06031-103">Excluir accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="06031-103">Delete accessPackageCatalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06031-104">Excluir um [accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="06031-104">Delete an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="06031-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="06031-105">Permissions</span></span>

<span data-ttu-id="06031-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06031-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06031-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06031-108">Permission type</span></span>                        | <span data-ttu-id="06031-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06031-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="06031-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06031-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="06031-111">EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="06031-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="06031-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06031-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06031-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06031-113">Not supported.</span></span> |
| <span data-ttu-id="06031-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06031-114">Application</span></span>                            | <span data-ttu-id="06031-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06031-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="06031-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06031-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="06031-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06031-117">Request headers</span></span>

| <span data-ttu-id="06031-118">Nome</span><span class="sxs-lookup"><span data-stu-id="06031-118">Name</span></span>          | <span data-ttu-id="06031-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="06031-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="06031-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="06031-120">Authorization</span></span> | <span data-ttu-id="06031-121">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="06031-121">Bearer \{token\}.</span></span> <span data-ttu-id="06031-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06031-122">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06031-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06031-123">Request body</span></span>

<span data-ttu-id="06031-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="06031-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06031-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="06031-125">Response</span></span>

<span data-ttu-id="06031-126">Se tiver êxito, este método retornará um código de resposta da série 200.</span><span class="sxs-lookup"><span data-stu-id="06031-126">If successful, this method returns a 200-series response code.</span></span> <span data-ttu-id="06031-127">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06031-127">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="06031-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="06031-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="06031-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06031-129">Request</span></span>

<span data-ttu-id="06031-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="06031-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accesspackagecatalog"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

### <a name="response"></a><span data-ttu-id="06031-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="06031-131">Response</span></span>

<span data-ttu-id="06031-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="06031-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
