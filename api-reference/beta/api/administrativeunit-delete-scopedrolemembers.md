---
title: Remover um scopedRoleMember
description: Remover um membro de função com escopo de uma unidade administrativa.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8bf7eff918b9b3e333dc0b5c19f787416675ffb6
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655415"
---
# <a name="remove-a-scopedrolemember"></a><span data-ttu-id="06741-103">Remover um scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="06741-103">Remove a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06741-104">Remover um membro de função com escopo de uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="06741-104">Remove a scoped-role member from an adminstrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="06741-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="06741-105">Permissions</span></span>
<span data-ttu-id="06741-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06741-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="06741-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06741-108">Permission type</span></span>      | <span data-ttu-id="06741-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06741-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06741-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06741-110">Delegated (work or school account)</span></span> | <span data-ttu-id="06741-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="06741-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="06741-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06741-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06741-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06741-113">Not supported.</span></span>    |
|<span data-ttu-id="06741-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06741-114">Application</span></span> | <span data-ttu-id="06741-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06741-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="06741-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06741-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/scopedRoleMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="06741-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06741-117">Request headers</span></span>
| <span data-ttu-id="06741-118">Nome</span><span class="sxs-lookup"><span data-stu-id="06741-118">Name</span></span>       | <span data-ttu-id="06741-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="06741-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="06741-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="06741-120">Authorization</span></span>  | <span data-ttu-id="06741-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06741-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06741-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06741-123">Request body</span></span>
<span data-ttu-id="06741-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="06741-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06741-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="06741-125">Response</span></span>

<span data-ttu-id="06741-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06741-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06741-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06741-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06741-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06741-129">Request</span></span>
<span data-ttu-id="06741-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06741-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_scopedrolemember"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
##### <a name="response"></a><span data-ttu-id="06741-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="06741-131">Response</span></span>
<span data-ttu-id="06741-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06741-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="06741-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="06741-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="06741-136">C#</span><span class="sxs-lookup"><span data-stu-id="06741-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_scopedrolemember-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="06741-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="06741-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_scopedrolemember-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-delete-scopedrolemembers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/administrativeunit-delete-scopedrolemembers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
