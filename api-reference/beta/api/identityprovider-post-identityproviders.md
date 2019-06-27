---
title: Criar identityProvider
description: Criar um novo identityProvider especificando o nome de exibição, tipo de identityProvider, ID do cliente e o segredo do cliente.
localization_priority: Normal
ms.openlocfilehash: 97a87d73090457a2e314a8b44903260b24e55a69
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262668"
---
# <a name="create-identityprovider"></a><span data-ttu-id="b2f85-103">Criar identityProvider</span><span class="sxs-lookup"><span data-stu-id="b2f85-103">Create identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2f85-104">Criar um novo [identityProvider](../resources/identityprovider.md) especificando o nome de exibição, tipo de identityProvider, ID do cliente e o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="b2f85-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2f85-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b2f85-105">Permissions</span></span>

<span data-ttu-id="b2f85-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2f85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2f85-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2f85-108">Permission type</span></span>      | <span data-ttu-id="b2f85-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2f85-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2f85-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2f85-110">Delegated (work or school account)</span></span>|<span data-ttu-id="b2f85-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2f85-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="b2f85-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2f85-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b2f85-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2f85-113">Not supported.</span></span>|
|<span data-ttu-id="b2f85-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2f85-114">Application</span></span>|<span data-ttu-id="b2f85-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2f85-115">Not supported.</span></span>|

<span data-ttu-id="b2f85-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="b2f85-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="b2f85-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2f85-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="b2f85-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2f85-118">Request headers</span></span>

|<span data-ttu-id="b2f85-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b2f85-119">Name</span></span>|<span data-ttu-id="b2f85-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2f85-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b2f85-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2f85-121">Authorization</span></span>|<span data-ttu-id="b2f85-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2f85-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b2f85-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b2f85-124">Content-Type</span></span>|<span data-ttu-id="b2f85-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2f85-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2f85-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2f85-127">Request body</span></span>

<span data-ttu-id="b2f85-128">No corpo da solicitação, forneça uma representação JSON do objeto [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="b2f85-128">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="b2f85-129">Todas as propriedades listadas na tabela a seguir são necessárias.</span><span class="sxs-lookup"><span data-stu-id="b2f85-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="b2f85-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2f85-130">Property</span></span>|<span data-ttu-id="b2f85-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2f85-131">Type</span></span>|<span data-ttu-id="b2f85-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2f85-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2f85-133">clientId</span><span class="sxs-lookup"><span data-stu-id="b2f85-133">clientId</span></span>|<span data-ttu-id="b2f85-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2f85-134">String</span></span>|<span data-ttu-id="b2f85-135">O ID do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b2f85-135">The client ID for the application.</span></span> <span data-ttu-id="b2f85-136">Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="b2f85-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="b2f85-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="b2f85-137">clientSecret</span></span>|<span data-ttu-id="b2f85-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2f85-138">String</span></span>|<span data-ttu-id="b2f85-139">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b2f85-139">The client secret for the application.</span></span> <span data-ttu-id="b2f85-140">Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="b2f85-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="b2f85-141">nome</span><span class="sxs-lookup"><span data-stu-id="b2f85-141">name</span></span>|<span data-ttu-id="b2f85-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2f85-142">String</span></span>|<span data-ttu-id="b2f85-143">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="b2f85-143">The display name of the identity provider.</span></span>|
|<span data-ttu-id="b2f85-144">tipo</span><span class="sxs-lookup"><span data-stu-id="b2f85-144">type</span></span>|<span data-ttu-id="b2f85-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2f85-145">String</span></span>|<span data-ttu-id="b2f85-146">A identidade do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="b2f85-146">The identity provider type.</span></span> <span data-ttu-id="b2f85-147">Deve ser um dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="b2f85-147">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="b2f85-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="b2f85-148">Microsoft</span></span><li/><span data-ttu-id="b2f85-149">Google</span><span class="sxs-lookup"><span data-stu-id="b2f85-149">Google</span></span><li/><span data-ttu-id="b2f85-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="b2f85-150">Amazon</span></span><li/><span data-ttu-id="b2f85-151">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="b2f85-151">LinkedIn</span></span><li/><span data-ttu-id="b2f85-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="b2f85-152">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="b2f85-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2f85-153">Response</span></span>

<span data-ttu-id="b2f85-154">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [identityProvider](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2f85-154">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="b2f85-155">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="b2f85-155">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="b2f85-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2f85-156">Example</span></span>

<span data-ttu-id="b2f85-157">O exemplo a seguir cria um **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="b2f85-157">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="b2f85-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2f85-158">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="b2f85-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2f85-159">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b2f85-160">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="b2f85-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b2f85-161">C#</span><span class="sxs-lookup"><span data-stu-id="b2f85-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_identityprovider_from_identityproviders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b2f85-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="b2f85-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_identityprovider_from_identityproviders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b2f85-163">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b2f85-163">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_identityprovider_from_identityproviders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
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
    "Error: /api-reference/beta/api/identityprovider-post-identityproviders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/identityprovider-post-identityproviders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/identityprovider-post-identityproviders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
