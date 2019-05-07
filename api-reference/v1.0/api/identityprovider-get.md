---
title: Obter identityProvider
description: Recuperar as propriedades de um identityProvider existente
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a666f9f578ab945c268646f898ec107194fb8016
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613388"
---
# <a name="get-identityprovider"></a><span data-ttu-id="e6733-103">Obter identityProvider</span><span class="sxs-lookup"><span data-stu-id="e6733-103">Get identityProvider</span></span>

<span data-ttu-id="e6733-104">Recuperar as propriedades de um [identityProvider](../resources/identityprovider.md) existente.</span><span class="sxs-lookup"><span data-stu-id="e6733-104">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e6733-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6733-105">Permissions</span></span>

<span data-ttu-id="e6733-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6733-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6733-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6733-108">Permission type</span></span>      | <span data-ttu-id="e6733-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6733-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6733-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6733-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e6733-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6733-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="e6733-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6733-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e6733-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6733-113">Not supported.</span></span>|
|<span data-ttu-id="e6733-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6733-114">Application</span></span>|<span data-ttu-id="e6733-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6733-115">Not supported.</span></span>|

<span data-ttu-id="e6733-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="e6733-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="e6733-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6733-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e6733-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6733-118">Request headers</span></span>

|<span data-ttu-id="e6733-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e6733-119">Name</span></span>|<span data-ttu-id="e6733-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6733-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e6733-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6733-121">Authorization</span></span>|<span data-ttu-id="e6733-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6733-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6733-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6733-124">Request body</span></span>

<span data-ttu-id="e6733-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e6733-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6733-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6733-126">Response</span></span>

<span data-ttu-id="e6733-127">Se bem-sucedido, esse método retornará `200 OK` código de resposta e uma representação JSON do [identityProvider](../resources/identityProvider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6733-127">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityProvider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6733-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6733-128">Example</span></span>

<span data-ttu-id="e6733-129">O exemplo a seguir recupera uma determinada **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="e6733-129">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="e6733-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6733-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-identityprovider"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="e6733-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6733-131">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e6733-132">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="e6733-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e6733-133">C#</span><span class="sxs-lookup"><span data-stu-id="e6733-133">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-identityprovider-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e6733-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="e6733-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-identityprovider-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/identityprovider-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/identityprovider-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
