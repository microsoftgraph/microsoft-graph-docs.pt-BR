---
title: Obter userFlowLanguageConfiguration
description: Leia as propriedades e as relações de um [objeto userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 61be7d9e73d739a445a9b7dfc96e315fb6734966
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351024"
---
# <a name="get-userflowlanguageconfiguration"></a><span data-ttu-id="80ef3-103">Obter userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="80ef3-103">Get userFlowLanguageConfiguration</span></span>

<span data-ttu-id="80ef3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80ef3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80ef3-105">Leia as propriedades e as relações de um [objeto userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80ef3-105">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="80ef3-106">Esses objetos representam um idioma disponível em um fluxo de usuários.</span><span class="sxs-lookup"><span data-stu-id="80ef3-106">These objects represent a language available in a user flow.</span></span>

<span data-ttu-id="80ef3-107">**Observação:** Para recuperar um idioma com suporte para personalização, você deve primeiro habilitar a personalização de idioma no fluxo de usuários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="80ef3-107">**Note:** To retrieve a language supported for customization, you must first enable language customization on your Azure AD B2C user flow.</span></span> <span data-ttu-id="80ef3-108">Para obter mais informações, [consulte Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span><span class="sxs-lookup"><span data-stu-id="80ef3-108">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span> <span data-ttu-id="80ef3-109">A personalização de idioma é habilitada por padrão [Azure Active Directory fluxos de usuário.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="80ef3-109">Language customization is enabled by default in [Azure Active Directory user flows](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="80ef3-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="80ef3-110">Permissions</span></span>

<span data-ttu-id="80ef3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80ef3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80ef3-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80ef3-113">Permission type</span></span>      | <span data-ttu-id="80ef3-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="80ef3-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80ef3-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80ef3-115">Delegated (work or school account)</span></span>|<span data-ttu-id="80ef3-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80ef3-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="80ef3-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80ef3-117">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="80ef3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80ef3-118">Not supported.</span></span>|
|<span data-ttu-id="80ef3-119">Application</span><span class="sxs-lookup"><span data-stu-id="80ef3-119">Application</span></span>|<span data-ttu-id="80ef3-120">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80ef3-120">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="80ef3-121">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="80ef3-121">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="80ef3-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="80ef3-122">Global administrator</span></span>
* <span data-ttu-id="80ef3-123">Administrador de identidade externa Flow usuário</span><span class="sxs-lookup"><span data-stu-id="80ef3-123">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="80ef3-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80ef3-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2cUserFlows/{id}/languages/{id}
GET identity/b2xUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="80ef3-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80ef3-125">Request headers</span></span>

|<span data-ttu-id="80ef3-126">Nome</span><span class="sxs-lookup"><span data-stu-id="80ef3-126">Name</span></span>|<span data-ttu-id="80ef3-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="80ef3-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="80ef3-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="80ef3-128">Authorization</span></span>|<span data-ttu-id="80ef3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80ef3-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="80ef3-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80ef3-131">Request body</span></span>

<span data-ttu-id="80ef3-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="80ef3-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80ef3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="80ef3-133">Response</span></span>

<span data-ttu-id="80ef3-134">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80ef3-134">If successful, this method returns a `200 OK` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="80ef3-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="80ef3-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="80ef3-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80ef3-136">Request</span></span>

<span data-ttu-id="80ef3-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="80ef3-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="80ef3-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="80ef3-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en
```
# <a name="c"></a>[<span data-ttu-id="80ef3-139">C#</span><span class="sxs-lookup"><span data-stu-id="80ef3-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80ef3-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80ef3-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80ef3-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80ef3-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80ef3-142">Java</span><span class="sxs-lookup"><span data-stu-id="80ef3-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="80ef3-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="80ef3-143">Response</span></span>

<span data-ttu-id="80ef3-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="80ef3-144">The following is an example of the response.</span></span>

<span data-ttu-id="80ef3-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="80ef3-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_Customer')/languages/$entity",
    "id": "en",
    "isEnabled": true,
    "displayName": "English"
  }
}
```
