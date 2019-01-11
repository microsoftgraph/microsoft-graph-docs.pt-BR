---
title: Criar identityProvider
description: Crie um novo identityProvider especificando o nome para exibição, tipo de identityProvider, ID de cliente e segredo do cliente.
localization_priority: Normal
ms.openlocfilehash: 50ead5acbbda7725e44de55865d6fe2184c89647
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866231"
---
# <a name="create-identityprovider"></a><span data-ttu-id="e2096-103">Criar identityProvider</span><span class="sxs-lookup"><span data-stu-id="e2096-103">Create identityProvider</span></span>

> <span data-ttu-id="e2096-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e2096-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2096-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e2096-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2096-106">Crie um novo [identityProvider](../resources/identityprovider.md) especificando o nome para exibição, tipo de identityProvider, ID de cliente e segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="e2096-106">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2096-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="e2096-107">Permissions</span></span>

<span data-ttu-id="e2096-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2096-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2096-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2096-110">Permission type</span></span>      | <span data-ttu-id="e2096-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2096-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2096-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2096-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e2096-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2096-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="e2096-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2096-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e2096-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2096-115">Not supported.</span></span>|
|<span data-ttu-id="e2096-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2096-116">Application</span></span>|<span data-ttu-id="e2096-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2096-117">Not supported.</span></span>|

<span data-ttu-id="e2096-118">A conta do trabalho ou da escola deve ser um administrador global do inquilino.</span><span class="sxs-lookup"><span data-stu-id="e2096-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="e2096-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2096-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="e2096-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2096-120">Request headers</span></span>

|<span data-ttu-id="e2096-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e2096-121">Name</span></span>|<span data-ttu-id="e2096-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2096-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e2096-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2096-123">Authorization</span></span>|<span data-ttu-id="e2096-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2096-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e2096-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e2096-126">Content-Type</span></span>|<span data-ttu-id="e2096-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2096-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2096-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2096-129">Request body</span></span>

<span data-ttu-id="e2096-130">No corpo da solicitação, fornecem uma representação de JSON do objeto [identityProvider](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="e2096-130">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="e2096-131">Todas as propriedades listadas na tabela a seguir são necessárias.</span><span class="sxs-lookup"><span data-stu-id="e2096-131">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="e2096-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2096-132">Property</span></span>|<span data-ttu-id="e2096-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2096-133">Type</span></span>|<span data-ttu-id="e2096-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2096-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2096-135">clientId</span><span class="sxs-lookup"><span data-stu-id="e2096-135">clientId</span></span>|<span data-ttu-id="e2096-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2096-136">String</span></span>|<span data-ttu-id="e2096-137">A identificação do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e2096-137">The client ID for the application.</span></span> <span data-ttu-id="e2096-138">Esta é a ID de cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="e2096-138">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="e2096-139">clientSecret</span><span class="sxs-lookup"><span data-stu-id="e2096-139">clientSecret</span></span>|<span data-ttu-id="e2096-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2096-140">String</span></span>|<span data-ttu-id="e2096-141">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e2096-141">The client secret for the application.</span></span> <span data-ttu-id="e2096-142">Esse é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="e2096-142">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="e2096-143">name</span><span class="sxs-lookup"><span data-stu-id="e2096-143">name</span></span>|<span data-ttu-id="e2096-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2096-144">String</span></span>|<span data-ttu-id="e2096-145">O nome de exibição do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="e2096-145">The display name of the identity provider.</span></span>|
|<span data-ttu-id="e2096-146">type</span><span class="sxs-lookup"><span data-stu-id="e2096-146">type</span></span>|<span data-ttu-id="e2096-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2096-147">String</span></span>|<span data-ttu-id="e2096-148">O tipo de provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="e2096-148">The identity provider type.</span></span> <span data-ttu-id="e2096-149">Ele deve ser um dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="e2096-149">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="e2096-150">Microsoft</span><span class="sxs-lookup"><span data-stu-id="e2096-150">Microsoft</span></span><li/><span data-ttu-id="e2096-151">Google</span><span class="sxs-lookup"><span data-stu-id="e2096-151">Google</span></span><li/><span data-ttu-id="e2096-152">Amazon</span><span class="sxs-lookup"><span data-stu-id="e2096-152">Amazon</span></span><li/><span data-ttu-id="e2096-153">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="e2096-153">LinkedIn</span></span><li/><span data-ttu-id="e2096-154">Facebook</span><span class="sxs-lookup"><span data-stu-id="e2096-154">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="e2096-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2096-155">Response</span></span>

<span data-ttu-id="e2096-156">Se tiver êxito, este método retornará `201 Created` objeto response de código e [identityProvider](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2096-156">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="e2096-157">Se não obtiver êxito, uma `4xx` será retornado o erro com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="e2096-157">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="e2096-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2096-158">Example</span></span>

<span data-ttu-id="e2096-159">O exemplo a seguir cria um **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="e2096-159">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="e2096-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2096-160">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="e2096-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2096-161">Response</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
