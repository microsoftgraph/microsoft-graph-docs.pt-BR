---
title: Criar idiomas
description: Crie um idioma personalizado em um fluxo de usuário do Azure AD B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e24841cebf0385563a1445a576cda8e8609f40c7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438187"
---
# <a name="create-languages"></a><span data-ttu-id="e6bc5-103">Criar idiomas</span><span class="sxs-lookup"><span data-stu-id="e6bc5-103">Create languages</span></span>

<span data-ttu-id="e6bc5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6bc5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e6bc5-105">Esse método é usado para criar ou atualizar um idioma personalizado em um fluxo de usuário do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="e6bc5-105">This method is used to create or update a custom language in an Azure AD B2C user flow.</span></span>

<span data-ttu-id="e6bc5-106">**Observação:** Você deve habilitar a personalização de idioma no fluxo de usuários do Azure AD B2C antes de criar um idioma personalizado.</span><span class="sxs-lookup"><span data-stu-id="e6bc5-106">**Note:** You must enable language customization in the Azure AD B2C user flow before you can create a custom language.</span></span> <span data-ttu-id="e6bc5-107">Para obter mais informações, [consulte Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span><span class="sxs-lookup"><span data-stu-id="e6bc5-107">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e6bc5-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6bc5-108">Permissions</span></span>

<span data-ttu-id="e6bc5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6bc5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6bc5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6bc5-111">Permission type</span></span>      | <span data-ttu-id="e6bc5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6bc5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6bc5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6bc5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6bc5-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6bc5-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="e6bc5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6bc5-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e6bc5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6bc5-116">Not supported.</span></span>|
|<span data-ttu-id="e6bc5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6bc5-117">Application</span></span>|<span data-ttu-id="e6bc5-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6bc5-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="e6bc5-119">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="e6bc5-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="e6bc5-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e6bc5-120">Global administrator</span></span>
* <span data-ttu-id="e6bc5-121">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="e6bc5-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e6bc5-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6bc5-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2cUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e6bc5-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6bc5-123">Request headers</span></span>

|<span data-ttu-id="e6bc5-124">Nome</span><span class="sxs-lookup"><span data-stu-id="e6bc5-124">Name</span></span>|<span data-ttu-id="e6bc5-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6bc5-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e6bc5-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6bc5-126">Authorization</span></span>|<span data-ttu-id="e6bc5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6bc5-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e6bc5-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6bc5-129">Content-Type</span></span>|<span data-ttu-id="e6bc5-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6bc5-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6bc5-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6bc5-132">Request body</span></span>

<span data-ttu-id="e6bc5-133">No corpo da solicitação, fornece uma representação JSON do [objeto userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6bc5-133">In the request body, supply a JSON representation of the [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span>

<span data-ttu-id="e6bc5-134">A tabela a seguir mostra as propriedades que podem ser fornecidas opcionalmente quando você cria [o userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6bc5-134">The following table shows the properties that can be optionally provided when you create the [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md).</span></span>

|<span data-ttu-id="e6bc5-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6bc5-135">Property</span></span>|<span data-ttu-id="e6bc5-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6bc5-136">Type</span></span>|<span data-ttu-id="e6bc5-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6bc5-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6bc5-138">id</span><span class="sxs-lookup"><span data-stu-id="e6bc5-138">id</span></span>|<span data-ttu-id="e6bc5-139">String</span><span class="sxs-lookup"><span data-stu-id="e6bc5-139">String</span></span>|<span data-ttu-id="e6bc5-140">O identificador do idioma.</span><span class="sxs-lookup"><span data-stu-id="e6bc5-140">The identifier of the language.</span></span> <span data-ttu-id="e6bc5-141">Este campo é a marca de identificação de idioma [RFC 5646](https://tools.ietf.org/html/rfc5646) compatível e deve ser uma ID de idioma documentada.</span><span class="sxs-lookup"><span data-stu-id="e6bc5-141">This field is Language ID tag [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant and must be a documented Language ID.</span></span> <span data-ttu-id="e6bc5-142">Se fornecido no corpo da solicitação, ele deve corresponder ao identifer fornecido na URL da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6bc5-142">If provided in the request body, it must match the identifer provided in the request URL.</span></span>|
|<span data-ttu-id="e6bc5-143">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e6bc5-143">isEnabled</span></span>|<span data-ttu-id="e6bc5-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="e6bc5-144">Boolean</span></span>|<span data-ttu-id="e6bc5-145">Indica se o idioma está habilitado no fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="e6bc5-145">Indicates whether the language is enabled within the user flow.</span></span> <span data-ttu-id="e6bc5-146">Se isso não for fornecido na solicitação, isEnabled será definido como "true".</span><span class="sxs-lookup"><span data-stu-id="e6bc5-146">If this is not provided in the request, isEnabled will be set to 'true'.</span></span>|

## <a name="response"></a><span data-ttu-id="e6bc5-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6bc5-147">Response</span></span>

<span data-ttu-id="e6bc5-148">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6bc5-148">If successful, this method returns a `201 Created` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e6bc5-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e6bc5-149">Examples</span></span>

### <a name="example-1-create-a-custom-language-in-an-azure-ad-b2c-user-flow"></a><span data-ttu-id="e6bc5-150">Exemplo 1: Criar um idioma personalizado em um fluxo de usuário do Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="e6bc5-150">Example 1: Create a custom language in an Azure AD B2C user flow</span></span>

#### <a name="request"></a><span data-ttu-id="e6bc5-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6bc5-151">Request</span></span>

<span data-ttu-id="e6bc5-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6bc5-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e6bc5-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6bc5-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e6bc5-154">C#</span><span class="sxs-lookup"><span data-stu-id="e6bc5-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-userflowlanguageconfiguration-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6bc5-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6bc5-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-userflowlanguageconfiguration-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6bc5-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6bc5-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-userflowlanguageconfiguration-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6bc5-157">Java</span><span class="sxs-lookup"><span data-stu-id="e6bc5-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-userflowlanguageconfiguration-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e6bc5-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6bc5-158">Response</span></span>

<span data-ttu-id="e6bc5-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6bc5-159">The following is an example of the response.</span></span>

<span data-ttu-id="e6bc5-160">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e6bc5-160">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-update-a-custom-language-in-an-azure-ad-b2c-user-flow"></a><span data-ttu-id="e6bc5-161">Exemplo 2: atualizar um idioma personalizado em um fluxo de usuário do Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="e6bc5-161">Example 2: Update a custom language in an Azure AD B2C user flow</span></span>

#### <a name="request"></a><span data-ttu-id="e6bc5-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6bc5-162">Request</span></span>

<span data-ttu-id="e6bc5-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6bc5-163">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="e6bc5-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6bc5-164">Response</span></span>

<span data-ttu-id="e6bc5-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6bc5-165">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
