---
title: Adicionar membro da função de diretório
description: Use esta API para criar um novo membro de função de diretório.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 04cf9a62fb4929a5f8df53a796374366cf6fd267
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052380"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="c879a-103">Adicionar membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="c879a-103">Add directory role member</span></span>

<span data-ttu-id="c879a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c879a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c879a-105">Use esta API para criar um novo membro de função de diretório.</span><span class="sxs-lookup"><span data-stu-id="c879a-105">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="c879a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c879a-106">Permissions</span></span>
<span data-ttu-id="c879a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c879a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c879a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c879a-109">Permission type</span></span>      | <span data-ttu-id="c879a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c879a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c879a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c879a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c879a-112">RoleManagement. ReadWrite. Directory, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="c879a-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c879a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c879a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c879a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c879a-114">Not supported.</span></span>    |
|<span data-ttu-id="c879a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c879a-115">Application</span></span> | <span data-ttu-id="c879a-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="c879a-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="c879a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c879a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="c879a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c879a-118">Request headers</span></span>
| <span data-ttu-id="c879a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c879a-119">Name</span></span>       | <span data-ttu-id="c879a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c879a-120">Type</span></span> | <span data-ttu-id="c879a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c879a-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c879a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c879a-122">Authorization</span></span>  | <span data-ttu-id="c879a-123">string</span><span class="sxs-lookup"><span data-stu-id="c879a-123">string</span></span>  | <span data-ttu-id="c879a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c879a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c879a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c879a-126">Content-Type</span></span>  | <span data-ttu-id="c879a-127">string</span><span class="sxs-lookup"><span data-stu-id="c879a-127">string</span></span>  | <span data-ttu-id="c879a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c879a-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c879a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c879a-129">Request body</span></span>
<span data-ttu-id="c879a-130">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="c879a-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="c879a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c879a-131">Response</span></span>

<span data-ttu-id="c879a-132">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c879a-132">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c879a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c879a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c879a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c879a-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c879a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c879a-135">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="c879a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c879a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c879a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c879a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="c879a-138">C#</span><span class="sxs-lookup"><span data-stu-id="c879a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c879a-139">Java</span><span class="sxs-lookup"><span data-stu-id="c879a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c879a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c879a-140">Response</span></span>
<span data-ttu-id="c879a-141">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="c879a-141">Note: The response object shown here may be truncated for brevity.</span></span> 
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

