---
title: Remover um scopedRoleMember
description: Remover um membro de função com escopo de uma unidade administrativa.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 90272c109e7304071f7245f588607c764999d0b2
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636678"
---
# <a name="remove-a-scopedrolemember"></a><span data-ttu-id="3ee86-103">Remover um scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="3ee86-103">Remove a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ee86-104">Remover um membro de função com escopo de uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="3ee86-104">Remove a scoped-role member from an adminstrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ee86-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ee86-105">Permissions</span></span>
<span data-ttu-id="3ee86-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ee86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3ee86-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ee86-108">Permission type</span></span>      | <span data-ttu-id="3ee86-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ee86-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ee86-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ee86-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3ee86-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3ee86-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3ee86-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ee86-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ee86-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ee86-113">Not supported.</span></span>    |
|<span data-ttu-id="3ee86-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ee86-114">Application</span></span> | <span data-ttu-id="3ee86-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ee86-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ee86-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ee86-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/scopedRoleMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="3ee86-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ee86-117">Request headers</span></span>
| <span data-ttu-id="3ee86-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3ee86-118">Name</span></span>       | <span data-ttu-id="3ee86-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ee86-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3ee86-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ee86-120">Authorization</span></span>  | <span data-ttu-id="3ee86-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ee86-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ee86-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ee86-123">Request body</span></span>
<span data-ttu-id="3ee86-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3ee86-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ee86-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ee86-125">Response</span></span>

<span data-ttu-id="3ee86-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ee86-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ee86-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ee86-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ee86-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ee86-129">Request</span></span>
<span data-ttu-id="3ee86-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ee86-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_scopedrolemember"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
##### <a name="response"></a><span data-ttu-id="3ee86-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ee86-131">Response</span></span>
<span data-ttu-id="3ee86-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ee86-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3ee86-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3ee86-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3ee86-136">Basic</span><span class="sxs-lookup"><span data-stu-id="3ee86-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_scopedrolemember-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3ee86-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ee86-137">Javascript</span></span>](#tab/javascript)
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
