---
title: Excluir programControl
description: No recurso de revisões de acesso do Azure AD, exclua um objeto programControl.  Isso desvincula uma revisão de acesso de um programa.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 3a3622c7e9d1390c956c926f8e04d85ecfe7b7c2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055222"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="f844e-104">Excluir programControl</span><span class="sxs-lookup"><span data-stu-id="f844e-104">Delete programControl</span></span>

<span data-ttu-id="f844e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f844e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f844e-106">No recurso de revisões de acesso do Azure [AD,](../resources/accessreviews-root.md) exclua um [objeto programControl.](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="f844e-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="f844e-107">Isso desvincula uma revisão de acesso de um programa.</span><span class="sxs-lookup"><span data-stu-id="f844e-107">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="f844e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f844e-108">Permissions</span></span>
<span data-ttu-id="f844e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f844e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f844e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f844e-111">Permission type</span></span>                        | <span data-ttu-id="f844e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f844e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f844e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f844e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f844e-114">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f844e-114">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="f844e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f844e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f844e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f844e-116">Not supported.</span></span> |
|<span data-ttu-id="f844e-117">Application</span><span class="sxs-lookup"><span data-stu-id="f844e-117">Application</span></span>                            | <span data-ttu-id="f844e-118">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f844e-118">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="f844e-119">O usuário inscreveu também deve estar em uma função de diretório que permita que ele exclua um `programControl` .</span><span class="sxs-lookup"><span data-stu-id="f844e-119">The signed in user must also be in a directory role that permits them to delete a `programControl`.</span></span>

## <a name="http-request"></a><span data-ttu-id="f844e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f844e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f844e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f844e-121">Request headers</span></span>
| <span data-ttu-id="f844e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f844e-122">Name</span></span>         | <span data-ttu-id="f844e-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f844e-123">Type</span></span>        | <span data-ttu-id="f844e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f844e-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f844e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f844e-125">Authorization</span></span> | <span data-ttu-id="f844e-126">string</span><span class="sxs-lookup"><span data-stu-id="f844e-126">string</span></span> | <span data-ttu-id="f844e-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f844e-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f844e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f844e-129">Request body</span></span>
<span data-ttu-id="f844e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f844e-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f844e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f844e-131">Response</span></span>
<span data-ttu-id="f844e-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f844e-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f844e-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f844e-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f844e-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f844e-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f844e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f844e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
# <a name="c"></a>[<span data-ttu-id="f844e-137">C#</span><span class="sxs-lookup"><span data-stu-id="f844e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-programcontrol-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f844e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f844e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-programcontrol-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f844e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f844e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-programcontrol-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f844e-140">Java</span><span class="sxs-lookup"><span data-stu-id="f844e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-programcontrol-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f844e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f844e-141">Response</span></span>
><span data-ttu-id="f844e-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f844e-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


