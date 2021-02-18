---
title: Atualizar b2cIdentityUserFlow
description: Atualizar as propriedades de um objeto b2cIdentityUserFlow.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7450c226f80908a08b81fec13eee61ea7aaa7e14
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291954"
---
# <a name="update-b2cidentityuserflow"></a><span data-ttu-id="bf6b8-103">Atualizar b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="bf6b8-103">Update b2cIdentityUserFlow</span></span>

<span data-ttu-id="bf6b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf6b8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bf6b8-105">Atualizar as propriedades de um [objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="bf6b8-105">Update the properties of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf6b8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf6b8-106">Permissions</span></span>

<span data-ttu-id="bf6b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf6b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf6b8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf6b8-109">Permission type</span></span>      | <span data-ttu-id="bf6b8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf6b8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf6b8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf6b8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bf6b8-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf6b8-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="bf6b8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf6b8-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="bf6b8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf6b8-114">Not supported.</span></span>|
|<span data-ttu-id="bf6b8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf6b8-115">Application</span></span>|<span data-ttu-id="bf6b8-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf6b8-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="bf6b8-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="bf6b8-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="bf6b8-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="bf6b8-118">Global administrator</span></span>
* <span data-ttu-id="bf6b8-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="bf6b8-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="bf6b8-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf6b8-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bf6b8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf6b8-121">Request headers</span></span>

|<span data-ttu-id="bf6b8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="bf6b8-122">Name</span></span>|<span data-ttu-id="bf6b8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf6b8-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bf6b8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf6b8-124">Authorization</span></span>|<span data-ttu-id="bf6b8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf6b8-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bf6b8-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf6b8-127">Content-Type</span></span>|<span data-ttu-id="bf6b8-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf6b8-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf6b8-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf6b8-130">Request body</span></span>

<span data-ttu-id="bf6b8-131">No corpo da solicitação, fornece uma representação JSON do [objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="bf6b8-131">In the request body, supply a JSON representation of the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

<span data-ttu-id="bf6b8-132">A tabela a seguir mostra as propriedades que podem ser atualizadas após a criação de [um b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="bf6b8-132">The following table shows the properties that are able to be updated after you create a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

|<span data-ttu-id="bf6b8-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf6b8-133">Property</span></span>|<span data-ttu-id="bf6b8-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf6b8-134">Type</span></span>|<span data-ttu-id="bf6b8-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf6b8-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf6b8-136">isLanguageCustomizationEnabled</span><span class="sxs-lookup"><span data-stu-id="bf6b8-136">isLanguageCustomizationEnabled</span></span>|<span data-ttu-id="bf6b8-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf6b8-137">Boolean</span></span>|<span data-ttu-id="bf6b8-138">A propriedade que determina se a personalização de idioma é habilitada dentro do fluxo do usuário do B2C.</span><span class="sxs-lookup"><span data-stu-id="bf6b8-138">The property that determines whether language customization is enabled within the B2C user flow.</span></span> <span data-ttu-id="bf6b8-139">A personalização de idioma não é habilitada por padrão para os fluxos de usuário do B2C.</span><span class="sxs-lookup"><span data-stu-id="bf6b8-139">Language customization is not enabled by default for B2C user flows.</span></span>|
|<span data-ttu-id="bf6b8-140">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="bf6b8-140">defaultLanguageTag</span></span>|<span data-ttu-id="bf6b8-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf6b8-141">String</span></span>|<span data-ttu-id="bf6b8-142">Indica o idioma padrão do b2cIdentityUserFlow que será usado quando nenhuma `ui_locale` marca for especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf6b8-142">Indicates the default language of the b2cIdentityUserFlow that is used when no `ui_locale` tag is specified in the request.</span></span> <span data-ttu-id="bf6b8-143">Esse campo é [RFC 5646](https://tools.ietf.org/html/rfc5646) compatível.</span><span class="sxs-lookup"><span data-stu-id="bf6b8-143">This field is [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant.</span></span>|

## <a name="response"></a><span data-ttu-id="bf6b8-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf6b8-144">Response</span></span>

<span data-ttu-id="bf6b8-145">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf6b8-145">If successful, this method returns a `200 OK` response code and an updated [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bf6b8-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bf6b8-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bf6b8-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf6b8-147">Request</span></span>

<span data-ttu-id="bf6b8-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf6b8-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bf6b8-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf6b8-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_b2cidentityuserflow"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp
Content-Type: application/json
Content-length: 469

{
  "isLanguageCustomizationEnabled": true,
  "defaultLanguageTag": "en",
}
```
# <a name="javascript"></a>[<span data-ttu-id="bf6b8-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf6b8-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2cidentityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf6b8-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf6b8-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2cidentityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="bf6b8-152">C#</span><span class="sxs-lookup"><span data-stu-id="bf6b8-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2cidentityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bf6b8-153">Java</span><span class="sxs-lookup"><span data-stu-id="bf6b8-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-b2cidentityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bf6b8-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf6b8-154">Response</span></span>

<span data-ttu-id="bf6b8-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bf6b8-155">The following is an example of the response.</span></span>

<span data-ttu-id="bf6b8-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bf6b8-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
}
-->

``` http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create b2CUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
