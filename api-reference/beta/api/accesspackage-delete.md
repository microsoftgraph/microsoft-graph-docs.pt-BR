---
title: Excluir accessPackage
description: Exclua accessPackage.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 05d4261f6a2fb6d786dfcb56214f11adec3ab7c0
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935069"
---
# <a name="delete-accesspackage"></a><span data-ttu-id="71771-103">Excluir accessPackage</span><span class="sxs-lookup"><span data-stu-id="71771-103">Delete accessPackage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71771-104">Excluir um objeto [accessPackage](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="71771-104">Delete an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="71771-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="71771-105">Permissions</span></span>

<span data-ttu-id="71771-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71771-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71771-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71771-108">Permission type</span></span>                        | <span data-ttu-id="71771-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71771-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="71771-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71771-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="71771-111">EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="71771-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="71771-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71771-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71771-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71771-113">Not supported.</span></span> |
| <span data-ttu-id="71771-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71771-114">Application</span></span>                            | <span data-ttu-id="71771-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71771-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71771-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71771-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}

```

## <a name="request-headers"></a><span data-ttu-id="71771-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71771-117">Request headers</span></span>

| <span data-ttu-id="71771-118">Nome</span><span class="sxs-lookup"><span data-stu-id="71771-118">Name</span></span>          | <span data-ttu-id="71771-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="71771-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="71771-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="71771-120">Authorization</span></span> | <span data-ttu-id="71771-121">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="71771-121">Bearer \{token\}.</span></span> <span data-ttu-id="71771-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71771-122">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71771-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71771-123">Request body</span></span>

<span data-ttu-id="71771-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71771-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71771-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="71771-125">Response</span></span>

<span data-ttu-id="71771-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71771-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="71771-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="71771-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="71771-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71771-129">Request</span></span>

<span data-ttu-id="71771-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="71771-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accesspackage"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}
```

### <a name="response"></a><span data-ttu-id="71771-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="71771-131">Response</span></span>

<span data-ttu-id="71771-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="71771-132">The following is an example of the response.</span></span>

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
  "description": "Delete accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
