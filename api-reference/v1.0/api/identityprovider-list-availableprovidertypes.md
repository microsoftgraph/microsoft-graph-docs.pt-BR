---
title: Listar availableProviderTypes
description: Recupere todos os tipos de provedores de identidade disponíveis no diretório.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 6c7c2189db2d4f1ffcca093bac6dc1a9a127c85e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882846"
---
# <a name="list-availableprovidertypes"></a><span data-ttu-id="079d6-103">Listar availableProviderTypes</span><span class="sxs-lookup"><span data-stu-id="079d6-103">List availableProviderTypes</span></span>

<span data-ttu-id="079d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="079d6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="079d6-105">Recupera todos os tipos de provedor de identidade disponíveis em um diretório.</span><span class="sxs-lookup"><span data-stu-id="079d6-105">Retrieves all identity provider types available in a directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="079d6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="079d6-106">Permissions</span></span>

<span data-ttu-id="079d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="079d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="079d6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="079d6-109">Permission type</span></span>      | <span data-ttu-id="079d6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="079d6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="079d6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="079d6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="079d6-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="079d6-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="079d6-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="079d6-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="079d6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="079d6-114">Not supported.</span></span>|
|<span data-ttu-id="079d6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="079d6-115">Application</span></span>|<span data-ttu-id="079d6-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="079d6-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="079d6-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="079d6-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="079d6-118">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="079d6-118">Global Administrator</span></span>
* <span data-ttu-id="079d6-119">Administrador do Provedor de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="079d6-119">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="079d6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="079d6-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders/availableProviderTypes
```

## <a name="request-headers"></a><span data-ttu-id="079d6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="079d6-121">Request headers</span></span>

|<span data-ttu-id="079d6-122">Nome</span><span class="sxs-lookup"><span data-stu-id="079d6-122">Name</span></span>|<span data-ttu-id="079d6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="079d6-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="079d6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="079d6-124">Authorization</span></span>|<span data-ttu-id="079d6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="079d6-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="079d6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="079d6-127">Request body</span></span>

<span data-ttu-id="079d6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="079d6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="079d6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="079d6-129">Response</span></span>

<span data-ttu-id="079d6-130">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="079d6-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="079d6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="079d6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="079d6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="079d6-132">Request</span></span>

<span data-ttu-id="079d6-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="079d6-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "identityprovider_availableprovidertypes"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identityProviders/availableProviderTypes
```

### <a name="response"></a><span data-ttu-id="079d6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="079d6-134">Response</span></span>

<span data-ttu-id="079d6-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="079d6-135">The following is an example of the response.</span></span>

<span data-ttu-id="079d6-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="079d6-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
      "Google",
      "Facebook",
      "MicrosoftAccount",
      "EmailOTP"
  ]
}
```
