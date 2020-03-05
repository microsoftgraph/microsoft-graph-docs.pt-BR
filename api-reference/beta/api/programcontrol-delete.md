---
title: Excluir programControl
description: No recurso de revisões do Azure AD Access, exclua um objeto programControl.  Isso desvincula uma revisão do Access de um programa.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 793e4697d7d692f9cf982a9114d8dd54b0280f07
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454959"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="53eed-104">Excluir programControl</span><span class="sxs-lookup"><span data-stu-id="53eed-104">Delete programControl</span></span>

<span data-ttu-id="53eed-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="53eed-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53eed-106">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , exclua um objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="53eed-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="53eed-107">Isso desvincula uma revisão do Access de um programa.</span><span class="sxs-lookup"><span data-stu-id="53eed-107">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="53eed-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="53eed-108">Permissions</span></span>
<span data-ttu-id="53eed-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53eed-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53eed-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53eed-111">Permission type</span></span>                        | <span data-ttu-id="53eed-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="53eed-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="53eed-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53eed-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="53eed-114">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53eed-114">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="53eed-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53eed-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53eed-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53eed-116">Not supported.</span></span> |
|<span data-ttu-id="53eed-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53eed-117">Application</span></span>                            | <span data-ttu-id="53eed-118">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53eed-118">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="53eed-119">O usuário conectado também deve estar em uma função de diretório que permite excluir um `programControl`.</span><span class="sxs-lookup"><span data-stu-id="53eed-119">The signed in user must also be in a directory role that permits them to delete a `programControl`.</span></span>

## <a name="http-request"></a><span data-ttu-id="53eed-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53eed-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls/{id}
```
## <a name="request-headers"></a><span data-ttu-id="53eed-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53eed-121">Request headers</span></span>
| <span data-ttu-id="53eed-122">Nome</span><span class="sxs-lookup"><span data-stu-id="53eed-122">Name</span></span>         | <span data-ttu-id="53eed-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="53eed-123">Type</span></span>        | <span data-ttu-id="53eed-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="53eed-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="53eed-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="53eed-125">Authorization</span></span> | <span data-ttu-id="53eed-126">string</span><span class="sxs-lookup"><span data-stu-id="53eed-126">string</span></span> | <span data-ttu-id="53eed-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53eed-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53eed-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53eed-129">Request body</span></span>
<span data-ttu-id="53eed-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="53eed-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="53eed-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="53eed-131">Response</span></span>
<span data-ttu-id="53eed-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53eed-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53eed-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53eed-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53eed-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53eed-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="53eed-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="53eed-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
# <a name="c"></a>[<span data-ttu-id="53eed-137">C#</span><span class="sxs-lookup"><span data-stu-id="53eed-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-programcontrol-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53eed-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53eed-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-programcontrol-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53eed-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53eed-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-programcontrol-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="53eed-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="53eed-140">Response</span></span>
><span data-ttu-id="53eed-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53eed-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
