---
title: Adicionar membro da função de diretório
description: Use esta API para criar um novo membro de função de diretório.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 00b9eaef51f282e891a279fa24a17e20a91102a6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460998"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="81de3-103">Adicionar membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="81de3-103">Add directory role member</span></span>

<span data-ttu-id="81de3-104">Use esta API para criar um novo membro de função de diretório.</span><span class="sxs-lookup"><span data-stu-id="81de3-104">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="81de3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="81de3-105">Permissions</span></span>
<span data-ttu-id="81de3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81de3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81de3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81de3-108">Permission type</span></span>      | <span data-ttu-id="81de3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81de3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81de3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81de3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="81de3-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="81de3-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="81de3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81de3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81de3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81de3-113">Not supported.</span></span>    |
|<span data-ttu-id="81de3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81de3-114">Application</span></span> | <span data-ttu-id="81de3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81de3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81de3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81de3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="81de3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81de3-117">Request headers</span></span>
| <span data-ttu-id="81de3-118">Nome</span><span class="sxs-lookup"><span data-stu-id="81de3-118">Name</span></span>       | <span data-ttu-id="81de3-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="81de3-119">Type</span></span> | <span data-ttu-id="81de3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="81de3-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="81de3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="81de3-121">Authorization</span></span>  | <span data-ttu-id="81de3-122">string</span><span class="sxs-lookup"><span data-stu-id="81de3-122">string</span></span>  | <span data-ttu-id="81de3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81de3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81de3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="81de3-125">Content-Type</span></span>  | <span data-ttu-id="81de3-126">string</span><span class="sxs-lookup"><span data-stu-id="81de3-126">string</span></span>  | <span data-ttu-id="81de3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="81de3-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="81de3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81de3-128">Request body</span></span>
<span data-ttu-id="81de3-129">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="81de3-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="81de3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="81de3-130">Response</span></span>

<span data-ttu-id="81de3-131">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="81de3-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="81de3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81de3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81de3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81de3-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="81de3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="81de3-134">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="81de3-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="81de3-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="81de3-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="81de3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="81de3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="81de3-137">Response</span></span>
<span data-ttu-id="81de3-138">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="81de3-138">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

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
