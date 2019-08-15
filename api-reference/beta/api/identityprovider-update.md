---
title: Atualizar identityProvider
description: Atualize as propriedades em um identityprovider existente.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: c0b13dd9eece28a2910f1034a9a484d932a9c6a8
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420494"
---
# <a name="update-identityprovider"></a><span data-ttu-id="ecd3d-103">Atualizar identityProvider</span><span class="sxs-lookup"><span data-stu-id="ecd3d-103">Update identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecd3d-104">Atualizar as propriedades em um [identityProvider](../resources/identityprovider.md) existente.</span><span class="sxs-lookup"><span data-stu-id="ecd3d-104">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ecd3d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ecd3d-105">Permissions</span></span>

<span data-ttu-id="ecd3d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecd3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecd3d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ecd3d-108">Permission type</span></span>      | <span data-ttu-id="ecd3d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ecd3d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ecd3d-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ecd3d-110">Delegated (work or school account)</span></span>|<span data-ttu-id="ecd3d-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecd3d-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="ecd3d-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ecd3d-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ecd3d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecd3d-113">Not supported.</span></span>|
|<span data-ttu-id="ecd3d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ecd3d-114">Application</span></span>|<span data-ttu-id="ecd3d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecd3d-115">Not supported.</span></span>|

<span data-ttu-id="ecd3d-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="ecd3d-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="ecd3d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecd3d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ecd3d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ecd3d-118">Request headers</span></span>

|<span data-ttu-id="ecd3d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ecd3d-119">Name</span></span>|<span data-ttu-id="ecd3d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecd3d-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ecd3d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ecd3d-121">Authorization</span></span>|<span data-ttu-id="ecd3d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecd3d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ecd3d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ecd3d-124">Content-Type</span></span>|<span data-ttu-id="ecd3d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecd3d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecd3d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ecd3d-127">Request body</span></span>

<span data-ttu-id="ecd3d-128">No corpo da solicitação, fornece um objeto JSON com uma ou mais propriedades que precisam ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="ecd3d-128">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="ecd3d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ecd3d-129">Property</span></span>|<span data-ttu-id="ecd3d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecd3d-130">Type</span></span>|<span data-ttu-id="ecd3d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecd3d-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ecd3d-132">clientId</span><span class="sxs-lookup"><span data-stu-id="ecd3d-132">clientId</span></span>|<span data-ttu-id="ecd3d-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecd3d-133">String</span></span>|<span data-ttu-id="ecd3d-134">O ID do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ecd3d-134">The client ID for the application.</span></span> <span data-ttu-id="ecd3d-135">Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="ecd3d-135">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="ecd3d-136">clientSecret</span><span class="sxs-lookup"><span data-stu-id="ecd3d-136">clientSecret</span></span>|<span data-ttu-id="ecd3d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecd3d-137">String</span></span>|<span data-ttu-id="ecd3d-138">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ecd3d-138">The client secret for the application.</span></span> <span data-ttu-id="ecd3d-139">Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="ecd3d-139">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="ecd3d-140">nome</span><span class="sxs-lookup"><span data-stu-id="ecd3d-140">name</span></span>|<span data-ttu-id="ecd3d-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecd3d-141">String</span></span>|<span data-ttu-id="ecd3d-142">O nome exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="ecd3d-142">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="ecd3d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecd3d-143">Response</span></span>

<span data-ttu-id="ecd3d-144">Quando é bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ecd3d-144">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="ecd3d-145">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="ecd3d-145">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="ecd3d-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ecd3d-146">Example</span></span>

<span data-ttu-id="ecd3d-147">O exemplo a seguir atualiza a definição da vida útil do token **identityProvider** e define como o padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="ecd3d-147">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="ecd3d-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ecd3d-148">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ecd3d-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecd3d-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ecd3d-150">C#</span><span class="sxs-lookup"><span data-stu-id="ecd3d-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ecd3d-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecd3d-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ecd3d-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ecd3d-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ecd3d-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecd3d-153">Response</span></span>

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
