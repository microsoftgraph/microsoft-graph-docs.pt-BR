---
title: Adicionar membro da função de diretório
description: Use esta API para criar um novo membro de função de diretório.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 82f42024bab578ffd70d0a13007b8b0b3eef2fbd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517920"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="a8b1b-103">Adicionar membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="a8b1b-103">Add directory role member</span></span>

<span data-ttu-id="a8b1b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8b1b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a8b1b-105">Use esta API para criar um novo membro de função de diretório.</span><span class="sxs-lookup"><span data-stu-id="a8b1b-105">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8b1b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8b1b-106">Permissions</span></span>
<span data-ttu-id="a8b1b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8b1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8b1b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8b1b-109">Permission type</span></span>      | <span data-ttu-id="a8b1b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8b1b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8b1b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8b1b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a8b1b-112">RoleManagement. ReadWrite. Directory, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="a8b1b-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a8b1b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8b1b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8b1b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8b1b-114">Not supported.</span></span>    |
|<span data-ttu-id="a8b1b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8b1b-115">Application</span></span> | <span data-ttu-id="a8b1b-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="a8b1b-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8b1b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8b1b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="a8b1b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8b1b-118">Request headers</span></span>
| <span data-ttu-id="a8b1b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a8b1b-119">Name</span></span>       | <span data-ttu-id="a8b1b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8b1b-120">Type</span></span> | <span data-ttu-id="a8b1b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8b1b-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a8b1b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8b1b-122">Authorization</span></span>  | <span data-ttu-id="a8b1b-123">string</span><span class="sxs-lookup"><span data-stu-id="a8b1b-123">string</span></span>  | <span data-ttu-id="a8b1b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8b1b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a8b1b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a8b1b-126">Content-Type</span></span>  | <span data-ttu-id="a8b1b-127">string</span><span class="sxs-lookup"><span data-stu-id="a8b1b-127">string</span></span>  | <span data-ttu-id="a8b1b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a8b1b-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a8b1b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8b1b-129">Request body</span></span>
<span data-ttu-id="a8b1b-130">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="a8b1b-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="a8b1b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8b1b-131">Response</span></span>

<span data-ttu-id="a8b1b-132">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a8b1b-132">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a8b1b-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8b1b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8b1b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8b1b-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a8b1b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8b1b-135">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="a8b1b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8b1b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8b1b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8b1b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="a8b1b-138">C#</span><span class="sxs-lookup"><span data-stu-id="a8b1b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8b1b-139">Java</span><span class="sxs-lookup"><span data-stu-id="a8b1b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a8b1b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8b1b-140">Response</span></span>
<span data-ttu-id="a8b1b-141">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="a8b1b-141">Note: The response object shown here may be truncated for brevity.</span></span> 
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
