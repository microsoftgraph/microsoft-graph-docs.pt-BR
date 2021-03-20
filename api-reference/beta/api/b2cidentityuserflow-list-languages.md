---
title: Idiomas da lista
description: Recupere uma lista de idiomas com suporte para personalização em um fluxo de usuários B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2f29a8d5c87c73c5a42c0cc71775a8e0dc893cec
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944779"
---
# <a name="list-languages"></a><span data-ttu-id="79629-103">Idiomas da lista</span><span class="sxs-lookup"><span data-stu-id="79629-103">List languages</span></span>

<span data-ttu-id="79629-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79629-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="79629-105">Recupere uma lista de idiomas com suporte para personalização em um fluxo de usuários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="79629-105">Retrieve a list of languages supported for customization in an Azure AD B2C user flow.</span></span>

<span data-ttu-id="79629-106">**Observação:** Para recuperar uma lista de idiomas com suporte para personalização, você deve primeiro habilitar a personalização de idioma no fluxo de usuários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="79629-106">**Note:** To retrieve a list of languages supported for customization, you must first enable language customization on your Azure AD B2C user flow.</span></span> <span data-ttu-id="79629-107">Para obter mais informações, [consulte Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span><span class="sxs-lookup"><span data-stu-id="79629-107">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="79629-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="79629-108">Permissions</span></span>

<span data-ttu-id="79629-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79629-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79629-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79629-111">Permission type</span></span>      | <span data-ttu-id="79629-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79629-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79629-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79629-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79629-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79629-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="79629-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79629-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="79629-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79629-116">Not supported.</span></span>|
|<span data-ttu-id="79629-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79629-117">Application</span></span>|<span data-ttu-id="79629-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79629-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="79629-119">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="79629-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="79629-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="79629-120">Global administrator</span></span>
* <span data-ttu-id="79629-121">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="79629-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="79629-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79629-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/languages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79629-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="79629-123">Optional query parameters</span></span>

<span data-ttu-id="79629-124">Este método dá suporte `$filter` ao parâmetro de consulta para mostrar apenas os idiomas habilitados.</span><span class="sxs-lookup"><span data-stu-id="79629-124">This method supports the `$filter` query parameter to show only the enabled languages.</span></span> <span data-ttu-id="79629-125">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="79629-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="79629-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79629-126">Request headers</span></span>

|<span data-ttu-id="79629-127">Nome</span><span class="sxs-lookup"><span data-stu-id="79629-127">Name</span></span>|<span data-ttu-id="79629-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="79629-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="79629-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="79629-129">Authorization</span></span>|<span data-ttu-id="79629-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79629-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79629-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79629-132">Request body</span></span>

<span data-ttu-id="79629-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79629-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79629-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="79629-134">Response</span></span>

<span data-ttu-id="79629-135">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79629-135">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79629-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="79629-136">Examples</span></span>

### <a name="example-1-retrieve-a-list-of-all-languages"></a><span data-ttu-id="79629-137">Exemplo 1: Recuperar uma lista de todos os idiomas</span><span class="sxs-lookup"><span data-stu-id="79629-137">Example 1: Retrieve a list of all languages</span></span>

#### <a name="request"></a><span data-ttu-id="79629-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79629-138">Request</span></span>

<span data-ttu-id="79629-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="79629-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="79629-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="79629-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages
```
# <a name="c"></a>[<span data-ttu-id="79629-141">C#</span><span class="sxs-lookup"><span data-stu-id="79629-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79629-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79629-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79629-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79629-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79629-144">Java</span><span class="sxs-lookup"><span data-stu-id="79629-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="79629-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="79629-145">Response</span></span>

<span data-ttu-id="79629-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79629-146">The following is an example of the response.</span></span>

<span data-ttu-id="79629-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="79629-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_CustomerSignUp')/languages",
  "value": [
    {
      "id": "en",
      "isEnabled": true,
      "displayName": "English"
    },
    {
      "id": "de",
      "isEnabled": false,
      "displayName": "Deutsch"
    }
  ]
}
```

### <a name="example-2-retrieve-a-list-of-only-enabled-languages"></a><span data-ttu-id="79629-148">Exemplo 2: Recuperar uma lista de idiomas habilitados somente</span><span class="sxs-lookup"><span data-stu-id="79629-148">Example 2: Retrieve a list of only enabled languages</span></span>

#### <a name="request"></a><span data-ttu-id="79629-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79629-149">Request</span></span>

<span data-ttu-id="79629-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="79629-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="79629-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="79629-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_filter"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages?$filter=isEnabled eq true
```
# <a name="c"></a>[<span data-ttu-id="79629-152">C#</span><span class="sxs-lookup"><span data-stu-id="79629-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79629-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79629-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79629-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79629-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79629-155">Java</span><span class="sxs-lookup"><span data-stu-id="79629-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="79629-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="79629-156">Response</span></span>

<span data-ttu-id="79629-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79629-157">The following is an example of the response.</span></span>

<span data-ttu-id="79629-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="79629-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_CustomerSignUp')/languages",
  "value": [
    {
      "id": "en",
      "isEnabled": true,
      "displayName": "English"
    }
  ]
}
```
