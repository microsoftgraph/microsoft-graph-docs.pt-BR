---
title: Obter identityUserFlowAttribute
description: Recupere as propriedades e as relações de um objeto identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: f98dc9a69aee1297d26ef4ed9891f9035a297ced
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435263"
---
# <a name="get-identityuserflowattribute"></a><span data-ttu-id="a196f-103">Obter identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="a196f-103">Get identityUserFlowAttribute</span></span>

<span data-ttu-id="a196f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a196f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a196f-105">Recupere as propriedades e as relações de [um objeto identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="a196f-105">Retrieve the properties and relationships of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a196f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a196f-106">Permissions</span></span>

<span data-ttu-id="a196f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a196f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a196f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a196f-109">Permission type</span></span>      | <span data-ttu-id="a196f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a196f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a196f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a196f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a196f-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a196f-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="a196f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a196f-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="a196f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a196f-114">Not supported.</span></span>|
|<span data-ttu-id="a196f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a196f-115">Application</span></span>|<span data-ttu-id="a196f-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a196f-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="a196f-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="a196f-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="a196f-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="a196f-118">Global administrator</span></span>
* <span data-ttu-id="a196f-119">Administrador de Atributo de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="a196f-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="a196f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a196f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a196f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a196f-121">Request headers</span></span>

|<span data-ttu-id="a196f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a196f-122">Name</span></span>|<span data-ttu-id="a196f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a196f-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="a196f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a196f-124">Authorization</span></span>|<span data-ttu-id="a196f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a196f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a196f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a196f-127">Request body</span></span>

<span data-ttu-id="a196f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a196f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a196f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a196f-129">Response</span></span>

<span data-ttu-id="a196f-130">Se tiver êxito, este método retornará um código de resposta e uma representação JSON da `200 OK` [identidadeUserFlowAttribute](../resources/identityuserflowattribute.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a196f-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityUserFlowAttribute](../resources/identityuserflowattribute.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a196f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a196f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a196f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a196f-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a196f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a196f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/userFlowAttributes/{id}
```
# <a name="c"></a>[<span data-ttu-id="a196f-134">C#</span><span class="sxs-lookup"><span data-stu-id="a196f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a196f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a196f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a196f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a196f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a196f-137">Java</span><span class="sxs-lookup"><span data-stu-id="a196f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a196f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a196f-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "City",
    "displayName": "City",
    "description": "Your city",
    "userFlowAttributeType": "builtIn",
    "dataType": "string"
}
```
