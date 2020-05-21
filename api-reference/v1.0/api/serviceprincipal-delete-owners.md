---
title: Remover proprietário
description: Remover um proprietário de um servicePrincipalName.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3999d5d193e4084b57f59fc2c5ca4fa647fa29a4
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334162"
---
# <a name="remove-owner"></a><span data-ttu-id="9158c-103">Remover proprietário</span><span class="sxs-lookup"><span data-stu-id="9158c-103">Remove owner</span></span>

<span data-ttu-id="9158c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9158c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9158c-105">Remover um proprietário de um objeto [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="9158c-105">Remove an owner from a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9158c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9158c-106">Permissions</span></span>
<span data-ttu-id="9158c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9158c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9158c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9158c-109">Permission type</span></span>      | <span data-ttu-id="9158c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9158c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9158c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9158c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9158c-112">Application. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="9158c-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9158c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9158c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9158c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9158c-114">Not supported.</span></span>    |
|<span data-ttu-id="9158c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9158c-115">Application</span></span> | <span data-ttu-id="9158c-116">Application. ReadWrite. All, Application. ReadWrite. OwnedBy</span><span class="sxs-lookup"><span data-stu-id="9158c-116">Application.ReadWrite.All, Application.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="9158c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9158c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /serviceprincipals/{id}/owners/{id}/$ref

```
## <a name="request-headers"></a><span data-ttu-id="9158c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9158c-118">Request headers</span></span>
| <span data-ttu-id="9158c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9158c-119">Name</span></span> | <span data-ttu-id="9158c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9158c-120">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="9158c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9158c-121">Authorization</span></span> | <span data-ttu-id="9158c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9158c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9158c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9158c-124">Request body</span></span>
<span data-ttu-id="9158c-125">No corpo da solicitação, forneça o identificador do objeto de diretório a ser atribuído como proprietário.</span><span class="sxs-lookup"><span data-stu-id="9158c-125">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="9158c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9158c-126">Response</span></span>

<span data-ttu-id="9158c-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9158c-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9158c-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9158c-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="9158c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9158c-129">Request</span></span>

<span data-ttu-id="9158c-130">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="9158c-130">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9158c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="9158c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_owners"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/serviceprincipals/{id}/owners/{id}/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}

```
# <a name="c"></a>[<span data-ttu-id="9158c-132">C#</span><span class="sxs-lookup"><span data-stu-id="9158c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9158c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9158c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9158c-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9158c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9158c-135">Java</span><span class="sxs-lookup"><span data-stu-id="9158c-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delete-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9158c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9158c-136">Response</span></span>

<span data-ttu-id="9158c-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9158c-137">The following is an example of the response.</span></span>

><span data-ttu-id="9158c-138">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9158c-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9158c-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9158c-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
