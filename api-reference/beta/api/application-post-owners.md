---
title: Criar proprietário
description: Use esta API para criar um novo proprietário.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2dbfaf498b8b0726da1de3ee35fafd547747e990
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408276"
---
# <a name="create-owner"></a><span data-ttu-id="13c27-103">Criar proprietário</span><span class="sxs-lookup"><span data-stu-id="13c27-103">Create owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13c27-104">Use esta API para criar um novo proprietário.</span><span class="sxs-lookup"><span data-stu-id="13c27-104">Use this API to create a new owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="13c27-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="13c27-105">Permissions</span></span>
<span data-ttu-id="13c27-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13c27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13c27-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13c27-108">Permission type</span></span>      | <span data-ttu-id="13c27-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13c27-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13c27-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13c27-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="13c27-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="13c27-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="13c27-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13c27-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13c27-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13c27-113">Not supported.</span></span>    |
|<span data-ttu-id="13c27-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13c27-114">Application</span></span> | <span data-ttu-id="13c27-115">Application. ReadWrite. OwnedBy e Directory. Read. All, Application. ReadWrite. All e Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="13c27-115">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13c27-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13c27-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="13c27-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13c27-117">Request headers</span></span>
| <span data-ttu-id="13c27-118">Nome</span><span class="sxs-lookup"><span data-stu-id="13c27-118">Name</span></span> | <span data-ttu-id="13c27-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="13c27-119">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="13c27-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="13c27-120">Authorization</span></span> | <span data-ttu-id="13c27-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13c27-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="13c27-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13c27-123">Request body</span></span>
<span data-ttu-id="13c27-124">No corpo da solicitação, forneça o identificador do objeto de diretório a ser atribuído como proprietário.</span><span class="sxs-lookup"><span data-stu-id="13c27-124">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="13c27-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="13c27-125">Response</span></span>

<span data-ttu-id="13c27-126">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="13c27-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="13c27-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13c27-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="13c27-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13c27-128">Request</span></span>
<span data-ttu-id="13c27-129">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="13c27-129">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="13c27-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="13c27-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_application"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
"@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}

```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="13c27-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13c27-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="13c27-132">C#</span><span class="sxs-lookup"><span data-stu-id="13c27-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="13c27-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="13c27-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="13c27-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="13c27-134">Response</span></span>

<span data-ttu-id="13c27-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="13c27-135">The following is an example of the response.</span></span>

><span data-ttu-id="13c27-136">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="13c27-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="13c27-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13c27-137">All the properties will be returned from an actual call.</span></span>

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
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
