---
title: Excluir programControl
description: No recurso de revisões do Azure AD Access, exclua um objeto programControl.  Isso desvincula uma revisão do Access de um programa.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 009bd40b873d7f501728e5407e79bb06ed89fc18
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360817"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="a8c72-104">Excluir programControl</span><span class="sxs-lookup"><span data-stu-id="a8c72-104">Delete programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8c72-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , exclua um objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="a8c72-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="a8c72-106">Isso desvincula uma revisão do Access de um programa.</span><span class="sxs-lookup"><span data-stu-id="a8c72-106">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="a8c72-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8c72-107">Permissions</span></span>
<span data-ttu-id="a8c72-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8c72-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8c72-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8c72-110">Permission type</span></span>                        | <span data-ttu-id="a8c72-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8c72-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8c72-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8c72-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8c72-113">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8c72-113">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="a8c72-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8c72-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8c72-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8c72-115">Not supported.</span></span> |
|<span data-ttu-id="a8c72-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8c72-116">Application</span></span>                            | <span data-ttu-id="a8c72-117">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8c72-117">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="a8c72-118">O usuário conectado também deve estar em uma função de diretório que permite excluir um `programControl`.</span><span class="sxs-lookup"><span data-stu-id="a8c72-118">The signed in user must also be in a directory role that permits them to delete a `programControl`.</span></span>

## <a name="http-request"></a><span data-ttu-id="a8c72-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8c72-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="a8c72-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8c72-120">Request headers</span></span>
| <span data-ttu-id="a8c72-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a8c72-121">Name</span></span>         | <span data-ttu-id="a8c72-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8c72-122">Type</span></span>        | <span data-ttu-id="a8c72-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8c72-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a8c72-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8c72-124">Authorization</span></span> | <span data-ttu-id="a8c72-125">string</span><span class="sxs-lookup"><span data-stu-id="a8c72-125">string</span></span> | <span data-ttu-id="a8c72-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8c72-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8c72-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8c72-128">Request body</span></span>
<span data-ttu-id="a8c72-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a8c72-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a8c72-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8c72-130">Response</span></span>
<span data-ttu-id="a8c72-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8c72-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8c72-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8c72-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8c72-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8c72-134">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a8c72-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8c72-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a8c72-136">C#</span><span class="sxs-lookup"><span data-stu-id="a8c72-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-programcontrol-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8c72-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8c72-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-programcontrol-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a8c72-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a8c72-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-programcontrol-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a8c72-139">Java</span><span class="sxs-lookup"><span data-stu-id="a8c72-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-programcontrol-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a8c72-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8c72-140">Response</span></span>
><span data-ttu-id="a8c72-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8c72-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
