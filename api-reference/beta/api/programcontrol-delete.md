---
title: Excluir programControl
description: No recurso de revisões do Azure AD Access, exclua um objeto programControl.  Isso desvincula uma revisão do Access de um programa.
localization_priority: Normal
ms.openlocfilehash: 6883c1683529338545be3a65629fdb6961d6c4bb
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33610718"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="5caad-104">Excluir programControl</span><span class="sxs-lookup"><span data-stu-id="5caad-104">Delete programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5caad-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , exclua um objeto [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="5caad-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="5caad-106">Isso desvincula uma revisão do Access de um programa.</span><span class="sxs-lookup"><span data-stu-id="5caad-106">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="5caad-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5caad-107">Permissions</span></span>
<span data-ttu-id="5caad-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5caad-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5caad-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5caad-110">Permission type</span></span>                        | <span data-ttu-id="5caad-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5caad-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5caad-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5caad-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5caad-113">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5caad-113">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="5caad-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5caad-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5caad-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5caad-115">Not supported.</span></span> |
|<span data-ttu-id="5caad-116">Application</span><span class="sxs-lookup"><span data-stu-id="5caad-116">Application</span></span>                            | <span data-ttu-id="5caad-117">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5caad-117">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="5caad-118">O usuário conectado também deve estar em uma função de diretório que permite excluir um `programControl`.</span><span class="sxs-lookup"><span data-stu-id="5caad-118">The signed in user must also be in a directory role that permits them to delete a `programControl`.</span></span>

## <a name="http-request"></a><span data-ttu-id="5caad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5caad-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="5caad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5caad-120">Request headers</span></span>
| <span data-ttu-id="5caad-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5caad-121">Name</span></span>         | <span data-ttu-id="5caad-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="5caad-122">Type</span></span>        | <span data-ttu-id="5caad-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5caad-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5caad-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5caad-124">Authorization</span></span> | <span data-ttu-id="5caad-125">string</span><span class="sxs-lookup"><span data-stu-id="5caad-125">string</span></span> | <span data-ttu-id="5caad-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5caad-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5caad-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5caad-128">Request body</span></span>
<span data-ttu-id="5caad-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5caad-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5caad-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5caad-130">Response</span></span>
<span data-ttu-id="5caad-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5caad-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5caad-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5caad-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5caad-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5caad-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
##### <a name="response"></a><span data-ttu-id="5caad-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5caad-135">Response</span></span>
><span data-ttu-id="5caad-p106">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5caad-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5caad-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5caad-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5caad-139">Basic</span><span class="sxs-lookup"><span data-stu-id="5caad-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_programControl-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5caad-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5caad-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_programControl-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/programcontrol-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/programcontrol-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
