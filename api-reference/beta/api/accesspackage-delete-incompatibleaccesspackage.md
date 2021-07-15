---
title: Remover accessPackage de incompatívelAccessPackages
description: Remova um link que indica que um pacote de acesso é incompatível com um pacote de acesso especificado.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c228402a433c3d9920481030ead07e79333459bc
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439357"
---
# <a name="remove-accesspackage-from-incompatibleaccesspackages"></a><span data-ttu-id="fc8aa-103">Remover accessPackage de incompatívelAccessPackages</span><span class="sxs-lookup"><span data-stu-id="fc8aa-103">Remove accessPackage from incompatibleAccessPackages</span></span>

<span data-ttu-id="fc8aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc8aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc8aa-105">Remover um [pacote de](../resources/accesspackage.md) acesso da lista de pacotes de acesso que foram marcados como incompatíveis em [um accessPackage](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="fc8aa-105">Remove an [access package](../resources/accesspackage.md) from the list of access packages that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="fc8aa-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="fc8aa-106">Permissions</span></span>

<span data-ttu-id="fc8aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc8aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fc8aa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc8aa-109">Permission type</span></span>                        | <span data-ttu-id="fc8aa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc8aa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fc8aa-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc8aa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc8aa-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc8aa-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="fc8aa-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc8aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc8aa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc8aa-114">Not supported.</span></span> |
| <span data-ttu-id="fc8aa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc8aa-115">Application</span></span>                            | <span data-ttu-id="fc8aa-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc8aa-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc8aa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc8aa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="fc8aa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc8aa-118">Request headers</span></span>

| <span data-ttu-id="fc8aa-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fc8aa-119">Name</span></span>          | <span data-ttu-id="fc8aa-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc8aa-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fc8aa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc8aa-121">Authorization</span></span> | <span data-ttu-id="fc8aa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc8aa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc8aa-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fc8aa-124">Content-Type</span></span>  | <span data-ttu-id="fc8aa-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc8aa-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fc8aa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc8aa-127">Request body</span></span>

<span data-ttu-id="fc8aa-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc8aa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc8aa-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc8aa-129">Response</span></span>

<span data-ttu-id="fc8aa-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc8aa-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fc8aa-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fc8aa-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fc8aa-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc8aa-133">Request</span></span>

<span data-ttu-id="fc8aa-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc8aa-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fc8aa-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc8aa-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_incompatibleaccesspackage_from_accesspackage"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="fc8aa-136">C#</span><span class="sxs-lookup"><span data-stu-id="fc8aa-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-incompatibleaccesspackage-from-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc8aa-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc8aa-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-incompatibleaccesspackage-from-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc8aa-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc8aa-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-incompatibleaccesspackage-from-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc8aa-139">Java</span><span class="sxs-lookup"><span data-stu-id="fc8aa-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-incompatibleaccesspackage-from-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="fc8aa-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc8aa-140">Response</span></span>

<span data-ttu-id="fc8aa-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fc8aa-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove incompatibleAccessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

