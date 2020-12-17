---
title: Criar idiomas
description: Criar um idioma personalizado em um fluxo de usuário do Azure AD B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a45e19b056b040d700bdb246e07eefee471342b2
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706200"
---
# <a name="create-languages"></a><span data-ttu-id="27f0b-103">Criar idiomas</span><span class="sxs-lookup"><span data-stu-id="27f0b-103">Create languages</span></span>

<span data-ttu-id="27f0b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27f0b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="27f0b-105">Este método é usado para criar ou atualizar um idioma personalizado em um fluxo de usuário do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="27f0b-105">This method is used to create or update a custom language in an Azure AD B2C user flow.</span></span>

<span data-ttu-id="27f0b-106">**Observação:** Você deve habilitar a personalização de idioma no fluxo de usuário do Azure AD B2C antes de poder criar um idioma personalizado.</span><span class="sxs-lookup"><span data-stu-id="27f0b-106">**Note:** You must enable language customization in the Azure AD B2C user flow before you can create a custom language.</span></span> <span data-ttu-id="27f0b-107">Para obter mais informações, consulte [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span><span class="sxs-lookup"><span data-stu-id="27f0b-107">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="27f0b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="27f0b-108">Permissions</span></span>

<span data-ttu-id="27f0b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27f0b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27f0b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27f0b-111">Permission type</span></span>      | <span data-ttu-id="27f0b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27f0b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27f0b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27f0b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27f0b-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27f0b-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="27f0b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27f0b-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="27f0b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27f0b-116">Not supported.</span></span>|
|<span data-ttu-id="27f0b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27f0b-117">Application</span></span>|<span data-ttu-id="27f0b-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27f0b-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="27f0b-119">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="27f0b-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="27f0b-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="27f0b-120">Global administrator</span></span>
* <span data-ttu-id="27f0b-121">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="27f0b-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="27f0b-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27f0b-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2cUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="27f0b-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27f0b-123">Request headers</span></span>

|<span data-ttu-id="27f0b-124">Nome</span><span class="sxs-lookup"><span data-stu-id="27f0b-124">Name</span></span>|<span data-ttu-id="27f0b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="27f0b-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="27f0b-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="27f0b-126">Authorization</span></span>|<span data-ttu-id="27f0b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27f0b-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="27f0b-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27f0b-129">Content-Type</span></span>|<span data-ttu-id="27f0b-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27f0b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27f0b-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27f0b-132">Request body</span></span>

<span data-ttu-id="27f0b-133">No corpo da solicitação, forneça uma representação JSON do objeto [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="27f0b-133">In the request body, supply a JSON representation of the [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span>

<span data-ttu-id="27f0b-134">A tabela a seguir mostra as propriedades que podem ser fornecidas opcionalmente quando você cria o [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="27f0b-134">The following table shows the properties that can be optionally provided when you create the [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md).</span></span>

|<span data-ttu-id="27f0b-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27f0b-135">Property</span></span>|<span data-ttu-id="27f0b-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="27f0b-136">Type</span></span>|<span data-ttu-id="27f0b-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="27f0b-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27f0b-138">id</span><span class="sxs-lookup"><span data-stu-id="27f0b-138">id</span></span>|<span data-ttu-id="27f0b-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27f0b-139">String</span></span>|<span data-ttu-id="27f0b-140">O identificador do idioma.</span><span class="sxs-lookup"><span data-stu-id="27f0b-140">The identifier of the language.</span></span> <span data-ttu-id="27f0b-141">Este campo é a marca ID de idioma compatível com [RFC 5646](https://tools.ietf.org/html/rfc5646) e deve ser uma ID de idioma documentada.</span><span class="sxs-lookup"><span data-stu-id="27f0b-141">This field is Language ID tag [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant and must be a documented Language ID.</span></span> <span data-ttu-id="27f0b-142">Se fornecido no corpo da solicitação, ele deve corresponder ao identificador fornecido na URL de solicitação.</span><span class="sxs-lookup"><span data-stu-id="27f0b-142">If provided in the request body, it must match the identifer provided in the request URL.</span></span>|
|<span data-ttu-id="27f0b-143">isEnabled</span><span class="sxs-lookup"><span data-stu-id="27f0b-143">isEnabled</span></span>|<span data-ttu-id="27f0b-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="27f0b-144">Boolean</span></span>|<span data-ttu-id="27f0b-145">Indica se o idioma está habilitado dentro do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="27f0b-145">Indicates whether the language is enabled within the user flow.</span></span> <span data-ttu-id="27f0b-146">Se isso não for fornecido na solicitação, isEnabled será definida como "true".</span><span class="sxs-lookup"><span data-stu-id="27f0b-146">If this is not provided in the request, isEnabled will be set to 'true'.</span></span>|

## <a name="response"></a><span data-ttu-id="27f0b-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="27f0b-147">Response</span></span>

<span data-ttu-id="27f0b-148">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27f0b-148">If successful, this method returns a `201 Created` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27f0b-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="27f0b-149">Examples</span></span>

### <a name="example-1-create-a-custom-language-in-an-azure-ad-b2c-user-flow"></a><span data-ttu-id="27f0b-150">Exemplo 1: criar um idioma personalizado em um fluxo de usuário do Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="27f0b-150">Example 1: Create a custom language in an Azure AD B2C user flow</span></span>

#### <a name="request"></a><span data-ttu-id="27f0b-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27f0b-151">Request</span></span>

<span data-ttu-id="27f0b-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="27f0b-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_userflowlanguageconfiguration_from_"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages/es-ES
Content-Type: application/json

{
  "id": "es-ES",
  "isEnabled": true
}
```

#### <a name="response"></a><span data-ttu-id="27f0b-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="27f0b-153">Response</span></span>

<span data-ttu-id="27f0b-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="27f0b-154">The following is an example of the response.</span></span>

<span data-ttu-id="27f0b-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="27f0b-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_CustomerSignUp')/languages/$entity",
  "id": "es-ES",
  "isEnabled": true,
  "displayName": "Spanish (Spain)"
}
```

### <a name="example-2-update-a-custom-language-in-an-azure-ad-b2c-user-flow"></a><span data-ttu-id="27f0b-156">Exemplo 2: atualizar um idioma personalizado em um fluxo de usuário do Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="27f0b-156">Example 2: Update a custom language in an Azure AD B2C user flow</span></span>

#### <a name="request"></a><span data-ttu-id="27f0b-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27f0b-157">Request</span></span>

<span data-ttu-id="27f0b-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="27f0b-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_userflowlanguageconfiguration_from_"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages/es-ES
Content-Type: application/json

{
  "isEnabled": false
}
```

#### <a name="response"></a><span data-ttu-id="27f0b-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="27f0b-159">Response</span></span>

<span data-ttu-id="27f0b-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="27f0b-160">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
