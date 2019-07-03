---
title: Remover membro
description: Use essa API para remover um membro de um grupo por meio **da** propriedade de navegação membros.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 688e93da20d247aee2250f1c21c329703f668522
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448107"
---
# <a name="remove-member"></a><span data-ttu-id="0c4a8-103">Remover membro</span><span class="sxs-lookup"><span data-stu-id="0c4a8-103">Remove member</span></span>
<span data-ttu-id="0c4a8-104">Use essa API para remover um membro de um grupo por meio **da** propriedade de navegação membros.</span><span class="sxs-lookup"><span data-stu-id="0c4a8-104">Use this API to remove a member from an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c4a8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0c4a8-105">Permissions</span></span>
<span data-ttu-id="0c4a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c4a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c4a8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c4a8-108">Permission type</span></span>      | <span data-ttu-id="0c4a8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c4a8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c4a8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c4a8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0c4a8-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0c4a8-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="0c4a8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c4a8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c4a8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c4a8-113">Not supported.</span></span> |
|<span data-ttu-id="0c4a8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c4a8-114">Application</span></span> | <span data-ttu-id="0c4a8-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c4a8-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c4a8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c4a8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0c4a8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c4a8-117">Request headers</span></span>
| <span data-ttu-id="0c4a8-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0c4a8-118">Name</span></span>       | <span data-ttu-id="0c4a8-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c4a8-119">Type</span></span> | <span data-ttu-id="0c4a8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c4a8-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0c4a8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c4a8-121">Authorization</span></span>  | <span data-ttu-id="0c4a8-122">string</span><span class="sxs-lookup"><span data-stu-id="0c4a8-122">string</span></span>  | <span data-ttu-id="0c4a8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c4a8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c4a8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c4a8-125">Request body</span></span>
<span data-ttu-id="0c4a8-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0c4a8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c4a8-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c4a8-127">Response</span></span>
<span data-ttu-id="0c4a8-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c4a8-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c4a8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c4a8-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0c4a8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c4a8-131">Request</span></span>
<span data-ttu-id="0c4a8-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c4a8-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0c4a8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c4a8-133">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c4a8-134">C#</span><span class="sxs-lookup"><span data-stu-id="0c4a8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c4a8-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="0c4a8-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c4a8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c4a8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0c4a8-137">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="0c4a8-137">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="0c4a8-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c4a8-138">Response</span></span>
<span data-ttu-id="0c4a8-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0c4a8-139">The following is an example of the response.</span></span>
><span data-ttu-id="0c4a8-140">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0c4a8-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0c4a8-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c4a8-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
