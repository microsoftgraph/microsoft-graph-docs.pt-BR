---
title: Atualizar identityProvider
description: Atualize as propriedades em um identityprovider existente.
localization_priority: Normal
doc_type: apiPageType
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1925e71e365d6a5f632176c62afc43ee30e829ee
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199568"
---
# <a name="update-identityprovider"></a><span data-ttu-id="964cc-103">Atualizar identityProvider</span><span class="sxs-lookup"><span data-stu-id="964cc-103">Update identityProvider</span></span>

<span data-ttu-id="964cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="964cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="964cc-105">Atualizar as propriedades em um [identityProvider](../resources/identityprovider.md) existente.</span><span class="sxs-lookup"><span data-stu-id="964cc-105">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="964cc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="964cc-106">Permissions</span></span>

<span data-ttu-id="964cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="964cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="964cc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="964cc-109">Permission type</span></span>      | <span data-ttu-id="964cc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="964cc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="964cc-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="964cc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="964cc-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="964cc-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="964cc-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="964cc-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="964cc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="964cc-114">Not supported.</span></span>|
|<span data-ttu-id="964cc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="964cc-115">Application</span></span>| <span data-ttu-id="964cc-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="964cc-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="964cc-117">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="964cc-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="964cc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="964cc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="964cc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="964cc-119">Request headers</span></span>

|<span data-ttu-id="964cc-120">Nome</span><span class="sxs-lookup"><span data-stu-id="964cc-120">Name</span></span>|<span data-ttu-id="964cc-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="964cc-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="964cc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="964cc-122">Authorization</span></span>|<span data-ttu-id="964cc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="964cc-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="964cc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="964cc-125">Content-Type</span></span>|<span data-ttu-id="964cc-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="964cc-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="964cc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="964cc-128">Request body</span></span>

<span data-ttu-id="964cc-129">No corpo da solicitação, fornece um objeto JSON com uma ou mais propriedades que precisam ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="964cc-129">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="964cc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="964cc-130">Property</span></span>|<span data-ttu-id="964cc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="964cc-131">Type</span></span>|<span data-ttu-id="964cc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="964cc-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="964cc-133">clientId</span><span class="sxs-lookup"><span data-stu-id="964cc-133">clientId</span></span>|<span data-ttu-id="964cc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="964cc-134">String</span></span>|<span data-ttu-id="964cc-135">O ID do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="964cc-135">The client ID for the application.</span></span> <span data-ttu-id="964cc-136">Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="964cc-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="964cc-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="964cc-137">clientSecret</span></span>|<span data-ttu-id="964cc-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="964cc-138">String</span></span>|<span data-ttu-id="964cc-139">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="964cc-139">The client secret for the application.</span></span> <span data-ttu-id="964cc-140">Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="964cc-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="964cc-141">nome</span><span class="sxs-lookup"><span data-stu-id="964cc-141">name</span></span>|<span data-ttu-id="964cc-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="964cc-142">String</span></span>|<span data-ttu-id="964cc-143">O nome exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="964cc-143">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="964cc-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="964cc-144">Response</span></span>

<span data-ttu-id="964cc-145">Quando é bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="964cc-145">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="964cc-146">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="964cc-146">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="964cc-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="964cc-147">Example</span></span>

<span data-ttu-id="964cc-148">O exemplo a seguir atualiza a definição da vida útil do token **identityProvider** e define como o padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="964cc-148">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="964cc-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="964cc-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="964cc-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="964cc-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="964cc-151">C#</span><span class="sxs-lookup"><span data-stu-id="964cc-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="964cc-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="964cc-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="964cc-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="964cc-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="964cc-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="964cc-154">Response</span></span>

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
