---
title: Criar ContactFolder
description: Crie uma nova contactFolder sob a pasta de contatos padrão do usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2ed499640f12894dc19c8da7122804134b9b9781
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421938"
---
# <a name="create-contactfolder"></a><span data-ttu-id="a4ab0-103">Criar ContactFolder</span><span class="sxs-lookup"><span data-stu-id="a4ab0-103">Create ContactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4ab0-104">Crie uma nova contactFolder sob a pasta de contatos padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="a4ab0-104">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="a4ab0-105">Você também pode [criar uma nova contactfolder como um filho de qualquer pasta de contatos especificada](contactfolder-post-childfolders.md).</span><span class="sxs-lookup"><span data-stu-id="a4ab0-105">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a4ab0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4ab0-106">Permissions</span></span>
<span data-ttu-id="a4ab0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4ab0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4ab0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4ab0-109">Permission type</span></span>      | <span data-ttu-id="a4ab0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4ab0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4ab0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4ab0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a4ab0-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4ab0-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a4ab0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4ab0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4ab0-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4ab0-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a4ab0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4ab0-115">Application</span></span> | <span data-ttu-id="a4ab0-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4ab0-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4ab0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4ab0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="a4ab0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4ab0-118">Request headers</span></span>
| <span data-ttu-id="a4ab0-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a4ab0-119">Header</span></span>       | <span data-ttu-id="a4ab0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a4ab0-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a4ab0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4ab0-121">Authorization</span></span>  | <span data-ttu-id="a4ab0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4ab0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a4ab0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a4ab0-124">Content-Type</span></span>  | <span data-ttu-id="a4ab0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4ab0-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a4ab0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4ab0-126">Request body</span></span>
<span data-ttu-id="a4ab0-127">No corpo da solicitação, forneça uma representação JSON do objeto [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a4ab0-127">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a4ab0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4ab0-128">Response</span></span>

<span data-ttu-id="a4ab0-129">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4ab0-129">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4ab0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4ab0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a4ab0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4ab0-131">Request</span></span>
<span data-ttu-id="a4ab0-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4ab0-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a4ab0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4ab0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a4ab0-134">C#</span><span class="sxs-lookup"><span data-stu-id="a4ab0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contactfolder-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a4ab0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4ab0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contactfolder-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a4ab0-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a4ab0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contactfolder-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a4ab0-137">No corpo da solicitação, forneça uma representação JSON do objeto [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a4ab0-137">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a4ab0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4ab0-138">Response</span></span>
<span data-ttu-id="a4ab0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a4ab0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
