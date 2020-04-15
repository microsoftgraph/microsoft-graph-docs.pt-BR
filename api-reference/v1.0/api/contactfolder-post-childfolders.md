---
title: Criar ContactFolder
description: 'Cria uma nova contactFolder como um filho de uma pasta especificada. '
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f3acdfc18b0727704c94ed84741a3413734ab90f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474698"
---
# <a name="create-contactfolder"></a><span data-ttu-id="1d8f5-103">Criar ContactFolder</span><span class="sxs-lookup"><span data-stu-id="1d8f5-103">Create ContactFolder</span></span>

<span data-ttu-id="1d8f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d8f5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d8f5-105">Cria uma nova contactFolder como um filho de uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="1d8f5-105">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="1d8f5-106">Também é possível [criar uma nova contactFolder sob a pasta de contatos padrão do usuário](user-post-contactfolders.md).</span><span class="sxs-lookup"><span data-stu-id="1d8f5-106">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="1d8f5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d8f5-107">Permissions</span></span>
<span data-ttu-id="1d8f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d8f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d8f5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d8f5-110">Permission type</span></span>      | <span data-ttu-id="1d8f5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d8f5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d8f5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d8f5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1d8f5-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d8f5-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1d8f5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d8f5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d8f5-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d8f5-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1d8f5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d8f5-116">Application</span></span> | <span data-ttu-id="1d8f5-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d8f5-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d8f5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d8f5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="1d8f5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d8f5-119">Request headers</span></span>
| <span data-ttu-id="1d8f5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d8f5-120">Header</span></span>       | <span data-ttu-id="1d8f5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1d8f5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1d8f5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d8f5-122">Authorization</span></span>  | <span data-ttu-id="1d8f5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d8f5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1d8f5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d8f5-125">Content-Type</span></span>  | <span data-ttu-id="1d8f5-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d8f5-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1d8f5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d8f5-128">Request body</span></span>
<span data-ttu-id="1d8f5-129">No corpo da solicitação, forneça uma representação JSON do objeto [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="1d8f5-129">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1d8f5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d8f5-130">Response</span></span>

<span data-ttu-id="1d8f5-131">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d8f5-131">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d8f5-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d8f5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d8f5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d8f5-133">Request</span></span>
<span data-ttu-id="1d8f5-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d8f5-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1d8f5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d8f5-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1d8f5-136">C#</span><span class="sxs-lookup"><span data-stu-id="1d8f5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contactfolder-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d8f5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d8f5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contactfolder-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d8f5-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d8f5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contactfolder-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1d8f5-139">Java</span><span class="sxs-lookup"><span data-stu-id="1d8f5-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contactfolder-from-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1d8f5-140">No corpo da solicitação, forneça uma representação JSON do objeto [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="1d8f5-140">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1d8f5-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d8f5-141">Response</span></span>
<span data-ttu-id="1d8f5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d8f5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
