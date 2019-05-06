---
title: Remover membro
description: Use esta API para remover um membro de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação **membros**. É possível remover usuários ou outros grupos.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 56b717556fd129f30ba5e2957a7779ea1c6a8a05
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593332"
---
# <a name="remove-member"></a><span data-ttu-id="c6903-104">Remover membro</span><span class="sxs-lookup"><span data-stu-id="c6903-104">Remove member</span></span>
<span data-ttu-id="c6903-p102">Use esta API para remover um membro de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação **membros**. É possível remover usuários ou outros grupos.</span><span class="sxs-lookup"><span data-stu-id="c6903-p102">Use this API to remove a member from an Office 365 group, a security group, or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6903-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6903-107">Permissions</span></span>
<span data-ttu-id="c6903-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6903-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6903-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6903-110">Permission type</span></span>      | <span data-ttu-id="c6903-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6903-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6903-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6903-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c6903-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c6903-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c6903-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6903-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6903-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6903-115">Not supported.</span></span>    |
|<span data-ttu-id="c6903-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6903-116">Application</span></span> | <span data-ttu-id="c6903-117">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6903-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c6903-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6903-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c6903-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6903-119">Request headers</span></span>
| <span data-ttu-id="c6903-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c6903-120">Name</span></span>       | <span data-ttu-id="c6903-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6903-121">Type</span></span> | <span data-ttu-id="c6903-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6903-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c6903-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6903-123">Authorization</span></span>  | <span data-ttu-id="c6903-124">string</span><span class="sxs-lookup"><span data-stu-id="c6903-124">string</span></span>  | <span data-ttu-id="c6903-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6903-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6903-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6903-127">Request body</span></span>
<span data-ttu-id="c6903-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c6903-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6903-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6903-129">Response</span></span>
<span data-ttu-id="c6903-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6903-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6903-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6903-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c6903-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6903-133">Request</span></span>
<span data-ttu-id="c6903-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6903-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="c6903-135">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="c6903-135">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="c6903-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6903-136">Response</span></span>
<span data-ttu-id="c6903-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c6903-137">The following is an example of the response.</span></span>
><span data-ttu-id="c6903-138">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c6903-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c6903-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6903-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c6903-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c6903-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c6903-141">Basic</span><span class="sxs-lookup"><span data-stu-id="c6903-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6903-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6903-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/api/group-delete-members.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-delete-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
