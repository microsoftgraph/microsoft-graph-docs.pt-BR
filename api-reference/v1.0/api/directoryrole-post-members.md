---
title: Adicionar membro da função de diretório
description: Use esta API para criar um novo membro de função de diretório.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a4db3323494847fce68923b7e8b85197f9ee8ff5
ms.sourcegitcommit: 27e8ddb53b699f70b676c9648db8f06bb8d831a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/27/2019
ms.locfileid: "35918017"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="9c307-103">Adicionar membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="9c307-103">Add directory role member</span></span>

<span data-ttu-id="9c307-104">Use esta API para criar um novo membro de função de diretório.</span><span class="sxs-lookup"><span data-stu-id="9c307-104">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c307-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c307-105">Permissions</span></span>
<span data-ttu-id="9c307-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c307-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c307-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c307-108">Permission type</span></span>      | <span data-ttu-id="9c307-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c307-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c307-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c307-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9c307-111">RoleManagement. ReadWrite. Directory, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="9c307-111">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9c307-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c307-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c307-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c307-113">Not supported.</span></span>    |
|<span data-ttu-id="9c307-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c307-114">Application</span></span> | <span data-ttu-id="9c307-115">RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="9c307-115">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c307-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c307-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="9c307-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c307-117">Request headers</span></span>
| <span data-ttu-id="9c307-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9c307-118">Name</span></span>       | <span data-ttu-id="9c307-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c307-119">Type</span></span> | <span data-ttu-id="9c307-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c307-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9c307-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c307-121">Authorization</span></span>  | <span data-ttu-id="9c307-122">string</span><span class="sxs-lookup"><span data-stu-id="9c307-122">string</span></span>  | <span data-ttu-id="9c307-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c307-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9c307-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9c307-125">Content-Type</span></span>  | <span data-ttu-id="9c307-126">string</span><span class="sxs-lookup"><span data-stu-id="9c307-126">string</span></span>  | <span data-ttu-id="9c307-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9c307-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9c307-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c307-128">Request body</span></span>
<span data-ttu-id="9c307-129">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="9c307-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="9c307-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c307-130">Response</span></span>

<span data-ttu-id="9c307-131">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9c307-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9c307-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c307-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c307-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c307-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9c307-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c307-134">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9c307-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="9c307-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9c307-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9c307-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="9c307-137">C#</span><span class="sxs-lookup"><span data-stu-id="9c307-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9c307-138">Java</span><span class="sxs-lookup"><span data-stu-id="9c307-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9c307-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c307-139">Response</span></span>
<span data-ttu-id="9c307-140">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="9c307-140">Note: The response object shown here may be truncated for brevity.</span></span> 
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
