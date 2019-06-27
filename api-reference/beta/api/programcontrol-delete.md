---
title: Excluir programControl
description: No recurso de revisões do Azure AD Access, exclua um objeto programControl.  Isso desvincula uma revisão do Access de um programa.
localization_priority: Normal
ms.openlocfilehash: ddbd040d05d6e2c236a024e3d5eb8710562cebe9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264089"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="31aa4-104">Excluir programControl</span><span class="sxs-lookup"><span data-stu-id="31aa4-104">Delete programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31aa4-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , exclua um objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="31aa4-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="31aa4-106">Isso desvincula uma revisão do Access de um programa.</span><span class="sxs-lookup"><span data-stu-id="31aa4-106">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="31aa4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="31aa4-107">Permissions</span></span>
<span data-ttu-id="31aa4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31aa4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31aa4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31aa4-110">Permission type</span></span>                        | <span data-ttu-id="31aa4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31aa4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="31aa4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31aa4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="31aa4-113">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31aa4-113">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="31aa4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31aa4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31aa4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31aa4-115">Not supported.</span></span> |
|<span data-ttu-id="31aa4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31aa4-116">Application</span></span>                            | <span data-ttu-id="31aa4-117">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31aa4-117">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="31aa4-118">O usuário conectado também deve estar em uma função de diretório que permite excluir um `programControl`.</span><span class="sxs-lookup"><span data-stu-id="31aa4-118">The signed in user must also be in a directory role that permits them to delete a `programControl`.</span></span>

## <a name="http-request"></a><span data-ttu-id="31aa4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31aa4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="31aa4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31aa4-120">Request headers</span></span>
| <span data-ttu-id="31aa4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="31aa4-121">Name</span></span>         | <span data-ttu-id="31aa4-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="31aa4-122">Type</span></span>        | <span data-ttu-id="31aa4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="31aa4-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="31aa4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="31aa4-124">Authorization</span></span> | <span data-ttu-id="31aa4-125">string</span><span class="sxs-lookup"><span data-stu-id="31aa4-125">string</span></span> | <span data-ttu-id="31aa4-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31aa4-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31aa4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31aa4-128">Request body</span></span>
<span data-ttu-id="31aa4-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="31aa4-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="31aa4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="31aa4-130">Response</span></span>
<span data-ttu-id="31aa4-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31aa4-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31aa4-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31aa4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31aa4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31aa4-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
##### <a name="response"></a><span data-ttu-id="31aa4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="31aa4-135">Response</span></span>
><span data-ttu-id="31aa4-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31aa4-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="31aa4-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="31aa4-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="31aa4-139">C#</span><span class="sxs-lookup"><span data-stu-id="31aa4-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_programControl-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="31aa4-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="31aa4-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_programControl-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="31aa4-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="31aa4-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_programControl-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/programcontrol-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/programcontrol-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/programcontrol-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
