---
title: Idiomas de lista
description: Recupere uma lista de idiomas com suporte para personalização dentro de um fluxo de usuário do B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3b4ecc71cd37ca25a4d45b2cc65f1e6ef5cc4bbb
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706198"
---
# <a name="list-languages"></a><span data-ttu-id="9e97d-103">Idiomas de lista</span><span class="sxs-lookup"><span data-stu-id="9e97d-103">List languages</span></span>

<span data-ttu-id="9e97d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e97d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e97d-105">Recupere uma lista de idiomas com suporte para personalização em um fluxo de usuário do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="9e97d-105">Retrieve a list of languages supported for customization in an Azure AD B2C user flow.</span></span>

<span data-ttu-id="9e97d-106">**Observação:** Para recuperar uma lista de idiomas com suporte para personalização, você deve primeiro habilitar a personalização de idioma em seu fluxo de usuário do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="9e97d-106">**Note:** To retrieve a list of languages supported for customization, you must first enable language customization on your Azure AD B2C user flow.</span></span> <span data-ttu-id="9e97d-107">Para obter mais informações, consulte [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span><span class="sxs-lookup"><span data-stu-id="9e97d-107">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9e97d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="9e97d-108">Permissions</span></span>

<span data-ttu-id="9e97d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e97d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e97d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e97d-111">Permission type</span></span>      | <span data-ttu-id="9e97d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e97d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e97d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e97d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9e97d-114">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9e97d-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="9e97d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e97d-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="9e97d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e97d-116">Not supported.</span></span>|
|<span data-ttu-id="9e97d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e97d-117">Application</span></span>|<span data-ttu-id="9e97d-118">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9e97d-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="9e97d-119">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="9e97d-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="9e97d-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="9e97d-120">Global administrator</span></span>
* <span data-ttu-id="9e97d-121">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="9e97d-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="9e97d-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e97d-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/languages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9e97d-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9e97d-123">Optional query parameters</span></span>

<span data-ttu-id="9e97d-124">Este método dá suporte ao `$filter` parâmetro de consulta para mostrar apenas os idiomas habilitados.</span><span class="sxs-lookup"><span data-stu-id="9e97d-124">This method supports the `$filter` query parameter to show only the enabled languages.</span></span> <span data-ttu-id="9e97d-125">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9e97d-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e97d-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e97d-126">Request headers</span></span>

|<span data-ttu-id="9e97d-127">Nome</span><span class="sxs-lookup"><span data-stu-id="9e97d-127">Name</span></span>|<span data-ttu-id="9e97d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e97d-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9e97d-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e97d-129">Authorization</span></span>|<span data-ttu-id="9e97d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e97d-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e97d-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e97d-132">Request body</span></span>

<span data-ttu-id="9e97d-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e97d-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e97d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e97d-134">Response</span></span>

<span data-ttu-id="9e97d-135">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e97d-135">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9e97d-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9e97d-136">Examples</span></span>

### <a name="example-1-retrieve-a-list-of-all-languages"></a><span data-ttu-id="9e97d-137">Exemplo 1: recuperar uma lista de todos os idiomas</span><span class="sxs-lookup"><span data-stu-id="9e97d-137">Example 1: Retrieve a list of all languages</span></span>

#### <a name="request"></a><span data-ttu-id="9e97d-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e97d-138">Request</span></span>

<span data-ttu-id="9e97d-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e97d-139">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages
```

#### <a name="response"></a><span data-ttu-id="9e97d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e97d-140">Response</span></span>

<span data-ttu-id="9e97d-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e97d-141">The following is an example of the response.</span></span>

<span data-ttu-id="9e97d-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9e97d-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguageConfiguration)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_CustomerSignUp')/languages",
  "value": [
    {
      "id": "en",
      "isEnabled": true,
      "displayName": "English"
    },
    {
      "id": "de",
      "isEnabled": false,
      "displayName": "Deutsch"
    }
  ]
}
```

### <a name="example-2-retrieve-a-list-of-only-enabled-languages"></a><span data-ttu-id="9e97d-143">Exemplo 2: recuperar uma lista de apenas idiomas habilitados</span><span class="sxs-lookup"><span data-stu-id="9e97d-143">Example 2: Retrieve a list of only enabled languages</span></span>

#### <a name="request"></a><span data-ttu-id="9e97d-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e97d-144">Request</span></span>

<span data-ttu-id="9e97d-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e97d-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_filter"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages?$filter=isEnabled eq true
```

#### <a name="response"></a><span data-ttu-id="9e97d-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e97d-146">Response</span></span>

<span data-ttu-id="9e97d-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e97d-147">The following is an example of the response.</span></span>

<span data-ttu-id="9e97d-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9e97d-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguageConfiguration)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_CustomerSignUp')/languages",
  "value": [
    {
      "id": "en",
      "isEnabled": true,
      "displayName": "English"
    }
  ]
}
```
