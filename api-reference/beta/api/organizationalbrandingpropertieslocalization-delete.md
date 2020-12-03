---
title: Excluir organizationalBrandingProperties localizado
description: Excluir organizationalBrandingProperties para uma localização específica.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8136325ce1e81728951165475d49944f048dd1a5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49524621"
---
# <a name="delete-localized-organizationalbrandingproperties"></a><span data-ttu-id="bd9ab-103">Excluir organizationalBrandingProperties localizado</span><span class="sxs-lookup"><span data-stu-id="bd9ab-103">Delete Localized organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd9ab-104">Excluir um objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="bd9ab-104">Delete an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd9ab-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="bd9ab-105">Permissions</span></span>

<span data-ttu-id="bd9ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd9ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd9ab-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd9ab-108">Permission type</span></span>                        | <span data-ttu-id="bd9ab-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd9ab-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bd9ab-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd9ab-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd9ab-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd9ab-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="bd9ab-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd9ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd9ab-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd9ab-113">Not supported.</span></span> |
| <span data-ttu-id="bd9ab-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd9ab-114">Application</span></span>                            | <span data-ttu-id="bd9ab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd9ab-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd9ab-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd9ab-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/branding/localizations/{locale}
```

## <a name="request-headers"></a><span data-ttu-id="bd9ab-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd9ab-117">Request headers</span></span>

| <span data-ttu-id="bd9ab-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bd9ab-118">Name</span></span>          | <span data-ttu-id="bd9ab-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd9ab-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bd9ab-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd9ab-120">Authorization</span></span> | <span data-ttu-id="bd9ab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd9ab-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd9ab-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd9ab-123">Request body</span></span>

<span data-ttu-id="bd9ab-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd9ab-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd9ab-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd9ab-125">Response</span></span>

<span data-ttu-id="bd9ab-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd9ab-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd9ab-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bd9ab-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd9ab-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd9ab-129">Request</span></span>

<span data-ttu-id="bd9ab-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd9ab-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bd9ab-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd9ab-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_organizationalbrandingproperties"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```
# <a name="c"></a>[<span data-ttu-id="bd9ab-132">C#</span><span class="sxs-lookup"><span data-stu-id="bd9ab-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd9ab-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd9ab-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd9ab-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd9ab-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd9ab-135">Java</span><span class="sxs-lookup"><span data-stu-id="bd9ab-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bd9ab-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd9ab-136">Response</span></span>

<span data-ttu-id="bd9ab-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bd9ab-137">The following is an example of the response.</span></span>

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
