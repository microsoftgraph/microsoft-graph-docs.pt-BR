---
title: Criar identityProvider
description: Crie um novo identityProvider especificando o nome para exibição, tipo de identityProvider, ID de cliente e segredo do cliente.
localization_priority: Normal
ms.openlocfilehash: c0b005d729510fa68d9edd8bfea7b85687543cf2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514646"
---
# <a name="create-identityprovider"></a><span data-ttu-id="e0668-103">Criar identityProvider</span><span class="sxs-lookup"><span data-stu-id="e0668-103">Create identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0668-104">Crie um novo [identityProvider](../resources/identityprovider.md) especificando o nome para exibição, tipo de identityProvider, ID de cliente e segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="e0668-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0668-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0668-105">Permissions</span></span>

<span data-ttu-id="e0668-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0668-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0668-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0668-108">Permission type</span></span>      | <span data-ttu-id="e0668-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0668-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0668-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0668-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e0668-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0668-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="e0668-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0668-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e0668-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0668-113">Not supported.</span></span>|
|<span data-ttu-id="e0668-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0668-114">Application</span></span>|<span data-ttu-id="e0668-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0668-115">Not supported.</span></span>|

<span data-ttu-id="e0668-116">A conta do trabalho ou da escola deve ser um administrador global do inquilino.</span><span class="sxs-lookup"><span data-stu-id="e0668-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="e0668-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0668-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="e0668-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0668-118">Request headers</span></span>

|<span data-ttu-id="e0668-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e0668-119">Name</span></span>|<span data-ttu-id="e0668-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0668-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e0668-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0668-121">Authorization</span></span>|<span data-ttu-id="e0668-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0668-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e0668-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0668-124">Content-Type</span></span>|<span data-ttu-id="e0668-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0668-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0668-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0668-127">Request body</span></span>

<span data-ttu-id="e0668-128">No corpo da solicitação, fornecem uma representação de JSON do objeto [identityProvider](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="e0668-128">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="e0668-129">Todas as propriedades listadas na tabela a seguir são necessárias.</span><span class="sxs-lookup"><span data-stu-id="e0668-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="e0668-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0668-130">Property</span></span>|<span data-ttu-id="e0668-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0668-131">Type</span></span>|<span data-ttu-id="e0668-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0668-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0668-133">clientId</span><span class="sxs-lookup"><span data-stu-id="e0668-133">clientId</span></span>|<span data-ttu-id="e0668-134">String</span><span class="sxs-lookup"><span data-stu-id="e0668-134">String</span></span>|<span data-ttu-id="e0668-135">A identificação do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e0668-135">The client ID for the application.</span></span> <span data-ttu-id="e0668-136">Esta é a ID de cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="e0668-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="e0668-137">client_secret</span><span class="sxs-lookup"><span data-stu-id="e0668-137">clientSecret</span></span>|<span data-ttu-id="e0668-138">String</span><span class="sxs-lookup"><span data-stu-id="e0668-138">String</span></span>|<span data-ttu-id="e0668-139">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e0668-139">The client secret for the application.</span></span> <span data-ttu-id="e0668-140">Esse é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="e0668-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="e0668-141">name</span><span class="sxs-lookup"><span data-stu-id="e0668-141">name</span></span>|<span data-ttu-id="e0668-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0668-142">String</span></span>|<span data-ttu-id="e0668-143">O nome de exibição do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="e0668-143">The display name of the identity provider.</span></span>|
|<span data-ttu-id="e0668-144">type</span><span class="sxs-lookup"><span data-stu-id="e0668-144">type</span></span>|<span data-ttu-id="e0668-145">String</span><span class="sxs-lookup"><span data-stu-id="e0668-145">String</span></span>|<span data-ttu-id="e0668-146">O tipo de provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="e0668-146">The identity provider type.</span></span> <span data-ttu-id="e0668-147">Ele deve ser um dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="e0668-147">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="e0668-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="e0668-148">Microsoft</span></span><li/><span data-ttu-id="e0668-149">Google</span><span class="sxs-lookup"><span data-stu-id="e0668-149">Google</span></span><li/><span data-ttu-id="e0668-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="e0668-150">Amazon</span></span><li/><span data-ttu-id="e0668-151">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="e0668-151">LinkedIn</span></span><li/><span data-ttu-id="e0668-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="e0668-152">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="e0668-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0668-153">Response</span></span>

<span data-ttu-id="e0668-154">Se tiver êxito, este método retornará `201 Created` objeto response de código e [identityProvider](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0668-154">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="e0668-155">Se não obtiver êxito, uma `4xx` será retornado o erro com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="e0668-155">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="e0668-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0668-156">Example</span></span>

<span data-ttu-id="e0668-157">O exemplo a seguir cria um **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="e0668-157">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="e0668-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0668-158">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="e0668-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0668-159">Response</span></span>

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
