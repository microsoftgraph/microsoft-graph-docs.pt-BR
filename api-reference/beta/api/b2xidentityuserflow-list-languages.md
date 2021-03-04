---
title: Idiomas da lista
description: Recupere uma lista de idiomas com suporte para personalização em um fluxo de usuário B2X.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b6f629f8abe4691e0f8f688e4640d2b56f0dce27
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438075"
---
# <a name="list-languages"></a><span data-ttu-id="fe1e4-103">Idiomas da lista</span><span class="sxs-lookup"><span data-stu-id="fe1e4-103">List languages</span></span>

<span data-ttu-id="fe1e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe1e4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe1e4-105">Recupere uma lista de idiomas com suporte para personalização em um fluxo de usuários B2X.</span><span class="sxs-lookup"><span data-stu-id="fe1e4-105">Retrieve a list of languages supported for customization in a B2X user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe1e4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe1e4-106">Permissions</span></span>

<span data-ttu-id="fe1e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe1e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe1e4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe1e4-109">Permission type</span></span>      | <span data-ttu-id="fe1e4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe1e4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe1e4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe1e4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fe1e4-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe1e4-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="fe1e4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe1e4-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="fe1e4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe1e4-114">Not supported.</span></span>|
|<span data-ttu-id="fe1e4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe1e4-115">Application</span></span>|<span data-ttu-id="fe1e4-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe1e4-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="fe1e4-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="fe1e4-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="fe1e4-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="fe1e4-118">Global administrator</span></span>
* <span data-ttu-id="fe1e4-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="fe1e4-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="fe1e4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe1e4-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/languages
```

## <a name="request-headers"></a><span data-ttu-id="fe1e4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe1e4-121">Request headers</span></span>

|<span data-ttu-id="fe1e4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fe1e4-122">Name</span></span>|<span data-ttu-id="fe1e4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe1e4-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fe1e4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe1e4-124">Authorization</span></span>|<span data-ttu-id="fe1e4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe1e4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe1e4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe1e4-127">Request body</span></span>

<span data-ttu-id="fe1e4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe1e4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe1e4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe1e4-129">Response</span></span>

<span data-ttu-id="fe1e4-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe1e4-130">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fe1e4-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fe1e4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fe1e4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe1e4-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fe1e4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe1e4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_PartnerSignUp/languages
```
# <a name="c"></a>[<span data-ttu-id="fe1e4-134">C#</span><span class="sxs-lookup"><span data-stu-id="fe1e4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe1e4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe1e4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe1e4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe1e4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe1e4-137">Java</span><span class="sxs-lookup"><span data-stu-id="fe1e4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fe1e4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe1e4-138">Response</span></span>

<span data-ttu-id="fe1e4-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fe1e4-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguageConfiguration)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows('B2X_1_PartnerSignUp')/languages",
  "value": [
    {
      "id": "en",
      "isEnabled": true,
      "displayName": "English"
    },
    {
      "id": "de",
      "isEnabled": true,
      "displayName": "Deutsch"
    }
  ]
}
```
