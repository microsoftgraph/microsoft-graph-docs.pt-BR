---
title: Obter identityUserFlowAttribute
description: Recupere as propriedades e os relacionamentos de um objeto identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: be05476a136a8a9512a102d11c516603f42aaaa7
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903899"
---
# <a name="get-identityuserflowattribute"></a><span data-ttu-id="c659b-103">Obter identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="c659b-103">Get identityUserFlowAttribute</span></span>

<span data-ttu-id="c659b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c659b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c659b-105">Recupere as propriedades e os relacionamentos de um objeto [identityUserFlowAttribute](../resources/identityuserflowattribute.md) .</span><span class="sxs-lookup"><span data-stu-id="c659b-105">Retrieve the properties and relationships of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c659b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c659b-106">Permissions</span></span>

<span data-ttu-id="c659b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c659b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c659b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c659b-109">Permission type</span></span>      | <span data-ttu-id="c659b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c659b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c659b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c659b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c659b-112">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c659b-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c659b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c659b-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c659b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c659b-114">Not supported.</span></span>|
|<span data-ttu-id="c659b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c659b-115">Application</span></span>|<span data-ttu-id="c659b-116">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c659b-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="c659b-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="c659b-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c659b-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c659b-118">Global administrator</span></span>
* <span data-ttu-id="c659b-119">Administrador do atributo de fluxo do usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="c659b-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c659b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c659b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c659b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c659b-121">Request headers</span></span>

|<span data-ttu-id="c659b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c659b-122">Name</span></span>|<span data-ttu-id="c659b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c659b-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c659b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c659b-124">Authorization</span></span>|<span data-ttu-id="c659b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c659b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c659b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c659b-127">Request body</span></span>

<span data-ttu-id="c659b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c659b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c659b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c659b-129">Response</span></span>

<span data-ttu-id="c659b-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma representação JSON do [identityUserFlowAttribute](../resources/identityuserflowattribute.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c659b-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityUserFlowAttribute](../resources/identityuserflowattribute.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c659b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c659b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c659b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c659b-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c659b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c659b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/userFlowAttributes/{id}
```
# <a name="c"></a>[<span data-ttu-id="c659b-134">C#</span><span class="sxs-lookup"><span data-stu-id="c659b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c659b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c659b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c659b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c659b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c659b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c659b-137">Response</span></span>

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
