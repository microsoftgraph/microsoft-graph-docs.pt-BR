---
title: Criar identityProvider
description: Criar um novo identityProvider especificando o nome de exibição, tipo de identityProvider, ID do cliente e o segredo do cliente.
localization_priority: Normal
doc_type: apiPageType
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 540af7a9ebb9ea56f6f3f61cff89ff6a4d3973d6
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199579"
---
# <a name="create-identityprovider"></a><span data-ttu-id="61771-103">Criar identityProvider</span><span class="sxs-lookup"><span data-stu-id="61771-103">Create identityProvider</span></span>

<span data-ttu-id="61771-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61771-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61771-105">Criar um novo [identityProvider](../resources/identityprovider.md) especificando o nome de exibição, tipo de identityProvider, ID do cliente e o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="61771-105">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="61771-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="61771-106">Permissions</span></span>

<span data-ttu-id="61771-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61771-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61771-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61771-109">Permission type</span></span>      | <span data-ttu-id="61771-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61771-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61771-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61771-111">Delegated (work or school account)</span></span>|<span data-ttu-id="61771-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61771-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="61771-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61771-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="61771-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61771-114">Not supported.</span></span>|
|<span data-ttu-id="61771-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61771-115">Application</span></span>|<span data-ttu-id="61771-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61771-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="61771-117">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="61771-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="61771-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61771-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="61771-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61771-119">Request headers</span></span>

|<span data-ttu-id="61771-120">Nome</span><span class="sxs-lookup"><span data-stu-id="61771-120">Name</span></span>|<span data-ttu-id="61771-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="61771-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="61771-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="61771-122">Authorization</span></span>|<span data-ttu-id="61771-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61771-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="61771-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="61771-125">Content-Type</span></span>|<span data-ttu-id="61771-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61771-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="61771-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61771-128">Request body</span></span>

<span data-ttu-id="61771-129">No corpo da solicitação, forneça uma representação JSON do objeto [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="61771-129">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="61771-130">Todas as propriedades listadas na tabela a seguir são necessárias.</span><span class="sxs-lookup"><span data-stu-id="61771-130">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="61771-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61771-131">Property</span></span>|<span data-ttu-id="61771-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="61771-132">Type</span></span>|<span data-ttu-id="61771-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="61771-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61771-134">clientId</span><span class="sxs-lookup"><span data-stu-id="61771-134">clientId</span></span>|<span data-ttu-id="61771-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61771-135">String</span></span>|<span data-ttu-id="61771-136">O ID do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="61771-136">The client ID for the application.</span></span> <span data-ttu-id="61771-137">Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="61771-137">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="61771-138">clientSecret</span><span class="sxs-lookup"><span data-stu-id="61771-138">clientSecret</span></span>|<span data-ttu-id="61771-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61771-139">String</span></span>|<span data-ttu-id="61771-140">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="61771-140">The client secret for the application.</span></span> <span data-ttu-id="61771-141">Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="61771-141">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="61771-142">nome</span><span class="sxs-lookup"><span data-stu-id="61771-142">name</span></span>|<span data-ttu-id="61771-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61771-143">String</span></span>|<span data-ttu-id="61771-144">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="61771-144">The display name of the identity provider.</span></span>|
|<span data-ttu-id="61771-145">tipo</span><span class="sxs-lookup"><span data-stu-id="61771-145">type</span></span>|<span data-ttu-id="61771-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61771-146">String</span></span>|<span data-ttu-id="61771-147">A identidade do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="61771-147">The identity provider type.</span></span> <span data-ttu-id="61771-148">Deve ser um dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="61771-148">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="61771-149">Microsoft</span><span class="sxs-lookup"><span data-stu-id="61771-149">Microsoft</span></span><li/><span data-ttu-id="61771-150">Google</span><span class="sxs-lookup"><span data-stu-id="61771-150">Google</span></span><li/><span data-ttu-id="61771-151">Amazon</span><span class="sxs-lookup"><span data-stu-id="61771-151">Amazon</span></span><li/><span data-ttu-id="61771-152">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="61771-152">LinkedIn</span></span><li/><span data-ttu-id="61771-153">Facebook</span><span class="sxs-lookup"><span data-stu-id="61771-153">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="61771-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="61771-154">Response</span></span>

<span data-ttu-id="61771-155">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [identityProvider](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61771-155">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="61771-156">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="61771-156">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="61771-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61771-157">Example</span></span>

<span data-ttu-id="61771-158">O exemplo a seguir cria um **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="61771-158">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="61771-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61771-159">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="61771-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="61771-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}-->
```http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json

{
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```
# <a name="c"></a>[<span data-ttu-id="61771-161">C#</span><span class="sxs-lookup"><span data-stu-id="61771-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61771-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61771-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61771-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61771-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="61771-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="61771-164">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
