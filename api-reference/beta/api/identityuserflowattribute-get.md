---
title: Obter identityUserFlowAttribute
description: Recupere as propriedades e os relacionamentos de um objeto identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2497ac509376aa07b692ac8d137e64b5c299ab49
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953170"
---
# <a name="get-identityuserflowattribute"></a><span data-ttu-id="f0fb5-103">Obter identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="f0fb5-103">Get identityUserFlowAttribute</span></span>

<span data-ttu-id="f0fb5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0fb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0fb5-105">Recupere as propriedades e os relacionamentos de um objeto [identityUserFlowAttribute](../resources/identityuserflowattribute.md) .</span><span class="sxs-lookup"><span data-stu-id="f0fb5-105">Retrieve the properties and relationships of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0fb5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0fb5-106">Permissions</span></span>

<span data-ttu-id="f0fb5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0fb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0fb5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0fb5-109">Permission type</span></span>      | <span data-ttu-id="f0fb5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0fb5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0fb5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0fb5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f0fb5-112">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f0fb5-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="f0fb5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0fb5-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f0fb5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0fb5-114">Not supported.</span></span>|
|<span data-ttu-id="f0fb5-115">Application</span><span class="sxs-lookup"><span data-stu-id="f0fb5-115">Application</span></span>|<span data-ttu-id="f0fb5-116">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f0fb5-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="f0fb5-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="f0fb5-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f0fb5-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="f0fb5-118">Global administrator</span></span>
* <span data-ttu-id="f0fb5-119">Administrador do atributo de fluxo do usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="f0fb5-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f0fb5-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0fb5-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f0fb5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0fb5-121">Request headers</span></span>

|<span data-ttu-id="f0fb5-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f0fb5-122">Name</span></span>|<span data-ttu-id="f0fb5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0fb5-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f0fb5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0fb5-124">Authorization</span></span>|<span data-ttu-id="f0fb5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0fb5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0fb5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0fb5-127">Request body</span></span>

<span data-ttu-id="f0fb5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f0fb5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0fb5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0fb5-129">Response</span></span>

<span data-ttu-id="f0fb5-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma representação JSON do [identityUserFlowAttribute](../resources/identityuserflowattribute.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0fb5-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityUserFlowAttribute](../resources/identityuserflowattribute.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f0fb5-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f0fb5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f0fb5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0fb5-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f0fb5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0fb5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/userFlowAttributes/{id}
```
# <a name="c"></a>[<span data-ttu-id="f0fb5-134">C#</span><span class="sxs-lookup"><span data-stu-id="f0fb5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0fb5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0fb5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0fb5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0fb5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0fb5-137">Java</span><span class="sxs-lookup"><span data-stu-id="f0fb5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f0fb5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0fb5-138">Response</span></span>

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
