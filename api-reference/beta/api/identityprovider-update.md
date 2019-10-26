---
title: Atualizar identityProvider
description: Atualize as propriedades em um identityprovider existente.
localization_priority: Normal
doc_type: apiPageType
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1cbbac43b7c47ee7aa160bf1e66a94e1afdb0c60
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734427"
---
# <a name="update-identityprovider"></a><span data-ttu-id="6cb6c-103">Atualizar identityProvider</span><span class="sxs-lookup"><span data-stu-id="6cb6c-103">Update identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cb6c-104">Atualizar as propriedades em um [identityProvider](../resources/identityprovider.md) existente.</span><span class="sxs-lookup"><span data-stu-id="6cb6c-104">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6cb6c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6cb6c-105">Permissions</span></span>

<span data-ttu-id="6cb6c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cb6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cb6c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cb6c-108">Permission type</span></span>      | <span data-ttu-id="6cb6c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6cb6c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cb6c-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cb6c-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6cb6c-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cb6c-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="6cb6c-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cb6c-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="6cb6c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cb6c-113">Not supported.</span></span>|
|<span data-ttu-id="6cb6c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cb6c-114">Application</span></span>| <span data-ttu-id="6cb6c-115">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cb6c-115">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="6cb6c-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="6cb6c-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="6cb6c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cb6c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6cb6c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cb6c-118">Request headers</span></span>

|<span data-ttu-id="6cb6c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6cb6c-119">Name</span></span>|<span data-ttu-id="6cb6c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cb6c-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="6cb6c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cb6c-121">Authorization</span></span>|<span data-ttu-id="6cb6c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cb6c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6cb6c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6cb6c-124">Content-Type</span></span>|<span data-ttu-id="6cb6c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cb6c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cb6c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cb6c-127">Request body</span></span>

<span data-ttu-id="6cb6c-128">No corpo da solicitação, fornece um objeto JSON com uma ou mais propriedades que precisam ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="6cb6c-128">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="6cb6c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6cb6c-129">Property</span></span>|<span data-ttu-id="6cb6c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cb6c-130">Type</span></span>|<span data-ttu-id="6cb6c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cb6c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cb6c-132">clientId</span><span class="sxs-lookup"><span data-stu-id="6cb6c-132">clientId</span></span>|<span data-ttu-id="6cb6c-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cb6c-133">String</span></span>|<span data-ttu-id="6cb6c-134">O ID do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cb6c-134">The client ID for the application.</span></span> <span data-ttu-id="6cb6c-135">Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="6cb6c-135">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="6cb6c-136">clientSecret</span><span class="sxs-lookup"><span data-stu-id="6cb6c-136">clientSecret</span></span>|<span data-ttu-id="6cb6c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cb6c-137">String</span></span>|<span data-ttu-id="6cb6c-138">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cb6c-138">The client secret for the application.</span></span> <span data-ttu-id="6cb6c-139">Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="6cb6c-139">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="6cb6c-140">nome</span><span class="sxs-lookup"><span data-stu-id="6cb6c-140">name</span></span>|<span data-ttu-id="6cb6c-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cb6c-141">String</span></span>|<span data-ttu-id="6cb6c-142">O nome exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="6cb6c-142">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="6cb6c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cb6c-143">Response</span></span>

<span data-ttu-id="6cb6c-144">Quando é bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6cb6c-144">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="6cb6c-145">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="6cb6c-145">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="6cb6c-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cb6c-146">Example</span></span>

<span data-ttu-id="6cb6c-147">O exemplo a seguir atualiza a definição da vida útil do token **identityProvider** e define como o padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="6cb6c-147">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="6cb6c-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cb6c-148">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6cb6c-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cb6c-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_identityprovider"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
    "clientSecret": "1111111111111"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6cb6c-150">C#</span><span class="sxs-lookup"><span data-stu-id="6cb6c-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6cb6c-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cb6c-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6cb6c-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cb6c-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6cb6c-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cb6c-153">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
