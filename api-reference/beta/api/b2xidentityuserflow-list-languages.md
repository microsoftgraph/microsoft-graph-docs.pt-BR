---
title: Idiomas de lista
description: Recupere uma lista de idiomas com suporte para personalização dentro de um fluxo de usuário do B2X.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 68ed77871be01f549f5c069613a2c2f71bdd0f65
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706197"
---
# <a name="list-languages"></a><span data-ttu-id="d6d53-103">Idiomas de lista</span><span class="sxs-lookup"><span data-stu-id="d6d53-103">List languages</span></span>

<span data-ttu-id="d6d53-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6d53-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d6d53-105">Recupere uma lista de idiomas com suporte para personalização em um fluxo de usuário do B2X.</span><span class="sxs-lookup"><span data-stu-id="d6d53-105">Retrieve a list of languages supported for customization in a B2X user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6d53-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6d53-106">Permissions</span></span>

<span data-ttu-id="d6d53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6d53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6d53-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6d53-109">Permission type</span></span>      | <span data-ttu-id="d6d53-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6d53-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6d53-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6d53-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d6d53-112">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d6d53-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="d6d53-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6d53-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d6d53-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6d53-114">Not supported.</span></span>|
|<span data-ttu-id="d6d53-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6d53-115">Application</span></span>|<span data-ttu-id="d6d53-116">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d6d53-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="d6d53-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="d6d53-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="d6d53-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d6d53-118">Global administrator</span></span>
* <span data-ttu-id="d6d53-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="d6d53-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="d6d53-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6d53-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/languages
```

## <a name="request-headers"></a><span data-ttu-id="d6d53-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6d53-121">Request headers</span></span>

|<span data-ttu-id="d6d53-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d6d53-122">Name</span></span>|<span data-ttu-id="d6d53-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6d53-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d6d53-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6d53-124">Authorization</span></span>|<span data-ttu-id="d6d53-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6d53-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6d53-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6d53-127">Request body</span></span>

<span data-ttu-id="d6d53-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d6d53-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6d53-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6d53-129">Response</span></span>

<span data-ttu-id="d6d53-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6d53-130">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d6d53-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d6d53-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d6d53-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6d53-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_PartnerSignUp/languages
```

### <a name="response"></a><span data-ttu-id="d6d53-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6d53-133">Response</span></span>

<span data-ttu-id="d6d53-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d6d53-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows('B2X_1_PartnerSignUp')/languages",
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
