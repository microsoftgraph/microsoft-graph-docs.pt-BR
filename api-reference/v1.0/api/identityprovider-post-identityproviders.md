---
title: Criar identityProvider
description: Criar um novo identityProvider
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 93fa2a438a3294ef52545bf241d93d39283f91a3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516756"
---
# <a name="create-identityprovider"></a><span data-ttu-id="384da-103">Criar identityProvider</span><span class="sxs-lookup"><span data-stu-id="384da-103">Create identityProvider</span></span>

<span data-ttu-id="384da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="384da-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="384da-105">Criar um novo [identityProvider](../resources/identityprovider.md) especificando o nome de exibição, tipo de identityProvider, ID do cliente e o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="384da-105">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="384da-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="384da-106">Permissions</span></span>

<span data-ttu-id="384da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="384da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="384da-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="384da-109">Permission type</span></span>      | <span data-ttu-id="384da-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="384da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="384da-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="384da-111">Delegated (work or school account)</span></span>|<span data-ttu-id="384da-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="384da-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="384da-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="384da-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="384da-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="384da-114">Not supported.</span></span>|
|<span data-ttu-id="384da-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="384da-115">Application</span></span>|<span data-ttu-id="384da-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="384da-116">Not supported.</span></span>|

<span data-ttu-id="384da-117">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="384da-117">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="384da-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="384da-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="384da-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="384da-119">Request headers</span></span>

|<span data-ttu-id="384da-120">Nome</span><span class="sxs-lookup"><span data-stu-id="384da-120">Name</span></span>|<span data-ttu-id="384da-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="384da-121">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="384da-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="384da-122">Authorization</span></span>|<span data-ttu-id="384da-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="384da-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="384da-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="384da-125">Content-Type</span></span>|<span data-ttu-id="384da-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="384da-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="384da-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="384da-128">Request body</span></span>

<span data-ttu-id="384da-129">No corpo da solicitação, forneça uma representação JSON do objeto [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="384da-129">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="384da-130">Todas as propriedades listadas na tabela a seguir são necessárias.</span><span class="sxs-lookup"><span data-stu-id="384da-130">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="384da-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="384da-131">Property</span></span>|<span data-ttu-id="384da-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="384da-132">Type</span></span>|<span data-ttu-id="384da-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="384da-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="384da-134">clientId</span><span class="sxs-lookup"><span data-stu-id="384da-134">clientId</span></span>|<span data-ttu-id="384da-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="384da-135">String</span></span>|<span data-ttu-id="384da-136">O ID do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="384da-136">The client ID for the application.</span></span> <span data-ttu-id="384da-137">Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="384da-137">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="384da-138">clientSecret</span><span class="sxs-lookup"><span data-stu-id="384da-138">clientSecret</span></span>|<span data-ttu-id="384da-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="384da-139">String</span></span>|<span data-ttu-id="384da-140">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="384da-140">The client secret for the application.</span></span> <span data-ttu-id="384da-141">Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="384da-141">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="384da-142">nome</span><span class="sxs-lookup"><span data-stu-id="384da-142">name</span></span>|<span data-ttu-id="384da-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="384da-143">String</span></span>|<span data-ttu-id="384da-144">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="384da-144">The display name of the identity provider.</span></span>|
|<span data-ttu-id="384da-145">tipo</span><span class="sxs-lookup"><span data-stu-id="384da-145">type</span></span>|<span data-ttu-id="384da-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="384da-146">String</span></span>|<span data-ttu-id="384da-147">A identidade do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="384da-147">The identity provider type.</span></span> <span data-ttu-id="384da-148">Ele deve ser um dos seguintes valores para cenários B2C:</span><span class="sxs-lookup"><span data-stu-id="384da-148">It must be one of the following values for B2C Scenarios:</span></span> <ul><li/><span data-ttu-id="384da-149">Microsoft</span><span class="sxs-lookup"><span data-stu-id="384da-149">Microsoft</span></span><li/><span data-ttu-id="384da-150">Google</span><span class="sxs-lookup"><span data-stu-id="384da-150">Google</span></span><li/><span data-ttu-id="384da-151">Amazon</span><span class="sxs-lookup"><span data-stu-id="384da-151">Amazon</span></span><li/><span data-ttu-id="384da-152">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="384da-152">LinkedIn</span></span><li/><span data-ttu-id="384da-153">Facebook</span><span class="sxs-lookup"><span data-stu-id="384da-153">Facebook</span></span><li/><span data-ttu-id="384da-154">GitHub</span><span class="sxs-lookup"><span data-stu-id="384da-154">GitHub</span></span><li/><span data-ttu-id="384da-155">Twitter</span><span class="sxs-lookup"><span data-stu-id="384da-155">Twitter</span></span><li/><span data-ttu-id="384da-156">Weibo</span><span class="sxs-lookup"><span data-stu-id="384da-156">Weibo</span></span><li/><span data-ttu-id="384da-157">QQ</span><span class="sxs-lookup"><span data-stu-id="384da-157">QQ</span></span><li/><span data-ttu-id="384da-158">WeChat</span><span class="sxs-lookup"><span data-stu-id="384da-158">WeChat</span></span></ul><span data-ttu-id="384da-159">Para B2B só pode ser Google</span><span class="sxs-lookup"><span data-stu-id="384da-159">For B2B it can only be Google</span></span>|

## <a name="response"></a><span data-ttu-id="384da-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="384da-160">Response</span></span>

<span data-ttu-id="384da-161">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [identityProvider](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="384da-161">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="384da-162">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="384da-162">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="384da-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="384da-163">Example</span></span>

<span data-ttu-id="384da-164">O exemplo a seguir cria um **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="384da-164">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="384da-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="384da-165">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="384da-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="384da-166">Response</span></span>

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


