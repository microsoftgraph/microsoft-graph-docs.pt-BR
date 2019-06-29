---
title: Remover membro
description: Use essa API para remover um membro de um grupo por meio **da** propriedade de navegação membros.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 87ab921912afeeb3b094c8e30d5678741eaddd66
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275821"
---
# <a name="remove-member"></a><span data-ttu-id="1fbaf-103">Remover membro</span><span class="sxs-lookup"><span data-stu-id="1fbaf-103">Remove member</span></span>
<span data-ttu-id="1fbaf-104">Use essa API para remover um membro de um grupo por meio **da** propriedade de navegação membros.</span><span class="sxs-lookup"><span data-stu-id="1fbaf-104">Use this API to remove a member from an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fbaf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1fbaf-105">Permissions</span></span>
<span data-ttu-id="1fbaf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fbaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fbaf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fbaf-108">Permission type</span></span>      | <span data-ttu-id="1fbaf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1fbaf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fbaf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fbaf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1fbaf-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1fbaf-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="1fbaf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fbaf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fbaf-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fbaf-113">Not supported.</span></span> |
|<span data-ttu-id="1fbaf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fbaf-114">Application</span></span> | <span data-ttu-id="1fbaf-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fbaf-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fbaf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fbaf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="1fbaf-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fbaf-117">Request headers</span></span>
| <span data-ttu-id="1fbaf-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1fbaf-118">Name</span></span>       | <span data-ttu-id="1fbaf-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fbaf-119">Type</span></span> | <span data-ttu-id="1fbaf-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fbaf-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1fbaf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fbaf-121">Authorization</span></span>  | <span data-ttu-id="1fbaf-122">string</span><span class="sxs-lookup"><span data-stu-id="1fbaf-122">string</span></span>  | <span data-ttu-id="1fbaf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fbaf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fbaf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fbaf-125">Request body</span></span>
<span data-ttu-id="1fbaf-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1fbaf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fbaf-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fbaf-127">Response</span></span>
<span data-ttu-id="1fbaf-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fbaf-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fbaf-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1fbaf-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1fbaf-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fbaf-131">Request</span></span>
<span data-ttu-id="1fbaf-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fbaf-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="1fbaf-133">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="1fbaf-133">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="1fbaf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fbaf-134">Response</span></span>
<span data-ttu-id="1fbaf-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1fbaf-135">The following is an example of the response.</span></span>
><span data-ttu-id="1fbaf-136">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1fbaf-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1fbaf-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1fbaf-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1fbaf-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="1fbaf-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1fbaf-139">C#</span><span class="sxs-lookup"><span data-stu-id="1fbaf-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1fbaf-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="1fbaf-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1fbaf-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fbaf-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-delete-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-delete-members.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-delete-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
