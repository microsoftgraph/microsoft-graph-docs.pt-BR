---
title: Adicionar proprietário
description: Use esta API para adicionar um proprietário a um aplicativo.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cc47d329e84cdd7cdea2356c81c3271f986e3d86
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441456"
---
# <a name="add-owner"></a><span data-ttu-id="ed9e3-103">Adicionar proprietário</span><span class="sxs-lookup"><span data-stu-id="ed9e3-103">Add owner</span></span>

<span data-ttu-id="ed9e3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ed9e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed9e3-105">Use esta API para adicionar um proprietário a um aplicativo postando na coleção de proprietários.</span><span class="sxs-lookup"><span data-stu-id="ed9e3-105">Use this API to add an owner to an application by posting to the owners collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed9e3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed9e3-106">Permissions</span></span>
<span data-ttu-id="ed9e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed9e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed9e3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed9e3-109">Permission type</span></span>      | <span data-ttu-id="ed9e3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed9e3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed9e3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed9e3-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="ed9e3-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ed9e3-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ed9e3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed9e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed9e3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed9e3-114">Not supported.</span></span>    |
|<span data-ttu-id="ed9e3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed9e3-115">Application</span></span> | <span data-ttu-id="ed9e3-116">Application. ReadWrite. OwnedBy e Directory. Read. All, Application. ReadWrite. All e Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="ed9e3-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed9e3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed9e3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="ed9e3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed9e3-118">Request headers</span></span>
| <span data-ttu-id="ed9e3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ed9e3-119">Name</span></span> | <span data-ttu-id="ed9e3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed9e3-120">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="ed9e3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed9e3-121">Authorization</span></span> | <span data-ttu-id="ed9e3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed9e3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ed9e3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed9e3-124">Request body</span></span>
<span data-ttu-id="ed9e3-125">No corpo da solicitação, forneça o identificador do objeto de diretório a ser atribuído como proprietário.</span><span class="sxs-lookup"><span data-stu-id="ed9e3-125">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="ed9e3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed9e3-126">Response</span></span>

<span data-ttu-id="ed9e3-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ed9e3-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ed9e3-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed9e3-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed9e3-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed9e3-129">Request</span></span>
<span data-ttu-id="ed9e3-130">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed9e3-130">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ed9e3-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed9e3-131">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="ed9e3-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed9e3-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="ed9e3-133">C#</span><span class="sxs-lookup"><span data-stu-id="ed9e3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed9e3-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed9e3-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ed9e3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed9e3-135">Response</span></span>

<span data-ttu-id="ed9e3-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ed9e3-136">The following is an example of the response.</span></span>

><span data-ttu-id="ed9e3-137">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ed9e3-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ed9e3-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed9e3-138">All the properties will be returned from an actual call.</span></span>

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
