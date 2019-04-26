---
title: Criar identityProvider
description: Criar um novo identityProvider especificando o nome de exibição, tipo de identityProvider, ID do cliente e o segredo do cliente.
localization_priority: Normal
ms.openlocfilehash: 5d9940803ab9a140312c21f21832623eccd77969
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323836"
---
# <a name="create-identityprovider"></a><span data-ttu-id="5bf46-103">Criar identityProvider</span><span class="sxs-lookup"><span data-stu-id="5bf46-103">Create identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bf46-104">Criar um novo [identityProvider](../resources/identityprovider.md) especificando o nome de exibição, tipo de identityProvider, ID do cliente e o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="5bf46-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bf46-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5bf46-105">Permissions</span></span>

<span data-ttu-id="5bf46-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bf46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bf46-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5bf46-108">Permission type</span></span>      | <span data-ttu-id="5bf46-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5bf46-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bf46-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5bf46-110">Delegated (work or school account)</span></span>|<span data-ttu-id="5bf46-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bf46-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="5bf46-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5bf46-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="5bf46-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bf46-113">Not supported.</span></span>|
|<span data-ttu-id="5bf46-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bf46-114">Application</span></span>|<span data-ttu-id="5bf46-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bf46-115">Not supported.</span></span>|

<span data-ttu-id="5bf46-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="5bf46-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="5bf46-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5bf46-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="5bf46-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5bf46-118">Request headers</span></span>

|<span data-ttu-id="5bf46-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5bf46-119">Name</span></span>|<span data-ttu-id="5bf46-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bf46-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="5bf46-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5bf46-121">Authorization</span></span>|<span data-ttu-id="5bf46-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bf46-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5bf46-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5bf46-124">Content-Type</span></span>|<span data-ttu-id="5bf46-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bf46-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bf46-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5bf46-127">Request body</span></span>

<span data-ttu-id="5bf46-128">No corpo da solicitação, forneça uma representação JSON do objeto [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="5bf46-128">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="5bf46-129">Todas as propriedades listadas na tabela a seguir são necessárias.</span><span class="sxs-lookup"><span data-stu-id="5bf46-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="5bf46-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5bf46-130">Property</span></span>|<span data-ttu-id="5bf46-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5bf46-131">Type</span></span>|<span data-ttu-id="5bf46-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bf46-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bf46-133">clientId</span><span class="sxs-lookup"><span data-stu-id="5bf46-133">clientId</span></span>|<span data-ttu-id="5bf46-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bf46-134">String</span></span>|<span data-ttu-id="5bf46-135">O ID do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5bf46-135">The client ID for the application.</span></span> <span data-ttu-id="5bf46-136">Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="5bf46-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="5bf46-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="5bf46-137">clientSecret</span></span>|<span data-ttu-id="5bf46-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bf46-138">String</span></span>|<span data-ttu-id="5bf46-139">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5bf46-139">The client secret for the application.</span></span> <span data-ttu-id="5bf46-140">Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="5bf46-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="5bf46-141">nome</span><span class="sxs-lookup"><span data-stu-id="5bf46-141">name</span></span>|<span data-ttu-id="5bf46-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bf46-142">String</span></span>|<span data-ttu-id="5bf46-143">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="5bf46-143">The display name of the identity provider.</span></span>|
|<span data-ttu-id="5bf46-144">tipo</span><span class="sxs-lookup"><span data-stu-id="5bf46-144">type</span></span>|<span data-ttu-id="5bf46-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bf46-145">String</span></span>|<span data-ttu-id="5bf46-146">A identidade do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="5bf46-146">The identity provider type.</span></span> <span data-ttu-id="5bf46-147">Deve ser um dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="5bf46-147">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="5bf46-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="5bf46-148">Microsoft</span></span><li/><span data-ttu-id="5bf46-149">Google</span><span class="sxs-lookup"><span data-stu-id="5bf46-149">Google</span></span><li/><span data-ttu-id="5bf46-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="5bf46-150">Amazon</span></span><li/><span data-ttu-id="5bf46-151">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="5bf46-151">LinkedIn</span></span><li/><span data-ttu-id="5bf46-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="5bf46-152">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="5bf46-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bf46-153">Response</span></span>

<span data-ttu-id="5bf46-154">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [identityProvider](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5bf46-154">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="5bf46-155">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="5bf46-155">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="5bf46-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5bf46-156">Example</span></span>

<span data-ttu-id="5bf46-157">O exemplo a seguir cria um **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="5bf46-157">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="5bf46-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bf46-158">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="5bf46-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bf46-159">Response</span></span>

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
  "suppressions": []
}
-->
