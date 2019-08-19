---
title: Excluir unifiedRoleDefinition
description: Excluir um objeto unifiedRoleDefinition.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e64dfdc90152675b18bda72cc17effc57e1df681
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461585"
---
# <a name="delete-unifiedroledefinition"></a><span data-ttu-id="c962f-103">Excluir unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c962f-103">Delete unifiedRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c962f-104">Excluir um objeto [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="c962f-104">Delete a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c962f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c962f-105">Permissions</span></span>

<span data-ttu-id="c962f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c962f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c962f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c962f-108">Permission type</span></span>                        | <span data-ttu-id="c962f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c962f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c962f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c962f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c962f-111">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="c962f-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="c962f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c962f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c962f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c962f-113">Not supported.</span></span> |
| <span data-ttu-id="c962f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c962f-114">Application</span></span>                            | <span data-ttu-id="c962f-115">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="c962f-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="c962f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c962f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleDefinitions/{id}

```

## <a name="request-headers"></a><span data-ttu-id="c962f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c962f-117">Request headers</span></span>

| <span data-ttu-id="c962f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c962f-118">Name</span></span>          | <span data-ttu-id="c962f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c962f-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c962f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c962f-120">Authorization</span></span> | <span data-ttu-id="c962f-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="c962f-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c962f-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c962f-122">Request body</span></span>

<span data-ttu-id="c962f-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c962f-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c962f-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="c962f-124">Response</span></span>

<span data-ttu-id="c962f-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c962f-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c962f-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c962f-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="c962f-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c962f-128">Request</span></span>

<span data-ttu-id="c962f-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c962f-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c962f-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="c962f-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c962f-131">C#</span><span class="sxs-lookup"><span data-stu-id="c962f-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c962f-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c962f-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c962f-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c962f-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c962f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c962f-134">Response</span></span>

<span data-ttu-id="c962f-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c962f-135">The following is an example of the response.</span></span>

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
  "description": "Delete unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
