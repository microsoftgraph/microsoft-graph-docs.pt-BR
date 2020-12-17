---
title: Atualizar b2cIdentityUserFlow
description: Atualiza as propriedades de um objeto b2cIdentityUserFlow.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bc030097cbfc6e57cbe841f6a0dd98660d1a12f7
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706199"
---
# <a name="update-b2cidentityuserflow"></a><span data-ttu-id="ca557-103">Atualizar b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="ca557-103">Update b2cIdentityUserFlow</span></span>

<span data-ttu-id="ca557-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca557-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ca557-105">Atualiza as propriedades de um objeto [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="ca557-105">Update the properties of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca557-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ca557-106">Permissions</span></span>

<span data-ttu-id="ca557-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca557-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca557-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca557-109">Permission type</span></span>      | <span data-ttu-id="ca557-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca557-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca557-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca557-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ca557-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca557-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ca557-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca557-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ca557-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca557-114">Not supported.</span></span>|
|<span data-ttu-id="ca557-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca557-115">Application</span></span>|<span data-ttu-id="ca557-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca557-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="ca557-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="ca557-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ca557-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ca557-118">Global administrator</span></span>
* <span data-ttu-id="ca557-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="ca557-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ca557-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca557-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ca557-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca557-121">Request headers</span></span>

|<span data-ttu-id="ca557-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ca557-122">Name</span></span>|<span data-ttu-id="ca557-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca557-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ca557-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca557-124">Authorization</span></span>|<span data-ttu-id="ca557-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca557-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ca557-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca557-127">Content-Type</span></span>|<span data-ttu-id="ca557-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca557-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca557-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca557-130">Request body</span></span>

<span data-ttu-id="ca557-131">No corpo da solicitação, forneça uma representação JSON do objeto [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="ca557-131">In the request body, supply a JSON representation of the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

<span data-ttu-id="ca557-132">A tabela a seguir mostra as propriedades que podem ser atualizadas após a criação de um [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="ca557-132">The following table shows the properties that are able to be updated after you create a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

|<span data-ttu-id="ca557-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca557-133">Property</span></span>|<span data-ttu-id="ca557-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca557-134">Type</span></span>|<span data-ttu-id="ca557-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca557-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca557-136">isLanguageCustomizationEnabled</span><span class="sxs-lookup"><span data-stu-id="ca557-136">isLanguageCustomizationEnabled</span></span>|<span data-ttu-id="ca557-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca557-137">Boolean</span></span>|<span data-ttu-id="ca557-138">A propriedade que determina se a personalização de idioma será habilitada dentro do fluxo de usuário do B2C.</span><span class="sxs-lookup"><span data-stu-id="ca557-138">The property that determines whether language customization is enabled within the B2C user flow.</span></span> <span data-ttu-id="ca557-139">A personalização de idioma não é habilitada por padrão para os fluxos de usuários do B2C.</span><span class="sxs-lookup"><span data-stu-id="ca557-139">Language customization is not enabled by default for B2C user flows.</span></span>|
|<span data-ttu-id="ca557-140">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="ca557-140">defaultLanguageTag</span></span>|<span data-ttu-id="ca557-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca557-141">String</span></span>|<span data-ttu-id="ca557-142">Indica o idioma padrão do b2cIdentityUserFlow usado quando nenhuma `ui_locale` marca é especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca557-142">Indicates the default language of the b2cIdentityUserFlow that is used when no `ui_locale` tag is specified in the request.</span></span> <span data-ttu-id="ca557-143">Este campo é compatível com [RFC 5646](https://tools.ietf.org/html/rfc5646) .</span><span class="sxs-lookup"><span data-stu-id="ca557-143">This field is [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant.</span></span>|

## <a name="response"></a><span data-ttu-id="ca557-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca557-144">Response</span></span>

<span data-ttu-id="ca557-145">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca557-145">If successful, this method returns a `200 OK` response code and an updated [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ca557-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ca557-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ca557-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca557-147">Request</span></span>

<span data-ttu-id="ca557-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca557-148">The following is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="ca557-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca557-149">Response</span></span>

<span data-ttu-id="ca557-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ca557-150">The following is an example of the response.</span></span>

<span data-ttu-id="ca557-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ca557-151">**Note:** The response object shown here might be shortened for readability.</span></span>
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
