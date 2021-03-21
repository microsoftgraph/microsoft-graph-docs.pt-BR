---
title: Obter userFlowLanguageConfiguration
description: Leia as propriedades e as relações de um [objeto userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 25fa30b9904854ce027c503cf738cabd55ce5567
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955244"
---
# <a name="get-userflowlanguageconfiguration"></a><span data-ttu-id="019ff-103">Obter userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="019ff-103">Get userFlowLanguageConfiguration</span></span>

<span data-ttu-id="019ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="019ff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="019ff-105">Leia as propriedades e as relações de um [objeto userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="019ff-105">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="019ff-106">Esses objetos representam um idioma disponível em um fluxo de usuários.</span><span class="sxs-lookup"><span data-stu-id="019ff-106">These objects represent a language available in a user flow.</span></span>

<span data-ttu-id="019ff-107">**Observação:** Para recuperar um idioma com suporte para personalização, você deve primeiro habilitar a personalização de idioma no fluxo de usuários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="019ff-107">**Note:** To retrieve a language supported for customization, you must first enable language customization on your Azure AD B2C user flow.</span></span> <span data-ttu-id="019ff-108">Para obter mais informações, [consulte Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span><span class="sxs-lookup"><span data-stu-id="019ff-108">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span> <span data-ttu-id="019ff-109">A personalização de idioma é habilitada por padrão nos fluxos de [usuários do Azure Active Directory.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="019ff-109">Language customization is enabled by default in [Azure Active Directory user flows](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="019ff-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="019ff-110">Permissions</span></span>

<span data-ttu-id="019ff-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="019ff-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="019ff-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="019ff-113">Permission type</span></span>      | <span data-ttu-id="019ff-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="019ff-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="019ff-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="019ff-115">Delegated (work or school account)</span></span>|<span data-ttu-id="019ff-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="019ff-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="019ff-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="019ff-117">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="019ff-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="019ff-118">Not supported.</span></span>|
|<span data-ttu-id="019ff-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="019ff-119">Application</span></span>|<span data-ttu-id="019ff-120">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="019ff-120">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="019ff-121">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="019ff-121">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="019ff-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="019ff-122">Global administrator</span></span>
* <span data-ttu-id="019ff-123">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="019ff-123">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="019ff-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="019ff-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2cUserFlows/{id}/languages/{id}
GET identity/b2xUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="019ff-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="019ff-125">Request headers</span></span>

|<span data-ttu-id="019ff-126">Nome</span><span class="sxs-lookup"><span data-stu-id="019ff-126">Name</span></span>|<span data-ttu-id="019ff-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="019ff-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="019ff-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="019ff-128">Authorization</span></span>|<span data-ttu-id="019ff-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="019ff-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="019ff-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="019ff-131">Request body</span></span>

<span data-ttu-id="019ff-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="019ff-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="019ff-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="019ff-133">Response</span></span>

<span data-ttu-id="019ff-134">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="019ff-134">If successful, this method returns a `200 OK` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="019ff-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="019ff-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="019ff-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="019ff-136">Request</span></span>

<span data-ttu-id="019ff-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="019ff-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="019ff-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="019ff-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en
```
# <a name="c"></a>[<span data-ttu-id="019ff-139">C#</span><span class="sxs-lookup"><span data-stu-id="019ff-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="019ff-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="019ff-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="019ff-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="019ff-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="019ff-142">Java</span><span class="sxs-lookup"><span data-stu-id="019ff-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="019ff-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="019ff-143">Response</span></span>

<span data-ttu-id="019ff-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="019ff-144">The following is an example of the response.</span></span>

<span data-ttu-id="019ff-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="019ff-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
