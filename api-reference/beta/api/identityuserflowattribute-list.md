---
title: Listar identityUserFlowAttributes
description: Recupere uma lista de objetos identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: af97b488cbc571c53363e088f6507d8c48593f42
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435249"
---
# <a name="list-identityuserflowattributes"></a><span data-ttu-id="d3a26-103">Listar identityUserFlowAttributes</span><span class="sxs-lookup"><span data-stu-id="d3a26-103">List identityUserFlowAttributes</span></span>

<span data-ttu-id="d3a26-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3a26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3a26-105">Recupere uma lista de [objetos identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="d3a26-105">Retrieve a list of [identityUserFlowAttribute](../resources/identityuserflowattribute.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3a26-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3a26-106">Permissions</span></span>

<span data-ttu-id="d3a26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3a26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3a26-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3a26-109">Permission type</span></span>      | <span data-ttu-id="d3a26-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3a26-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3a26-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3a26-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d3a26-112">IdentityUserFlow.Read.All, IdentityUserflow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3a26-112">IdentityUserFlow.Read.All, IdentityUserflow.ReadWrite.All</span></span>|
|<span data-ttu-id="d3a26-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3a26-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d3a26-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3a26-114">Not supported.</span></span>|
|<span data-ttu-id="d3a26-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3a26-115">Application</span></span>|<span data-ttu-id="d3a26-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3a26-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="d3a26-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="d3a26-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="d3a26-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d3a26-118">Global administrator</span></span>
* <span data-ttu-id="d3a26-119">Administrador de Atributo de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="d3a26-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="d3a26-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3a26-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes
```

## <a name="request-headers"></a><span data-ttu-id="d3a26-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3a26-121">Request headers</span></span>

|<span data-ttu-id="d3a26-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d3a26-122">Name</span></span>|<span data-ttu-id="d3a26-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3a26-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d3a26-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3a26-124">Authorization</span></span>|<span data-ttu-id="d3a26-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3a26-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3a26-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3a26-127">Request body</span></span>

<span data-ttu-id="d3a26-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3a26-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3a26-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3a26-129">Response</span></span>

<span data-ttu-id="d3a26-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos identityUserFlowAttribute](../resources/identityuserflowattribute.md)  no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3a26-130">If successful, this method returns a `200 OK` response code and a collection of [identityUserFlowAttribute](../resources/identityuserflowattribute.md)  objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3a26-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3a26-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3a26-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3a26-132">Request</span></span>

<span data-ttu-id="d3a26-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3a26-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d3a26-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3a26-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/userFlowAttributes
```
# <a name="c"></a>[<span data-ttu-id="d3a26-135">C#</span><span class="sxs-lookup"><span data-stu-id="d3a26-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3a26-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3a26-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3a26-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3a26-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3a26-138">Java</span><span class="sxs-lookup"><span data-stu-id="d3a26-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d3a26-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3a26-139">Response</span></span>

<span data-ttu-id="d3a26-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d3a26-140">The following is an example of the response.</span></span>

<span data-ttu-id="d3a26-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d3a26-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#userFlowAttributes",
    "value": [
      {
          "id": "City",
          "displayName": "City",
          "description": "Your city",
          "userFlowAttributeType": "builtIn",
          "dataType": "string"
      },
      {
          "id": "extension_d09380e2b4c6429a203fb816a04a7ad_Hobby",
          "displayName": "Hobby",
          "description": "Your hobby",
          "userFlowAttributeType": "custom",
          "dataType": "string",
      },
    ]
}
```
