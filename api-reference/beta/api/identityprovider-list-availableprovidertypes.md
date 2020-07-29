---
title: Listar availableProviderTypes
description: Recupere todos os tipos de provedor de identidade disponíveis no diretório.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6b3f44c1638bf698c477fd7e0d9e02538a963b21
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509961"
---
# <a name="list-availableprovidertypes"></a><span data-ttu-id="64670-103">Listar availableProviderTypes</span><span class="sxs-lookup"><span data-stu-id="64670-103">List availableProviderTypes</span></span>

<span data-ttu-id="64670-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64670-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64670-105">Recupera todos os tipos de provedor de identidade disponíveis em um diretório.</span><span class="sxs-lookup"><span data-stu-id="64670-105">Retrieves all identity provider types available in a directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="64670-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="64670-106">Permissions</span></span>

<span data-ttu-id="64670-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64670-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64670-109">Permission type</span></span>      | <span data-ttu-id="64670-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64670-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64670-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64670-111">Delegated (work or school account)</span></span>|<span data-ttu-id="64670-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64670-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="64670-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64670-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="64670-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64670-114">Not supported.</span></span>|
|<span data-ttu-id="64670-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64670-115">Application</span></span>|<span data-ttu-id="64670-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64670-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="64670-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="64670-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="64670-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="64670-118">Global administrator</span></span>
* <span data-ttu-id="64670-119">Administrador do provedor de identidade externa</span><span class="sxs-lookup"><span data-stu-id="64670-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="64670-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64670-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders/availableProviderTypes
```

## <a name="request-headers"></a><span data-ttu-id="64670-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64670-121">Request headers</span></span>

|<span data-ttu-id="64670-122">Nome</span><span class="sxs-lookup"><span data-stu-id="64670-122">Name</span></span>|<span data-ttu-id="64670-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="64670-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="64670-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="64670-124">Authorization</span></span>|<span data-ttu-id="64670-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64670-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64670-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64670-127">Request body</span></span>
<span data-ttu-id="64670-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64670-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64670-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="64670-129">Response</span></span>

<span data-ttu-id="64670-130">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64670-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64670-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64670-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="64670-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64670-132">Request</span></span>
<span data-ttu-id="64670-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="64670-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "identityprovider_availableprovidertypes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/availableProviderTypes
```

### <a name="response"></a><span data-ttu-id="64670-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="64670-134">Response</span></span>

<span data-ttu-id="64670-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="64670-135">The following is an example of the response.</span></span>

<span data-ttu-id="64670-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="64670-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "Amazon",
      "OpenIDConnect",
      "Facebook",
      "GitHub",
      "Google",
      "LinkedIn",
      "Microsoft",
      "QQ",
      "Twitter",
      "WeChat",
      "Weibo"
  ]
}
```
