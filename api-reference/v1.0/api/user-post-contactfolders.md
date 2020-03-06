---
title: Criar ContactFolder
description: Crie uma nova contactFolder sob a pasta de contatos padrão do usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7a0729bc61881606106340dffbc765040386d0e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508993"
---
# <a name="create-contactfolder"></a><span data-ttu-id="abf33-103">Criar ContactFolder</span><span class="sxs-lookup"><span data-stu-id="abf33-103">Create ContactFolder</span></span>

<span data-ttu-id="abf33-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abf33-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="abf33-105">Crie uma nova contactFolder sob a pasta de contatos padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="abf33-105">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="abf33-106">Você também pode [criar uma nova contactfolder como um filho de qualquer pasta de contatos especificada](contactfolder-post-childfolders.md).</span><span class="sxs-lookup"><span data-stu-id="abf33-106">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="abf33-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="abf33-107">Permissions</span></span>
<span data-ttu-id="abf33-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abf33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abf33-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abf33-110">Permission type</span></span>      | <span data-ttu-id="abf33-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="abf33-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abf33-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abf33-112">Delegated (work or school account)</span></span> | <span data-ttu-id="abf33-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="abf33-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="abf33-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abf33-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abf33-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="abf33-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="abf33-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abf33-116">Application</span></span> | <span data-ttu-id="abf33-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="abf33-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="abf33-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abf33-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="abf33-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abf33-119">Request headers</span></span>
| <span data-ttu-id="abf33-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abf33-120">Header</span></span>       | <span data-ttu-id="abf33-121">Valor</span><span class="sxs-lookup"><span data-stu-id="abf33-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="abf33-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="abf33-122">Authorization</span></span>  | <span data-ttu-id="abf33-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abf33-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="abf33-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="abf33-125">Content-Type</span></span>  | <span data-ttu-id="abf33-126">application/json</span><span class="sxs-lookup"><span data-stu-id="abf33-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="abf33-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abf33-127">Request body</span></span>
<span data-ttu-id="abf33-128">No corpo da solicitação, forneça uma representação JSON do objeto [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="abf33-128">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="abf33-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="abf33-129">Response</span></span>

<span data-ttu-id="abf33-130">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abf33-130">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abf33-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abf33-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="abf33-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abf33-132">Request</span></span>
<span data-ttu-id="abf33-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abf33-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="abf33-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="abf33-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
# <a name="c"></a>[<span data-ttu-id="abf33-135">C#</span><span class="sxs-lookup"><span data-stu-id="abf33-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contactfolder-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="abf33-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="abf33-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contactfolder-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="abf33-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="abf33-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contactfolder-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="abf33-138">Java</span><span class="sxs-lookup"><span data-stu-id="abf33-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contactfolder-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="abf33-139">No corpo da solicitação, forneça uma representação JSON do objeto [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="abf33-139">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="abf33-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="abf33-140">Response</span></span>
<span data-ttu-id="abf33-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="abf33-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
