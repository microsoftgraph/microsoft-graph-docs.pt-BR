---
title: Criar identityProvider
description: Criar um novo identityProvider especificando o nome de exibição, tipo de identityProvider, ID do cliente e o segredo do cliente.
localization_priority: Normal
ms.openlocfilehash: c0b005d729510fa68d9edd8bfea7b85687543cf2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32501263"
---
# <a name="create-identityprovider"></a><span data-ttu-id="915d0-103">Criar identityProvider</span><span class="sxs-lookup"><span data-stu-id="915d0-103">Create identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="915d0-104">Criar um novo [identityProvider](../resources/identityprovider.md) especificando o nome de exibição, tipo de identityProvider, ID do cliente e o segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="915d0-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="915d0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="915d0-105">Permissions</span></span>

<span data-ttu-id="915d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="915d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="915d0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="915d0-108">Permission type</span></span>      | <span data-ttu-id="915d0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="915d0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="915d0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="915d0-110">Delegated (work or school account)</span></span>|<span data-ttu-id="915d0-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="915d0-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="915d0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="915d0-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="915d0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="915d0-113">Not supported.</span></span>|
|<span data-ttu-id="915d0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="915d0-114">Application</span></span>|<span data-ttu-id="915d0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="915d0-115">Not supported.</span></span>|

<span data-ttu-id="915d0-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="915d0-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="915d0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="915d0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="915d0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="915d0-118">Request headers</span></span>

|<span data-ttu-id="915d0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="915d0-119">Name</span></span>|<span data-ttu-id="915d0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="915d0-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="915d0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="915d0-121">Authorization</span></span>|<span data-ttu-id="915d0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="915d0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="915d0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="915d0-124">Content-Type</span></span>|<span data-ttu-id="915d0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="915d0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="915d0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="915d0-127">Request body</span></span>

<span data-ttu-id="915d0-128">No corpo da solicitação, forneça uma representação JSON do objeto [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="915d0-128">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="915d0-129">Todas as propriedades listadas na tabela a seguir são necessárias.</span><span class="sxs-lookup"><span data-stu-id="915d0-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="915d0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="915d0-130">Property</span></span>|<span data-ttu-id="915d0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="915d0-131">Type</span></span>|<span data-ttu-id="915d0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="915d0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="915d0-133">clientId</span><span class="sxs-lookup"><span data-stu-id="915d0-133">clientId</span></span>|<span data-ttu-id="915d0-134">String</span><span class="sxs-lookup"><span data-stu-id="915d0-134">String</span></span>|<span data-ttu-id="915d0-135">ID do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="915d0-135">The client ID for the application.</span></span> <span data-ttu-id="915d0-136">Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="915d0-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="915d0-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="915d0-137">clientSecret</span></span>|<span data-ttu-id="915d0-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="915d0-138">String</span></span>|<span data-ttu-id="915d0-139">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="915d0-139">The client secret for the application.</span></span> <span data-ttu-id="915d0-140">Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="915d0-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="915d0-141">nome</span><span class="sxs-lookup"><span data-stu-id="915d0-141">name</span></span>|<span data-ttu-id="915d0-142">String</span><span class="sxs-lookup"><span data-stu-id="915d0-142">String</span></span>|<span data-ttu-id="915d0-143">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="915d0-143">The display name of the identity provider.</span></span>|
|<span data-ttu-id="915d0-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="915d0-144">type</span></span>|<span data-ttu-id="915d0-145">String</span><span class="sxs-lookup"><span data-stu-id="915d0-145">String</span></span>|<span data-ttu-id="915d0-146">A identidade do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="915d0-146">The identity provider type.</span></span> <span data-ttu-id="915d0-147">Deve ser um dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="915d0-147">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="915d0-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="915d0-148">Microsoft</span></span><li/><span data-ttu-id="915d0-149">Google</span><span class="sxs-lookup"><span data-stu-id="915d0-149">Google</span></span><li/><span data-ttu-id="915d0-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="915d0-150">Amazon</span></span><li/><span data-ttu-id="915d0-151">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="915d0-151">LinkedIn</span></span><li/><span data-ttu-id="915d0-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="915d0-152">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="915d0-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="915d0-153">Response</span></span>

<span data-ttu-id="915d0-154">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [identityProvider](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="915d0-154">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="915d0-155">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="915d0-155">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="915d0-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="915d0-156">Example</span></span>

<span data-ttu-id="915d0-157">O exemplo a seguir cria um **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="915d0-157">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="915d0-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="915d0-158">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="915d0-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="915d0-159">Response</span></span>

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
    "Error: /api-reference/beta/api/identityprovider-post-identityproviders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
