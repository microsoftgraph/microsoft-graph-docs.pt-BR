---
title: Criar identityProvider
description: Criar um novo identityProvider
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a33354c35903fedc3efedb84e9f2ed7bc20c9506
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649359"
---
# <a name="create-identityprovider"></a><span data-ttu-id="957f0-103">Criar identityProvider</span><span class="sxs-lookup"><span data-stu-id="957f0-103">Create identityProvider</span></span>

<span data-ttu-id="957f0-104">Criar um novo [identityProvider](../resources/identityprovider.md) especificando o nome de exibição, tipo de identityProvider, ID do cliente e o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="957f0-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="957f0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="957f0-105">Permissions</span></span>

<span data-ttu-id="957f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="957f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="957f0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="957f0-108">Permission type</span></span>      | <span data-ttu-id="957f0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="957f0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="957f0-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="957f0-110">Delegated (work or school account)</span></span>|<span data-ttu-id="957f0-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="957f0-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="957f0-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="957f0-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="957f0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="957f0-113">Not supported.</span></span>|
|<span data-ttu-id="957f0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="957f0-114">Application</span></span>|<span data-ttu-id="957f0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="957f0-115">Not supported.</span></span>|

<span data-ttu-id="957f0-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="957f0-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="957f0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="957f0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="957f0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="957f0-118">Request headers</span></span>

|<span data-ttu-id="957f0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="957f0-119">Name</span></span>|<span data-ttu-id="957f0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="957f0-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="957f0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="957f0-121">Authorization</span></span>|<span data-ttu-id="957f0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="957f0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="957f0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="957f0-124">Content-Type</span></span>|<span data-ttu-id="957f0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="957f0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="957f0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="957f0-127">Request body</span></span>

<span data-ttu-id="957f0-128">No corpo da solicitação, forneça uma representação JSON do objeto [identityProvider](../resources/identityProvider.md).</span><span class="sxs-lookup"><span data-stu-id="957f0-128">In the request body, supply a JSON representation of a [team](../resources/identityProvider.md) object.</span></span> <span data-ttu-id="957f0-129">Todas as propriedades listadas na tabela a seguir são necessárias.</span><span class="sxs-lookup"><span data-stu-id="957f0-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="957f0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="957f0-130">Property</span></span>|<span data-ttu-id="957f0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="957f0-131">Type</span></span>|<span data-ttu-id="957f0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="957f0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="957f0-133">clientId</span><span class="sxs-lookup"><span data-stu-id="957f0-133">clientId</span></span>|<span data-ttu-id="957f0-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="957f0-134">String</span></span>|<span data-ttu-id="957f0-135">O ID do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="957f0-135">The client ID created for your application.</span></span> <span data-ttu-id="957f0-136">Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="957f0-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="957f0-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="957f0-137">client_secret</span></span>|<span data-ttu-id="957f0-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="957f0-138">String</span></span>|<span data-ttu-id="957f0-139">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="957f0-139">The client secret created for your application.</span></span> <span data-ttu-id="957f0-140">Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="957f0-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="957f0-141">nome</span><span class="sxs-lookup"><span data-stu-id="957f0-141">name</span></span>|<span data-ttu-id="957f0-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="957f0-142">String</span></span>|<span data-ttu-id="957f0-143">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="957f0-143">The unique name of the identity provider.</span></span>|
|<span data-ttu-id="957f0-144">tipo</span><span class="sxs-lookup"><span data-stu-id="957f0-144">type</span></span>|<span data-ttu-id="957f0-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="957f0-145">String</span></span>|<span data-ttu-id="957f0-146">A identidade do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="957f0-146">The identity provider type.</span></span> <span data-ttu-id="957f0-147">Ele deve ser um dos seguintes valores para cenários B2C:</span><span class="sxs-lookup"><span data-stu-id="957f0-147">It must be one of the following values for B2C Scenarios:</span></span> <ul><li/><span data-ttu-id="957f0-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="957f0-148">Microsoft</span></span><li/><span data-ttu-id="957f0-149">Google</span><span class="sxs-lookup"><span data-stu-id="957f0-149">Google</span></span><li/><span data-ttu-id="957f0-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="957f0-150">Amazon</span></span><li/><span data-ttu-id="957f0-151">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="957f0-151">LinkedIn</span></span><li/><span data-ttu-id="957f0-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="957f0-152">Facebook</span></span><li/><span data-ttu-id="957f0-153">GitHub</span><span class="sxs-lookup"><span data-stu-id="957f0-153">GitHub</span></span><li/><span data-ttu-id="957f0-154">Twitter</span><span class="sxs-lookup"><span data-stu-id="957f0-154">Twitter</span></span><li/><span data-ttu-id="957f0-155">Weibo</span><span class="sxs-lookup"><span data-stu-id="957f0-155">Weibo</span></span><li/><span data-ttu-id="957f0-156">QQ</span><span class="sxs-lookup"><span data-stu-id="957f0-156">QQ</span></span><li/><span data-ttu-id="957f0-157">WeChat</span><span class="sxs-lookup"><span data-stu-id="957f0-157">WeChat</span></span></ul><span data-ttu-id="957f0-158">Para B2B só pode ser Google</span><span class="sxs-lookup"><span data-stu-id="957f0-158">For B2B it can only be Google</span></span>|

## <a name="response"></a><span data-ttu-id="957f0-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="957f0-159">Response</span></span>

<span data-ttu-id="957f0-160">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [identityProvider](../resources/identityProvider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="957f0-160">If successful, this method returns a `201 Created` response code and [Contract](../resources/identityProvider.md) object in the response body.</span></span> <span data-ttu-id="957f0-161">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="957f0-161">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="957f0-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="957f0-162">Example</span></span>

<span data-ttu-id="957f0-163">O exemplo a seguir cria um **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="957f0-163">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="957f0-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="957f0-164">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/identityProviders
Content-type: application/json

{
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

##### <a name="response"></a><span data-ttu-id="957f0-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="957f0-165">Response</span></span>

<!-- { "blockType": "ignored" } -->
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
<!-- {
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


