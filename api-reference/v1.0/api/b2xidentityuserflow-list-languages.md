---
title: Idiomas da lista
description: Recupere uma lista de idiomas com suporte para personalização em um fluxo de usuário B2X.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8458bff2364c9d8f5ac9fa084f72dcd57681a90c
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882862"
---
# <a name="list-languages"></a><span data-ttu-id="0238e-103">Idiomas da lista</span><span class="sxs-lookup"><span data-stu-id="0238e-103">List languages</span></span>

<span data-ttu-id="0238e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0238e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0238e-105">Recupere uma lista de idiomas com suporte para personalização em um fluxo de usuários B2X.</span><span class="sxs-lookup"><span data-stu-id="0238e-105">Retrieve a list of languages supported for customization in a B2X user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="0238e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0238e-106">Permissions</span></span>

<span data-ttu-id="0238e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0238e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0238e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0238e-109">Permission type</span></span>      | <span data-ttu-id="0238e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0238e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0238e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0238e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0238e-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0238e-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="0238e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0238e-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0238e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0238e-114">Not supported.</span></span>|
|<span data-ttu-id="0238e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0238e-115">Application</span></span>|<span data-ttu-id="0238e-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0238e-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="0238e-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="0238e-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="0238e-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="0238e-118">Global administrator</span></span>
* <span data-ttu-id="0238e-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="0238e-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="0238e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0238e-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/languages
```

## <a name="request-headers"></a><span data-ttu-id="0238e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0238e-121">Request headers</span></span>

|<span data-ttu-id="0238e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="0238e-122">Name</span></span>|<span data-ttu-id="0238e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0238e-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0238e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0238e-124">Authorization</span></span>|<span data-ttu-id="0238e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0238e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0238e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0238e-127">Request body</span></span>

<span data-ttu-id="0238e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0238e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0238e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0238e-129">Response</span></span>

<span data-ttu-id="0238e-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0238e-130">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0238e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0238e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0238e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0238e-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_2"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_PartnerSignUp/languages
```

### <a name="response"></a><span data-ttu-id="0238e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0238e-133">Response</span></span>

<span data-ttu-id="0238e-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0238e-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('B2X_1_PartnerSignUp')/languages",
  "value": [
    {
      "id": "en",
      "isEnabled": true,
      "displayName": "English"
    },
    {
      "id": "de",
      "isEnabled": true,
      "displayName": "Deutsch"
    }
  ]
}
```
