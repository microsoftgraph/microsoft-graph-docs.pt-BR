---
title: Obter userFlowLanguagePage
description: Ler os valores em um objeto userFlowLanguagePage para um idioma em um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a772f0df072436d9ff03c83493ec870e6bc5baec
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706246"
---
# <a name="get-userflowlanguagepage"></a><span data-ttu-id="51ffb-103">Obter userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="51ffb-103">Get userFlowLanguagePage</span></span>

<span data-ttu-id="51ffb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51ffb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="51ffb-105">Ler os valores em um objeto [userFlowLanguagePage](../resources/userflowlanguagepage.md) para um idioma em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="51ffb-105">Read the values in a [userFlowLanguagePage](../resources/userflowlanguagepage.md) object for a language in a user flow.</span></span> <span data-ttu-id="51ffb-106">Esses valores são mostrados para um usuário durante uma jornada do usuário definida por um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="51ffb-106">These values are shown to a user during a user journey defined by a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="51ffb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="51ffb-107">Permissions</span></span>

<span data-ttu-id="51ffb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51ffb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51ffb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51ffb-110">Permission type</span></span>      | <span data-ttu-id="51ffb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51ffb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51ffb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51ffb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51ffb-113">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="51ffb-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="51ffb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51ffb-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="51ffb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51ffb-115">Not supported.</span></span>|
|<span data-ttu-id="51ffb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51ffb-116">Application</span></span>|<span data-ttu-id="51ffb-117">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="51ffb-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="51ffb-118">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="51ffb-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="51ffb-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="51ffb-119">Global administrator</span></span>
* <span data-ttu-id="51ffb-120">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="51ffb-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="51ffb-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51ffb-121">HTTP request</span></span>

<span data-ttu-id="51ffb-122">Para fazer referência ao conteúdo dentro do objeto, você deve usar `$value` .</span><span class="sxs-lookup"><span data-stu-id="51ffb-122">To reference the content within the object, you must use `$value`.</span></span> <span data-ttu-id="51ffb-123">Isso retorna o conteúdo dentro do objeto e permite que você faça referência a ele diretamente.</span><span class="sxs-lookup"><span data-stu-id="51ffb-123">This returns the content within the object and allows you to reference it directly.</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/languages/{id}/defaultPages/{id}/$value
GET /identity/b2cUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
GET /identity/b2xUserFlows/{id}/languages/{id}/defaultPages/{id}/$value
GET /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
```

## <a name="request-headers"></a><span data-ttu-id="51ffb-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51ffb-124">Request headers</span></span>

|<span data-ttu-id="51ffb-125">Nome</span><span class="sxs-lookup"><span data-stu-id="51ffb-125">Name</span></span>|<span data-ttu-id="51ffb-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="51ffb-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="51ffb-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="51ffb-127">Authorization</span></span>|<span data-ttu-id="51ffb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51ffb-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="51ffb-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51ffb-130">Request body</span></span>

<span data-ttu-id="51ffb-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51ffb-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51ffb-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="51ffb-132">Response</span></span>

<span data-ttu-id="51ffb-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [userFlowLanguagePage](../resources/userflowlanguagepage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51ffb-133">If successful, this method returns a `200 OK` response code and a [userFlowLanguagePage](../resources/userflowlanguagepage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51ffb-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="51ffb-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="51ffb-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51ffb-135">Request</span></span>

<span data-ttu-id="51ffb-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="51ffb-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguagepage"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en/defaultPages/idpselections/$value
```

### <a name="response"></a><span data-ttu-id="51ffb-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="51ffb-137">Response</span></span>

<span data-ttu-id="51ffb-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="51ffb-138">The following is an example of the response.</span></span>

<span data-ttu-id="51ffb-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="51ffb-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguagePage"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "LocalizedStrings": [
      {
        "ElementType": "ClaimsProvider",
        "ElementId": null,
        "StringId": "AmazonExchange",
        "Override": false,
        "Value": "Amazon"
      },
      {
        "ElementType": "ClaimsProvider",
        "ElementId": null,
        "StringId": "FacebookExchange",
        "Override": false,
        "Value": "Facebook"
      }
   ]
}
```
