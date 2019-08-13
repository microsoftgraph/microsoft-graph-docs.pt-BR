---
title: Remover proprietário
description: Use esta API para remover um proprietário de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação owners.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7bf3bee1b45886332ba8a203da7ff7808a37fe49
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326405"
---
# <a name="remove-owner"></a><span data-ttu-id="4bdbd-103">Remover proprietário</span><span class="sxs-lookup"><span data-stu-id="4bdbd-103">Remove owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bdbd-104">Use esta API para remover um proprietário de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação owners.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-104">Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="4bdbd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4bdbd-105">Permissions</span></span>
<span data-ttu-id="4bdbd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bdbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bdbd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bdbd-108">Permission type</span></span>      | <span data-ttu-id="4bdbd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4bdbd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bdbd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bdbd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4bdbd-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4bdbd-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4bdbd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bdbd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bdbd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-113">Not supported.</span></span>    |
|<span data-ttu-id="4bdbd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bdbd-114">Application</span></span> | <span data-ttu-id="4bdbd-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bdbd-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bdbd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bdbd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="4bdbd-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bdbd-117">Request headers</span></span>
| <span data-ttu-id="4bdbd-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4bdbd-118">Name</span></span>       | <span data-ttu-id="4bdbd-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bdbd-119">Type</span></span> | <span data-ttu-id="4bdbd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bdbd-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4bdbd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4bdbd-121">Authorization</span></span>  | <span data-ttu-id="4bdbd-122">string</span><span class="sxs-lookup"><span data-stu-id="4bdbd-122">string</span></span>  | <span data-ttu-id="4bdbd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bdbd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4bdbd-125">Request body</span></span>
<span data-ttu-id="4bdbd-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bdbd-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bdbd-127">Response</span></span>
<span data-ttu-id="4bdbd-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bdbd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bdbd-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4bdbd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bdbd-131">Request</span></span>
<span data-ttu-id="4bdbd-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4bdbd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4bdbd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/owners/{id}/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4bdbd-134">C#</span><span class="sxs-lookup"><span data-stu-id="4bdbd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4bdbd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4bdbd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4bdbd-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4bdbd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4bdbd-137">Java</span><span class="sxs-lookup"><span data-stu-id="4bdbd-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4bdbd-138">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-138">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="4bdbd-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bdbd-139">Response</span></span>
<span data-ttu-id="4bdbd-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-140">The following is an example of the response.</span></span>
><span data-ttu-id="4bdbd-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4bdbd-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4bdbd-142">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
