---
title: Excluir organizationalBrandingProperties
description: Excluir organizationalBrandingProperties.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 14531b138a811ef0c5f69cf8121d97cc521ca615
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949414"
---
# <a name="delete-organizationalbrandingproperties"></a><span data-ttu-id="f8d6c-103">Excluir organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="f8d6c-103">Delete organizationalBrandingProperties</span></span>

<span data-ttu-id="f8d6c-104">[Exclua um objeto organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="f8d6c-104">Delete an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8d6c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f8d6c-105">Permissions</span></span>

<span data-ttu-id="f8d6c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8d6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8d6c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8d6c-108">Permission type</span></span>                        | <span data-ttu-id="f8d6c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8d6c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f8d6c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8d6c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8d6c-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8d6c-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="f8d6c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8d6c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8d6c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8d6c-113">Not supported.</span></span> |
| <span data-ttu-id="f8d6c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8d6c-114">Application</span></span>                            | <span data-ttu-id="f8d6c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8d6c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8d6c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8d6c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/branding
```

## <a name="request-headers"></a><span data-ttu-id="f8d6c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8d6c-117">Request headers</span></span>

| <span data-ttu-id="f8d6c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f8d6c-118">Name</span></span>          | <span data-ttu-id="f8d6c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8d6c-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f8d6c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8d6c-120">Authorization</span></span> | <span data-ttu-id="f8d6c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8d6c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8d6c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8d6c-123">Request body</span></span>

<span data-ttu-id="f8d6c-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8d6c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8d6c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8d6c-125">Response</span></span>

<span data-ttu-id="f8d6c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8d6c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f8d6c-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f8d6c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f8d6c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8d6c-129">Request</span></span>

<span data-ttu-id="f8d6c-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8d6c-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f8d6c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8d6c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_organizationalbrandingproperties_1"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```
# <a name="c"></a>[<span data-ttu-id="f8d6c-132">C#</span><span class="sxs-lookup"><span data-stu-id="f8d6c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-organizationalbrandingproperties-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8d6c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8d6c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-organizationalbrandingproperties-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8d6c-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8d6c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-organizationalbrandingproperties-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f8d6c-135">Java</span><span class="sxs-lookup"><span data-stu-id="f8d6c-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-organizationalbrandingproperties-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f8d6c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8d6c-136">Response</span></span>

<span data-ttu-id="f8d6c-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f8d6c-137">The following is an example of the response.</span></span>

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
  "description": "Delete organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
