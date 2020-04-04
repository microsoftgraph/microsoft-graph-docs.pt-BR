---
title: Remover proprietário
description: Remover um proprietário de um aplicativo.
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e0a0bdda6325afa6d21769117a04430f1455e7eb
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144209"
---
# <a name="remove-owner"></a><span data-ttu-id="df7de-103">Remover proprietário</span><span class="sxs-lookup"><span data-stu-id="df7de-103">Remove owner</span></span>

<span data-ttu-id="df7de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df7de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df7de-105">Remover um proprietário de um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="df7de-105">Remove an owner from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="df7de-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="df7de-106">Permissions</span></span>
<span data-ttu-id="df7de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df7de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df7de-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df7de-109">Permission type</span></span>      | <span data-ttu-id="df7de-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df7de-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df7de-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df7de-111">Delegated (work or school account)</span></span> | <span data-ttu-id="df7de-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="df7de-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="df7de-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df7de-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df7de-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df7de-114">Not supported.</span></span>    |
|<span data-ttu-id="df7de-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df7de-115">Application</span></span> | <span data-ttu-id="df7de-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df7de-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df7de-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df7de-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}/owners/{id}/$ref

```
## <a name="request-headers"></a><span data-ttu-id="df7de-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df7de-118">Request headers</span></span>
| <span data-ttu-id="df7de-119">Nome</span><span class="sxs-lookup"><span data-stu-id="df7de-119">Name</span></span> | <span data-ttu-id="df7de-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="df7de-120">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="df7de-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="df7de-121">Authorization</span></span> | <span data-ttu-id="df7de-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df7de-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="df7de-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df7de-124">Request body</span></span>
<span data-ttu-id="df7de-125">No corpo da solicitação, forneça o identificador do objeto de diretório a ser atribuído como proprietário.</span><span class="sxs-lookup"><span data-stu-id="df7de-125">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="df7de-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="df7de-126">Response</span></span>

<span data-ttu-id="df7de-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="df7de-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="df7de-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df7de-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="df7de-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df7de-129">Request</span></span>

<span data-ttu-id="df7de-130">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="df7de-130">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="df7de-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="df7de-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_delete_owners"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/owners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="df7de-132">C#</span><span class="sxs-lookup"><span data-stu-id="df7de-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-delete-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df7de-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df7de-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-delete-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df7de-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df7de-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-delete-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df7de-135">Java</span><span class="sxs-lookup"><span data-stu-id="df7de-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-delete-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="df7de-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="df7de-136">Response</span></span>

<span data-ttu-id="df7de-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="df7de-137">The following is an example of the response.</span></span>

><span data-ttu-id="df7de-138">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="df7de-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="df7de-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df7de-139">All the properties will be returned from an actual call.</span></span>

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
