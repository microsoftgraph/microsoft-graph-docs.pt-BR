---
title: Adicionar membro da função de diretório
description: Use esta API para criar um novo membro de função de diretório.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bf7b88596ea2735c38d2fe258ba398ee6c48906b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264635"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="52d71-103">Adicionar membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="52d71-103">Add directory role member</span></span>

<span data-ttu-id="52d71-104">Use esta API para criar um novo membro de função de diretório.</span><span class="sxs-lookup"><span data-stu-id="52d71-104">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="52d71-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="52d71-105">Permissions</span></span>
<span data-ttu-id="52d71-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52d71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52d71-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52d71-108">Permission type</span></span>      | <span data-ttu-id="52d71-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52d71-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52d71-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52d71-110">Delegated (work or school account)</span></span> | <span data-ttu-id="52d71-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="52d71-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="52d71-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52d71-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52d71-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52d71-113">Not supported.</span></span>    |
|<span data-ttu-id="52d71-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52d71-114">Application</span></span> | <span data-ttu-id="52d71-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52d71-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52d71-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52d71-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="52d71-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52d71-117">Request headers</span></span>
| <span data-ttu-id="52d71-118">Nome</span><span class="sxs-lookup"><span data-stu-id="52d71-118">Name</span></span>       | <span data-ttu-id="52d71-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="52d71-119">Type</span></span> | <span data-ttu-id="52d71-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="52d71-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="52d71-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="52d71-121">Authorization</span></span>  | <span data-ttu-id="52d71-122">string</span><span class="sxs-lookup"><span data-stu-id="52d71-122">string</span></span>  | <span data-ttu-id="52d71-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52d71-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52d71-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="52d71-125">Content-Type</span></span>  | <span data-ttu-id="52d71-126">string</span><span class="sxs-lookup"><span data-stu-id="52d71-126">string</span></span>  | <span data-ttu-id="52d71-127">application/json</span><span class="sxs-lookup"><span data-stu-id="52d71-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="52d71-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52d71-128">Request body</span></span>
<span data-ttu-id="52d71-129">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="52d71-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="52d71-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="52d71-130">Response</span></span>

<span data-ttu-id="52d71-131">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="52d71-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="52d71-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52d71-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52d71-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52d71-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

##### <a name="response"></a><span data-ttu-id="52d71-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="52d71-134">Response</span></span>
<span data-ttu-id="52d71-135">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="52d71-135">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="52d71-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="52d71-136">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52d71-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="52d71-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_directoryrole-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="52d71-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="52d71-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_directoryrole-Objective-C-snippets.md)]
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
    "Error: /api-reference/v1.0/api/directoryrole-post-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directoryrole-post-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
