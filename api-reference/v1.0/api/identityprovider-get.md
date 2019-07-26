---
title: Obter identityProvider
description: Recuperar as propriedades de um identityProvider existente
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 25b3e2733c3dcd9261f2b8ef59a4a98e96cfb401
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880912"
---
# <a name="get-identityprovider"></a><span data-ttu-id="c2567-103">Obter identityProvider</span><span class="sxs-lookup"><span data-stu-id="c2567-103">Get identityProvider</span></span>

<span data-ttu-id="c2567-104">Recuperar as propriedades de um [identityProvider](../resources/identityprovider.md) existente.</span><span class="sxs-lookup"><span data-stu-id="c2567-104">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2567-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2567-105">Permissions</span></span>

<span data-ttu-id="c2567-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2567-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2567-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2567-108">Permission type</span></span>      | <span data-ttu-id="c2567-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2567-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2567-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2567-110">Delegated (work or school account)</span></span>|<span data-ttu-id="c2567-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2567-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="c2567-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2567-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c2567-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2567-113">Not supported.</span></span>|
|<span data-ttu-id="c2567-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2567-114">Application</span></span>|<span data-ttu-id="c2567-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2567-115">Not supported.</span></span>|

<span data-ttu-id="c2567-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="c2567-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="c2567-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2567-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c2567-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2567-118">Request headers</span></span>

|<span data-ttu-id="c2567-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c2567-119">Name</span></span>|<span data-ttu-id="c2567-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2567-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c2567-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2567-121">Authorization</span></span>|<span data-ttu-id="c2567-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2567-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2567-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2567-124">Request body</span></span>

<span data-ttu-id="c2567-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2567-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2567-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2567-126">Response</span></span>

<span data-ttu-id="c2567-127">Se bem-sucedido, esse método retornará `200 OK` código de resposta e uma representação JSON do [identityProvider](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2567-127">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2567-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2567-128">Example</span></span>

<span data-ttu-id="c2567-129">O exemplo a seguir recupera uma determinada **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="c2567-129">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="c2567-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2567-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c2567-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2567-131">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-identityprovider"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2567-132">C#</span><span class="sxs-lookup"><span data-stu-id="c2567-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2567-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2567-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2567-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2567-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c2567-135">Java</span><span class="sxs-lookup"><span data-stu-id="c2567-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c2567-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2567-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "type": "Amazon",
    "name": "Login with Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
