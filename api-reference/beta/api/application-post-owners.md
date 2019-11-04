---
title: Adicionar proprietário
description: Use esta API para adicionar um proprietário a um aplicativo.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f6defdd415ac2286c1a81d5d03fc7664233fd4de
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37934306"
---
# <a name="add-owner"></a><span data-ttu-id="e91f2-103">Adicionar proprietário</span><span class="sxs-lookup"><span data-stu-id="e91f2-103">Add owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e91f2-104">Use esta API para adicionar um proprietário a um aplicativo postando na coleção de proprietários.</span><span class="sxs-lookup"><span data-stu-id="e91f2-104">Use this API to add an owner to an application by posting to the owners collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="e91f2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e91f2-105">Permissions</span></span>
<span data-ttu-id="e91f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e91f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e91f2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e91f2-108">Permission type</span></span>      | <span data-ttu-id="e91f2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e91f2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e91f2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e91f2-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e91f2-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e91f2-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e91f2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e91f2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e91f2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e91f2-113">Not supported.</span></span>    |
|<span data-ttu-id="e91f2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e91f2-114">Application</span></span> | <span data-ttu-id="e91f2-115">Application. ReadWrite. OwnedBy e Directory. Read. All, Application. ReadWrite. All e Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="e91f2-115">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e91f2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e91f2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="e91f2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e91f2-117">Request headers</span></span>
| <span data-ttu-id="e91f2-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e91f2-118">Name</span></span> | <span data-ttu-id="e91f2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e91f2-119">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="e91f2-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e91f2-120">Authorization</span></span> | <span data-ttu-id="e91f2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e91f2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e91f2-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e91f2-123">Request body</span></span>
<span data-ttu-id="e91f2-124">No corpo da solicitação, forneça o identificador do objeto de diretório a ser atribuído como proprietário.</span><span class="sxs-lookup"><span data-stu-id="e91f2-124">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="e91f2-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e91f2-125">Response</span></span>

<span data-ttu-id="e91f2-126">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e91f2-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e91f2-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e91f2-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="e91f2-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e91f2-128">Request</span></span>
<span data-ttu-id="e91f2-129">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="e91f2-129">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e91f2-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="e91f2-130">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e91f2-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e91f2-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="e91f2-132">C#</span><span class="sxs-lookup"><span data-stu-id="e91f2-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e91f2-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e91f2-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e91f2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e91f2-134">Response</span></span>

<span data-ttu-id="e91f2-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e91f2-135">The following is an example of the response.</span></span>

><span data-ttu-id="e91f2-136">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e91f2-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e91f2-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e91f2-137">All the properties will be returned from an actual call.</span></span>

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
