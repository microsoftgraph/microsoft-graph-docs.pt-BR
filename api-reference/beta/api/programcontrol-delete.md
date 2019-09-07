---
title: Excluir programControl
description: No recurso de revisões do Azure AD Access, exclua um objeto programControl.  Isso desvincula uma revisão do Access de um programa.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 569b084a149308d1ea5d3bc8311e2e6d13634eaa
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792800"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="eaffb-104">Excluir programControl</span><span class="sxs-lookup"><span data-stu-id="eaffb-104">Delete programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eaffb-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , exclua um objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="eaffb-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="eaffb-106">Isso desvincula uma revisão do Access de um programa.</span><span class="sxs-lookup"><span data-stu-id="eaffb-106">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="eaffb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="eaffb-107">Permissions</span></span>
<span data-ttu-id="eaffb-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaffb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaffb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eaffb-110">Permission type</span></span>                        | <span data-ttu-id="eaffb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eaffb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="eaffb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eaffb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="eaffb-113">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaffb-113">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="eaffb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eaffb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eaffb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eaffb-115">Not supported.</span></span> |
|<span data-ttu-id="eaffb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eaffb-116">Application</span></span>                            | <span data-ttu-id="eaffb-117">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaffb-117">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="eaffb-118">O usuário conectado também deve estar em uma função de diretório que permite excluir um `programControl`.</span><span class="sxs-lookup"><span data-stu-id="eaffb-118">The signed in user must also be in a directory role that permits them to delete a `programControl`.</span></span>

## <a name="http-request"></a><span data-ttu-id="eaffb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eaffb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls/{id}
```
## <a name="request-headers"></a><span data-ttu-id="eaffb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eaffb-120">Request headers</span></span>
| <span data-ttu-id="eaffb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="eaffb-121">Name</span></span>         | <span data-ttu-id="eaffb-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="eaffb-122">Type</span></span>        | <span data-ttu-id="eaffb-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaffb-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="eaffb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="eaffb-124">Authorization</span></span> | <span data-ttu-id="eaffb-125">string</span><span class="sxs-lookup"><span data-stu-id="eaffb-125">string</span></span> | <span data-ttu-id="eaffb-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eaffb-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eaffb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eaffb-128">Request body</span></span>
<span data-ttu-id="eaffb-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eaffb-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="eaffb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaffb-130">Response</span></span>
<span data-ttu-id="eaffb-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eaffb-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaffb-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eaffb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eaffb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eaffb-134">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="eaffb-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="eaffb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eaffb-136">C#</span><span class="sxs-lookup"><span data-stu-id="eaffb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-programcontrol-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eaffb-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eaffb-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-programcontrol-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eaffb-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="eaffb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-programcontrol-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="eaffb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaffb-139">Response</span></span>
><span data-ttu-id="eaffb-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eaffb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
