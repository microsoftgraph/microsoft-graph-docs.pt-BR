---
title: Atualizar identityProvider
description: Atualize propriedades em uma identityProvider existente.
localization_priority: Normal
ms.openlocfilehash: ebe49fb562f77004edfa3504130fbf50f4d40003
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832806"
---
# <a name="update-identityprovider"></a><span data-ttu-id="1e0f8-103">Atualizar identityProvider</span><span class="sxs-lookup"><span data-stu-id="1e0f8-103">Update identityProvider</span></span>

> <span data-ttu-id="1e0f8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e0f8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e0f8-106">Atualize propriedades em um existente [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="1e0f8-106">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1e0f8-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="1e0f8-107">Permissions</span></span>

<span data-ttu-id="1e0f8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e0f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e0f8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e0f8-110">Permission type</span></span>      | <span data-ttu-id="1e0f8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e0f8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e0f8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e0f8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e0f8-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e0f8-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="1e0f8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e0f8-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="1e0f8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-115">Not supported.</span></span>|
|<span data-ttu-id="1e0f8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e0f8-116">Application</span></span>|<span data-ttu-id="1e0f8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-117">Not supported.</span></span>|

<span data-ttu-id="1e0f8-118">A conta do trabalho ou da escola deve ser um administrador global do inquilino.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="1e0f8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e0f8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1e0f8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e0f8-120">Request headers</span></span>

|<span data-ttu-id="1e0f8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1e0f8-121">Name</span></span>|<span data-ttu-id="1e0f8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e0f8-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="1e0f8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e0f8-123">Authorization</span></span>|<span data-ttu-id="1e0f8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1e0f8-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1e0f8-126">Content-Type</span></span>|<span data-ttu-id="1e0f8-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e0f8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e0f8-129">Request body</span></span>

<span data-ttu-id="1e0f8-130">No corpo da solicitação, fornecem um objeto JSON com uma ou mais propriedades que precisam ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-130">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="1e0f8-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e0f8-131">Property</span></span>|<span data-ttu-id="1e0f8-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e0f8-132">Type</span></span>|<span data-ttu-id="1e0f8-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e0f8-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e0f8-134">clientId</span><span class="sxs-lookup"><span data-stu-id="1e0f8-134">clientId</span></span>|<span data-ttu-id="1e0f8-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e0f8-135">String</span></span>|<span data-ttu-id="1e0f8-136">A identificação do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-136">The client ID for the application.</span></span> <span data-ttu-id="1e0f8-137">Esta é a ID de cliente obtida ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-137">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="1e0f8-138">clientSecret</span><span class="sxs-lookup"><span data-stu-id="1e0f8-138">clientSecret</span></span>|<span data-ttu-id="1e0f8-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e0f8-139">String</span></span>|<span data-ttu-id="1e0f8-140">O segredo do cliente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-140">The client secret for the application.</span></span> <span data-ttu-id="1e0f8-141">Esse é o segredo do cliente obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-141">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="1e0f8-142">name</span><span class="sxs-lookup"><span data-stu-id="1e0f8-142">name</span></span>|<span data-ttu-id="1e0f8-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e0f8-143">String</span></span>|<span data-ttu-id="1e0f8-144">O nome de exibição do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-144">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="1e0f8-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e0f8-145">Response</span></span>

<span data-ttu-id="1e0f8-146">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-146">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="1e0f8-147">Se não obtiver êxito, uma `4xx` será retornado o erro com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-147">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="1e0f8-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e0f8-148">Example</span></span>

<span data-ttu-id="1e0f8-149">O exemplo a seguir atualiza a definição da vida útil do token **identityProvider** e define como o padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="1e0f8-149">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="1e0f8-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e0f8-150">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="1e0f8-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e0f8-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
