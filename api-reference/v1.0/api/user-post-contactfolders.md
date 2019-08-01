---
title: Criar ContactFolder
description: Crie uma nova contactFolder sob a pasta de contatos padrão do usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 62bbe7461fba4901ce367e9a45f6b573a9b8e911
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026728"
---
# <a name="create-contactfolder"></a><span data-ttu-id="7a299-103">Criar ContactFolder</span><span class="sxs-lookup"><span data-stu-id="7a299-103">Create ContactFolder</span></span>

<span data-ttu-id="7a299-104">Crie uma nova contactFolder sob a pasta de contatos padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="7a299-104">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="7a299-105">Você também pode [criar uma nova contactfolder como um filho de qualquer pasta de contatos especificada](contactfolder-post-childfolders.md).</span><span class="sxs-lookup"><span data-stu-id="7a299-105">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="7a299-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a299-106">Permissions</span></span>
<span data-ttu-id="7a299-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a299-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a299-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a299-109">Permission type</span></span>      | <span data-ttu-id="7a299-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a299-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a299-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a299-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7a299-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a299-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7a299-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a299-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a299-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a299-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7a299-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a299-115">Application</span></span> | <span data-ttu-id="7a299-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a299-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a299-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a299-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="7a299-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a299-118">Request headers</span></span>
| <span data-ttu-id="7a299-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7a299-119">Header</span></span>       | <span data-ttu-id="7a299-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7a299-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7a299-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a299-121">Authorization</span></span>  | <span data-ttu-id="7a299-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a299-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7a299-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7a299-124">Content-Type</span></span>  | <span data-ttu-id="7a299-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7a299-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7a299-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a299-126">Request body</span></span>
<span data-ttu-id="7a299-127">No corpo da solicitação, forneça uma representação JSON do objeto [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="7a299-127">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7a299-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a299-128">Response</span></span>

<span data-ttu-id="7a299-129">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a299-129">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a299-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a299-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a299-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a299-131">Request</span></span>
<span data-ttu-id="7a299-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a299-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7a299-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a299-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7a299-134">C#</span><span class="sxs-lookup"><span data-stu-id="7a299-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contactfolder-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a299-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="7a299-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contactfolder-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7a299-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7a299-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contactfolder-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7a299-137">Java</span><span class="sxs-lookup"><span data-stu-id="7a299-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contactfolder-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7a299-138">No corpo da solicitação, forneça uma representação JSON do objeto [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="7a299-138">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7a299-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a299-139">Response</span></span>
<span data-ttu-id="7a299-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a299-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
