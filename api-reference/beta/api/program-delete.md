---
title: Excluir programa
description: No recurso de revisões do Azure AD Access, exclua um objeto Program.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 6949a3fd6d925296711c915d7934f3e0855d0f1d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977889"
---
# <a name="delete-program"></a><span data-ttu-id="c3c0f-103">Excluir programa</span><span class="sxs-lookup"><span data-stu-id="c3c0f-103">Delete program</span></span>

<span data-ttu-id="c3c0f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3c0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3c0f-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , exclua um objeto [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="c3c0f-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="c3c0f-106">Não exclua um programa que ainda esteja `programControl` vinculado a ele, essas revisões de acesso devem primeiro ser excluídas ou desvinculadas do programa e vinculadas a um programa diferente.</span><span class="sxs-lookup"><span data-stu-id="c3c0f-106">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="c3c0f-107">Além disso, observe que o programa padrão interno não pode ser excluído.</span><span class="sxs-lookup"><span data-stu-id="c3c0f-107">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="c3c0f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3c0f-108">Permissions</span></span>
<span data-ttu-id="c3c0f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3c0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3c0f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3c0f-111">Permission type</span></span>                        | <span data-ttu-id="c3c0f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3c0f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3c0f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3c0f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c3c0f-114">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3c0f-114">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="c3c0f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3c0f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3c0f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3c0f-116">Not supported.</span></span> |
|<span data-ttu-id="c3c0f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3c0f-117">Application</span></span>                            | <span data-ttu-id="c3c0f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3c0f-118">Not supported.</span></span> |

<span data-ttu-id="c3c0f-119">O usuário conectado também deve estar em uma função de diretório que permite que eles criem um programa.</span><span class="sxs-lookup"><span data-stu-id="c3c0f-119">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="c3c0f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3c0f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c3c0f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3c0f-121">Request headers</span></span>
| <span data-ttu-id="c3c0f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c3c0f-122">Name</span></span>         | <span data-ttu-id="c3c0f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3c0f-123">Type</span></span>        | <span data-ttu-id="c3c0f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3c0f-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c3c0f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3c0f-125">Authorization</span></span> | <span data-ttu-id="c3c0f-126">string</span><span class="sxs-lookup"><span data-stu-id="c3c0f-126">string</span></span> | <span data-ttu-id="c3c0f-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3c0f-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3c0f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3c0f-129">Request body</span></span>
<span data-ttu-id="c3c0f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c3c0f-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c3c0f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3c0f-131">Response</span></span>
<span data-ttu-id="c3c0f-p104">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3c0f-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3c0f-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3c0f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3c0f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3c0f-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c3c0f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3c0f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
# <a name="c"></a>[<span data-ttu-id="c3c0f-137">C#</span><span class="sxs-lookup"><span data-stu-id="c3c0f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3c0f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3c0f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3c0f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3c0f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3c0f-140">Java</span><span class="sxs-lookup"><span data-stu-id="c3c0f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c3c0f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3c0f-141">Response</span></span>
><span data-ttu-id="c3c0f-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3c0f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


