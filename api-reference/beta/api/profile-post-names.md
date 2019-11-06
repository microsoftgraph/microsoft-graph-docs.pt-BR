---
title: Criar PersonName
description: Use esta API para criar um novo PersonName no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: fd2937004a38326ad934d4e7c32e5d3009021154
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997781"
---
# <a name="create-personname"></a><span data-ttu-id="a8211-103">Criar PersonName</span><span class="sxs-lookup"><span data-stu-id="a8211-103">Create personName</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8211-104">Use esta API para criar um novo objeto [PersonName](../resources/personname.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a8211-104">Use this API to create a new [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a8211-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8211-105">Permissions</span></span>

<span data-ttu-id="a8211-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8211-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a8211-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8211-108">Permission type</span></span>                        | <span data-ttu-id="a8211-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8211-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="a8211-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8211-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8211-111">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a8211-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a8211-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8211-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8211-113">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a8211-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a8211-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8211-114">Application</span></span>                            | <span data-ttu-id="a8211-115">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a8211-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8211-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8211-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/names
```

## <a name="request-headers"></a><span data-ttu-id="a8211-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8211-117">Request headers</span></span>

| <span data-ttu-id="a8211-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a8211-118">Name</span></span>           |<span data-ttu-id="a8211-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8211-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="a8211-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8211-120">Authorization</span></span>  | <span data-ttu-id="a8211-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8211-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="a8211-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a8211-123">Content-Type</span></span>   | <span data-ttu-id="a8211-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8211-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8211-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8211-126">Request body</span></span>

<span data-ttu-id="a8211-127">No corpo da solicitação, forneça uma representação JSON do objeto [PersonName](../resources/personname.md) .</span><span class="sxs-lookup"><span data-stu-id="a8211-127">In the request body, supply a JSON representation of [personName](../resources/personname.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a8211-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8211-128">Response</span></span>

<span data-ttu-id="a8211-129">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [PersonName](../resources/personname.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8211-129">If successful, this method returns `201, Created` response code and a new [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a8211-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a8211-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a8211-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8211-131">Request</span></span>

<span data-ttu-id="a8211-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8211-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a8211-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8211-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personname_from_profilev2"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/names
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a8211-134">C#</span><span class="sxs-lookup"><span data-stu-id="a8211-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personname-from-profilev2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8211-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8211-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personname-from-profilev2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a8211-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8211-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personname-from-profilev2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a8211-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8211-137">Response</span></span>

<span data-ttu-id="a8211-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a8211-138">The following is an example of the response.</span></span>

> <span data-ttu-id="a8211-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8211-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create personName",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
