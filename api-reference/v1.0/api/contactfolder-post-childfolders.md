---
title: Criar ContactFolder
description: 'Cria uma nova contactFolder como um filho de uma pasta especificada. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 61bf132688fbe0b7b8580c4fdb1f637b26ef7cb9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443018"
---
# <a name="create-contactfolder"></a><span data-ttu-id="ad150-103">Criar ContactFolder</span><span class="sxs-lookup"><span data-stu-id="ad150-103">Create ContactFolder</span></span>

<span data-ttu-id="ad150-104">Cria uma nova contactFolder como um filho de uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="ad150-104">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="ad150-105">Também é possível [criar uma nova contactFolder sob a pasta de contatos padrão do usuário](user-post-contactfolders.md).</span><span class="sxs-lookup"><span data-stu-id="ad150-105">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="ad150-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad150-106">Permissions</span></span>
<span data-ttu-id="ad150-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad150-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad150-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad150-109">Permission type</span></span>      | <span data-ttu-id="ad150-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad150-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad150-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad150-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ad150-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad150-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ad150-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad150-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad150-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad150-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ad150-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad150-115">Application</span></span> | <span data-ttu-id="ad150-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad150-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad150-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad150-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="ad150-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad150-118">Request headers</span></span>
| <span data-ttu-id="ad150-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ad150-119">Header</span></span>       | <span data-ttu-id="ad150-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ad150-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ad150-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad150-121">Authorization</span></span>  | <span data-ttu-id="ad150-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad150-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ad150-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ad150-124">Content-Type</span></span>  | <span data-ttu-id="ad150-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad150-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ad150-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad150-127">Request body</span></span>
<span data-ttu-id="ad150-128">No corpo da solicitação, forneça uma representação JSON do objeto [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="ad150-128">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ad150-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad150-129">Response</span></span>

<span data-ttu-id="ad150-130">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad150-130">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad150-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad150-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad150-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad150-132">Request</span></span>
<span data-ttu-id="ad150-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad150-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ad150-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad150-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/childFolders
Content-type: application/json
Content-length: 84

{
  "displayName": "displayName-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ad150-135">C#</span><span class="sxs-lookup"><span data-stu-id="ad150-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contactfolder-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad150-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="ad150-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contactfolder-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ad150-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ad150-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contactfolder-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="ad150-138">No corpo da solicitação, forneça uma representação JSON do objeto [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="ad150-138">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ad150-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad150-139">Response</span></span>
<span data-ttu-id="ad150-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad150-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
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
