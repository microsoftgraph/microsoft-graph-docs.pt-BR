---
title: Remover proprietário
description: Remover um proprietário de um aplicativo.
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 034e8299ec1a5a05f1fa307f0196aed2113aebbc
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786072"
---
# <a name="remove-owner"></a><span data-ttu-id="94a1a-103">Remover proprietário</span><span class="sxs-lookup"><span data-stu-id="94a1a-103">Remove owner</span></span>

<span data-ttu-id="94a1a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94a1a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94a1a-105">Remover um proprietário de um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="94a1a-105">Remove an owner from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="94a1a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="94a1a-106">Permissions</span></span>
<span data-ttu-id="94a1a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94a1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94a1a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94a1a-109">Permission type</span></span>      | <span data-ttu-id="94a1a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94a1a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94a1a-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94a1a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="94a1a-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="94a1a-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="94a1a-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94a1a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94a1a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94a1a-114">Not supported.</span></span>    |
|<span data-ttu-id="94a1a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94a1a-115">Application</span></span> | <span data-ttu-id="94a1a-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94a1a-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94a1a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94a1a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}/owners/{id}/$ref

```
## <a name="request-headers"></a><span data-ttu-id="94a1a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94a1a-118">Request headers</span></span>
| <span data-ttu-id="94a1a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="94a1a-119">Name</span></span> | <span data-ttu-id="94a1a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="94a1a-120">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="94a1a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="94a1a-121">Authorization</span></span> | <span data-ttu-id="94a1a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94a1a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="94a1a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94a1a-124">Request body</span></span>
<span data-ttu-id="94a1a-125">No corpo da solicitação, fornece o identificador do objeto de diretório a ser atribuído como proprietário.</span><span class="sxs-lookup"><span data-stu-id="94a1a-125">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="94a1a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="94a1a-126">Response</span></span>

<span data-ttu-id="94a1a-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="94a1a-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="94a1a-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94a1a-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="94a1a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94a1a-129">Request</span></span>

<span data-ttu-id="94a1a-130">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="94a1a-130">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="94a1a-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="94a1a-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_delete_owners"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/owners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="94a1a-132">C#</span><span class="sxs-lookup"><span data-stu-id="94a1a-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-delete-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94a1a-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94a1a-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-delete-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94a1a-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94a1a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-delete-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94a1a-135">Java</span><span class="sxs-lookup"><span data-stu-id="94a1a-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-delete-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="94a1a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="94a1a-136">Response</span></span>

<span data-ttu-id="94a1a-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="94a1a-137">The following is an example of the response.</span></span>

><span data-ttu-id="94a1a-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="94a1a-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
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

