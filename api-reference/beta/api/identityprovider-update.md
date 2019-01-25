---
title: Atualizar identityProvider
description: Atualize propriedades em uma identityProvider existente.
localization_priority: Normal
ms.openlocfilehash: d98bc5d0bd7a8f165f33c89548a69805039cdf07
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525742"
---
# <a name="update-identityprovider"></a><span data-ttu-id="7f9e0-103">Atualizar identityProvider</span><span class="sxs-lookup"><span data-stu-id="7f9e0-103">Update identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f9e0-104">Atualize propriedades em um existente [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="7f9e0-104">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f9e0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f9e0-105">Permissions</span></span>

<span data-ttu-id="7f9e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f9e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f9e0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f9e0-108">Permission type</span></span>      | <span data-ttu-id="7f9e0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f9e0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f9e0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f9e0-110">Delegated (work or school account)</span></span>|<span data-ttu-id="7f9e0-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f9e0-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="7f9e0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f9e0-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="7f9e0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f9e0-113">Not supported.</span></span>|
|<span data-ttu-id="7f9e0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f9e0-114">Application</span></span>|<span data-ttu-id="7f9e0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f9e0-115">Not supported.</span></span>|

<span data-ttu-id="7f9e0-116">A conta do trabalho ou da escola deve ser um administrador global do inquilino.</span><span class="sxs-lookup"><span data-stu-id="7f9e0-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="7f9e0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f9e0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7f9e0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f9e0-118">Request headers</span></span>

|<span data-ttu-id="7f9e0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7f9e0-119">Name</span></span>|<span data-ttu-id="7f9e0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f9e0-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="7f9e0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f9e0-121">Authorization</span></span>|<span data-ttu-id="7f9e0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f9e0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7f9e0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7f9e0-124">Content-Type</span></span>|<span data-ttu-id="7f9e0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f9e0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f9e0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f9e0-127">Request body</span></span>

<span data-ttu-id="7f9e0-128">No corpo da solicitação, fornecem um objeto JSON com uma ou mais propriedades que precisam ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="7f9e0-128">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="7f9e0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f9e0-129">Property</span></span>|<span data-ttu-id="7f9e0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f9e0-130">Type</span></span>|<span data-ttu-id="7f9e0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f9e0-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f9e0-132">clientId</span><span class="sxs-lookup"><span data-stu-id="7f9e0-132">clientId</span></span>|<span data-ttu-id="7f9e0-133">String</span><span class="sxs-lookup"><span data-stu-id="7f9e0-133">String</span></span>|<span data-ttu-id="7f9e0-134">A identificação do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f9e0-134">The client ID for the application.</span></span> <span data-ttu-id="7f9e0-135">Esta é a ID de cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="7f9e0-135">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="7f9e0-136">client_secret</span><span class="sxs-lookup"><span data-stu-id="7f9e0-136">clientSecret</span></span>|<span data-ttu-id="7f9e0-137">String</span><span class="sxs-lookup"><span data-stu-id="7f9e0-137">String</span></span>|<span data-ttu-id="7f9e0-138">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f9e0-138">The client secret for the application.</span></span> <span data-ttu-id="7f9e0-139">Esse é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="7f9e0-139">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="7f9e0-140">name</span><span class="sxs-lookup"><span data-stu-id="7f9e0-140">name</span></span>|<span data-ttu-id="7f9e0-141">String</span><span class="sxs-lookup"><span data-stu-id="7f9e0-141">String</span></span>|<span data-ttu-id="7f9e0-142">O nome de exibição do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="7f9e0-142">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="7f9e0-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f9e0-143">Response</span></span>

<span data-ttu-id="7f9e0-144">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7f9e0-144">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="7f9e0-145">Se não obtiver êxito, uma `4xx` será retornado o erro com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="7f9e0-145">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="7f9e0-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f9e0-146">Example</span></span>

<span data-ttu-id="7f9e0-147">O exemplo a seguir atualiza a definição da vida útil do token **identityProvider** e define como o padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="7f9e0-147">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="7f9e0-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f9e0-148">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="7f9e0-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f9e0-149">Response</span></span>

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
    "Error: /api-reference/beta/api/identityprovider-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
