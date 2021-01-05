---
title: Atualizar b2cIdentityUserFlow
description: Atualiza as propriedades de um objeto b2cIdentityUserFlow.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2fb11cd2f9dc547499091876e1bdf6130819d270
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753121"
---
# <a name="update-b2cidentityuserflow"></a><span data-ttu-id="1b1c9-103">Atualizar b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="1b1c9-103">Update b2cIdentityUserFlow</span></span>

<span data-ttu-id="1b1c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b1c9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1b1c9-105">Atualiza as propriedades de um objeto [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="1b1c9-105">Update the properties of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b1c9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b1c9-106">Permissions</span></span>

<span data-ttu-id="1b1c9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b1c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b1c9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b1c9-109">Permission type</span></span>      | <span data-ttu-id="1b1c9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b1c9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b1c9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b1c9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1b1c9-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b1c9-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="1b1c9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b1c9-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="1b1c9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b1c9-114">Not supported.</span></span>|
|<span data-ttu-id="1b1c9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b1c9-115">Application</span></span>|<span data-ttu-id="1b1c9-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b1c9-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="1b1c9-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="1b1c9-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="1b1c9-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1b1c9-118">Global administrator</span></span>
* <span data-ttu-id="1b1c9-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="1b1c9-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="1b1c9-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b1c9-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1b1c9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b1c9-121">Request headers</span></span>

|<span data-ttu-id="1b1c9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1b1c9-122">Name</span></span>|<span data-ttu-id="1b1c9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b1c9-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1b1c9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b1c9-124">Authorization</span></span>|<span data-ttu-id="1b1c9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b1c9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1b1c9-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b1c9-127">Content-Type</span></span>|<span data-ttu-id="1b1c9-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b1c9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b1c9-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b1c9-130">Request body</span></span>

<span data-ttu-id="1b1c9-131">No corpo da solicitação, forneça uma representação JSON do objeto [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="1b1c9-131">In the request body, supply a JSON representation of the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

<span data-ttu-id="1b1c9-132">A tabela a seguir mostra as propriedades que podem ser atualizadas após a criação de um [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="1b1c9-132">The following table shows the properties that are able to be updated after you create a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

|<span data-ttu-id="1b1c9-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b1c9-133">Property</span></span>|<span data-ttu-id="1b1c9-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b1c9-134">Type</span></span>|<span data-ttu-id="1b1c9-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b1c9-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b1c9-136">isLanguageCustomizationEnabled</span><span class="sxs-lookup"><span data-stu-id="1b1c9-136">isLanguageCustomizationEnabled</span></span>|<span data-ttu-id="1b1c9-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="1b1c9-137">Boolean</span></span>|<span data-ttu-id="1b1c9-138">A propriedade que determina se a personalização de idioma é habilitada dentro do fluxo do usuário do B2C.</span><span class="sxs-lookup"><span data-stu-id="1b1c9-138">The property that determines whether language customization is enabled within the B2C user flow.</span></span> <span data-ttu-id="1b1c9-139">A personalização de idioma não é habilitada por padrão para os fluxos de usuário do B2C.</span><span class="sxs-lookup"><span data-stu-id="1b1c9-139">Language customization is not enabled by default for B2C user flows.</span></span>|
|<span data-ttu-id="1b1c9-140">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="1b1c9-140">defaultLanguageTag</span></span>|<span data-ttu-id="1b1c9-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b1c9-141">String</span></span>|<span data-ttu-id="1b1c9-142">Indica o idioma padrão do b2cIdentityUserFlow que será usado quando nenhuma `ui_locale` marca for especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b1c9-142">Indicates the default language of the b2cIdentityUserFlow that is used when no `ui_locale` tag is specified in the request.</span></span> <span data-ttu-id="1b1c9-143">Esse campo é [RFC 5646](https://tools.ietf.org/html/rfc5646) compatível.</span><span class="sxs-lookup"><span data-stu-id="1b1c9-143">This field is [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant.</span></span>|

## <a name="response"></a><span data-ttu-id="1b1c9-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b1c9-144">Response</span></span>

<span data-ttu-id="1b1c9-145">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b1c9-145">If successful, this method returns a `200 OK` response code and an updated [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b1c9-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1b1c9-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1b1c9-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b1c9-147">Request</span></span>

<span data-ttu-id="1b1c9-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b1c9-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1b1c9-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b1c9-149">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="1b1c9-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b1c9-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2cidentityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b1c9-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b1c9-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2cidentityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1b1c9-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b1c9-152">Response</span></span>

<span data-ttu-id="1b1c9-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1b1c9-153">The following is an example of the response.</span></span>

<span data-ttu-id="1b1c9-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1b1c9-154">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "Error: update_b2cidentityuserflow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: update_b2cidentityuserflow/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
