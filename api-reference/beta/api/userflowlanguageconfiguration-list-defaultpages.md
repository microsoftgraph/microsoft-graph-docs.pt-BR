---
title: Listar defaultPages
description: Obter os recursos userFlowLanguagePage da propriedade de navegação defaultPages.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 58cffebabba13553f18c8bb5b7b45845bdd1fe64
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547096"
---
# <a name="list-defaultpages"></a><span data-ttu-id="1e3ce-103">Listar defaultPages</span><span class="sxs-lookup"><span data-stu-id="1e3ce-103">List defaultPages</span></span>

<span data-ttu-id="1e3ce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e3ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e3ce-105">Obter os recursos userFlowLanguagePage da propriedade de navegação defaultPages.</span><span class="sxs-lookup"><span data-stu-id="1e3ce-105">Get the userFlowLanguagePage resources from the defaultPages navigation property.</span></span> <span data-ttu-id="1e3ce-106">Eles contêm os valores mostrados para o usuário em uma jornada de usuário padrão de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="1e3ce-106">These contain the values shown to the user in a default user journey of a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e3ce-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e3ce-107">Permissions</span></span>

<span data-ttu-id="1e3ce-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e3ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e3ce-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e3ce-110">Permission type</span></span>      | <span data-ttu-id="1e3ce-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e3ce-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e3ce-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e3ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e3ce-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e3ce-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="1e3ce-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e3ce-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="1e3ce-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e3ce-115">Not supported.</span></span>|
|<span data-ttu-id="1e3ce-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e3ce-116">Application</span></span>|<span data-ttu-id="1e3ce-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e3ce-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="1e3ce-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="1e3ce-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="1e3ce-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1e3ce-119">Global administrator</span></span>
* <span data-ttu-id="1e3ce-120">Administrador de identidade externa Flow usuário</span><span class="sxs-lookup"><span data-stu-id="1e3ce-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="1e3ce-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e3ce-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/languages/{id}/defaultPages
GET /identity/b2xUserFlows/{id}/languages/{id}/defaultPages
```

## <a name="request-headers"></a><span data-ttu-id="1e3ce-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e3ce-122">Request headers</span></span>

|<span data-ttu-id="1e3ce-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1e3ce-123">Name</span></span>|<span data-ttu-id="1e3ce-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e3ce-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1e3ce-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e3ce-125">Authorization</span></span>|<span data-ttu-id="1e3ce-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e3ce-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e3ce-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e3ce-128">Request body</span></span>

<span data-ttu-id="1e3ce-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1e3ce-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e3ce-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e3ce-130">Response</span></span>

<span data-ttu-id="1e3ce-131">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos userFlowLanguagePage](../resources/userflowlanguagepage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e3ce-131">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguagePage](../resources/userflowlanguagepage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1e3ce-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1e3ce-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1e3ce-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e3ce-133">Request</span></span>

<span data-ttu-id="1e3ce-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e3ce-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1e3ce-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e3ce-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguagepage_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en/defaultPages
```
# <a name="c"></a>[<span data-ttu-id="1e3ce-136">C#</span><span class="sxs-lookup"><span data-stu-id="1e3ce-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguagepage-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1e3ce-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e3ce-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguagepage-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1e3ce-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1e3ce-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguagepage-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1e3ce-139">Java</span><span class="sxs-lookup"><span data-stu-id="1e3ce-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguagepage-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1e3ce-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e3ce-140">Response</span></span>

<span data-ttu-id="1e3ce-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1e3ce-141">The following is an example of the response.</span></span>

<span data-ttu-id="1e3ce-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1e3ce-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguagePage)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "idpselections"
    },
    {
      "id": "phonefactor"
    }
  ]
}
```
