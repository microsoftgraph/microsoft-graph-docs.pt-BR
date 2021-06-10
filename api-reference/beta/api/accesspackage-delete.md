---
title: Excluir accessPackage
description: Excluir accessPackage.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 710bbd3e015af5109b95905d6db68061de1506f5
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52868865"
---
# <a name="delete-accesspackage"></a><span data-ttu-id="77153-103">Excluir accessPackage</span><span class="sxs-lookup"><span data-stu-id="77153-103">Delete accessPackage</span></span>

<span data-ttu-id="77153-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77153-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77153-105">[Exclua um objeto accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="77153-105">Delete an [accessPackage](../resources/accesspackage.md) object.</span></span>

<span data-ttu-id="77153-106">Não é possível excluir um pacote de acesso se ele tiver **qualquer accessPackageAssignment**.</span><span class="sxs-lookup"><span data-stu-id="77153-106">You cannot delete an access package if it has any **accessPackageAssignment**.</span></span> <span data-ttu-id="77153-107">Para excluir o pacote de acesso, [primeiro consulte](accesspackageassignment-list.md) se há alguma atribuição com um filtro para indicar o pacote de acesso específico, como: `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'` .</span><span class="sxs-lookup"><span data-stu-id="77153-107">To delete the access package, first [query if there are any assignments](accesspackageassignment-list.md) with a filter to indicate the specific access package, such as: `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'`.</span></span> <span data-ttu-id="77153-108">Para obter mais informações sobre como remover atribuições que ainda estão no estado entregue, consulte [Remover uma atribuição](accesspackageassignmentrequest-post.md#example-4-remove-an-assignment).</span><span class="sxs-lookup"><span data-stu-id="77153-108">For more information on how to remove assignments that are still in the delivered state, see [Remove an assignment](accesspackageassignmentrequest-post.md#example-4-remove-an-assignment).</span></span>


## <a name="permissions"></a><span data-ttu-id="77153-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="77153-109">Permissions</span></span>

<span data-ttu-id="77153-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77153-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="77153-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77153-112">Permission type</span></span>                        | <span data-ttu-id="77153-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77153-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="77153-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77153-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="77153-115">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77153-115">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="77153-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77153-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77153-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77153-117">Not supported.</span></span> |
| <span data-ttu-id="77153-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77153-118">Application</span></span>                            | <span data-ttu-id="77153-119">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77153-119">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77153-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77153-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="77153-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77153-121">Request headers</span></span>

| <span data-ttu-id="77153-122">Nome</span><span class="sxs-lookup"><span data-stu-id="77153-122">Name</span></span>          | <span data-ttu-id="77153-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="77153-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="77153-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="77153-124">Authorization</span></span> | <span data-ttu-id="77153-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77153-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77153-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77153-127">Request body</span></span>

<span data-ttu-id="77153-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="77153-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77153-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="77153-129">Response</span></span>

<span data-ttu-id="77153-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77153-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="77153-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="77153-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="77153-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77153-133">Request</span></span>

<span data-ttu-id="77153-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="77153-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="77153-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="77153-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackage"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}
```
# <a name="c"></a>[<span data-ttu-id="77153-136">C#</span><span class="sxs-lookup"><span data-stu-id="77153-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77153-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77153-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77153-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77153-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77153-139">Java</span><span class="sxs-lookup"><span data-stu-id="77153-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="77153-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="77153-140">Response</span></span>

<span data-ttu-id="77153-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="77153-141">The following is an example of the response.</span></span>

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


