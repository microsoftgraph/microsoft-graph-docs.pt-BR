---
title: Atualizar identityProvider
description: Atualize as propriedades em um identityprovider existente.
localization_priority: Normal
ms.openlocfilehash: d98bc5d0bd7a8f165f33c89548a69805039cdf07
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32501452"
---
# <a name="update-identityprovider"></a><span data-ttu-id="b6b8f-103">Atualizar identityProvider</span><span class="sxs-lookup"><span data-stu-id="b6b8f-103">Update identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6b8f-104">Atualizar as propriedades em um [identityProvider](../resources/identityprovider.md) existente.</span><span class="sxs-lookup"><span data-stu-id="b6b8f-104">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b6b8f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6b8f-105">Permissions</span></span>

<span data-ttu-id="b6b8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6b8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6b8f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6b8f-108">Permission type</span></span>      | <span data-ttu-id="b6b8f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6b8f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6b8f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6b8f-110">Delegated (work or school account)</span></span>|<span data-ttu-id="b6b8f-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6b8f-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="b6b8f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6b8f-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b6b8f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6b8f-113">Not supported.</span></span>|
|<span data-ttu-id="b6b8f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6b8f-114">Application</span></span>|<span data-ttu-id="b6b8f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6b8f-115">Not supported.</span></span>|

<span data-ttu-id="b6b8f-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="b6b8f-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="b6b8f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6b8f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b6b8f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6b8f-118">Request headers</span></span>

|<span data-ttu-id="b6b8f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b6b8f-119">Name</span></span>|<span data-ttu-id="b6b8f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6b8f-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b6b8f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6b8f-121">Authorization</span></span>|<span data-ttu-id="b6b8f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6b8f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b6b8f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b6b8f-124">Content-Type</span></span>|<span data-ttu-id="b6b8f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6b8f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6b8f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6b8f-127">Request body</span></span>

<span data-ttu-id="b6b8f-128">No corpo da solicitação, fornece um objeto JSON com uma ou mais propriedades que precisam ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="b6b8f-128">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="b6b8f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6b8f-129">Property</span></span>|<span data-ttu-id="b6b8f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6b8f-130">Type</span></span>|<span data-ttu-id="b6b8f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6b8f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6b8f-132">clientId</span><span class="sxs-lookup"><span data-stu-id="b6b8f-132">clientId</span></span>|<span data-ttu-id="b6b8f-133">String</span><span class="sxs-lookup"><span data-stu-id="b6b8f-133">String</span></span>|<span data-ttu-id="b6b8f-134">ID do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b6b8f-134">The client ID for the application.</span></span> <span data-ttu-id="b6b8f-135">Esta é a ID do cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="b6b8f-135">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="b6b8f-136">clientSecret</span><span class="sxs-lookup"><span data-stu-id="b6b8f-136">clientSecret</span></span>|<span data-ttu-id="b6b8f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6b8f-137">String</span></span>|<span data-ttu-id="b6b8f-138">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b6b8f-138">The client secret for the application.</span></span> <span data-ttu-id="b6b8f-139">Este é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="b6b8f-139">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="b6b8f-140">nome</span><span class="sxs-lookup"><span data-stu-id="b6b8f-140">name</span></span>|<span data-ttu-id="b6b8f-141">String</span><span class="sxs-lookup"><span data-stu-id="b6b8f-141">String</span></span>|<span data-ttu-id="b6b8f-142">O nome exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="b6b8f-142">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="b6b8f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6b8f-143">Response</span></span>

<span data-ttu-id="b6b8f-144">Quando é bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b6b8f-144">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="b6b8f-145">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="b6b8f-145">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="b6b8f-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6b8f-146">Example</span></span>

<span data-ttu-id="b6b8f-147">O exemplo a seguir atualiza a definição da vida útil do token **identityProvider** e define como o padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="b6b8f-147">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="b6b8f-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6b8f-148">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="b6b8f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6b8f-149">Response</span></span>

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
