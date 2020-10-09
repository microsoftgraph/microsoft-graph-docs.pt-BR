---
title: Obter b2cAuthenticationMethodsPolicy
description: Ler as propriedades de um objeto b2cAuthenticationMethodsPolicy.
localization_priority: Priority
author: namkedia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5b2fc42c3a2d65dd06dce6e3e39e1cae090023bb
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406253"
---
# <a name="get-b2cauthenticationmethodspolicy"></a><span data-ttu-id="787d2-103">Obter b2cAuthenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="787d2-103">Get b2cAuthenticationMethodsPolicy</span></span>

<span data-ttu-id="787d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="787d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="787d2-105">Ler as propriedades de um objeto [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="787d2-105">Read the properties of a [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="787d2-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="787d2-106">Permissions</span></span>

<span data-ttu-id="787d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="787d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="787d2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="787d2-109">Permission type</span></span>                        | <span data-ttu-id="787d2-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="787d2-110">Permissions</span></span>|
|:---------------------------------------|:---------------|
| <span data-ttu-id="787d2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="787d2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="787d2-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="787d2-112">Policy.Read.All</span></span>|
| <span data-ttu-id="787d2-113">Delegada (conta Microsoft pessoal)</span><span class="sxs-lookup"><span data-stu-id="787d2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="787d2-114">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="787d2-114">Policy.Read.All</span></span>|
| <span data-ttu-id="787d2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="787d2-115">Application</span></span>                            | <span data-ttu-id="787d2-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="787d2-116">Policy.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="787d2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="787d2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/b2cAuthenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="787d2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="787d2-118">Request headers</span></span>

| <span data-ttu-id="787d2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="787d2-119">Name</span></span>      |<span data-ttu-id="787d2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="787d2-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="787d2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="787d2-121">Authorization</span></span> | <span data-ttu-id="787d2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="787d2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="787d2-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="787d2-124">Request body</span></span>

<span data-ttu-id="787d2-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="787d2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="787d2-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="787d2-126">Response</span></span>

<span data-ttu-id="787d2-127">Se bem-sucedido, este método retorna um `200 OK`código de resposta e um objeto [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="787d2-127">If successful, this method returns a `200 OK` response code and the requested [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="787d2-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="787d2-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="787d2-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="787d2-129">Request</span></span>

<span data-ttu-id="787d2-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="787d2-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2cauthenticationmethodspolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/b2cAuthenticationMethodsPolicy
```

### <a name="response"></a><span data-ttu-id="787d2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="787d2-131">Response</span></span>

<span data-ttu-id="787d2-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="787d2-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cAuthenticationMethodsPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#b2cAuthenticationMethodsPolicy",
    "id": "b2CAuthenticationMethodsPolicy",
    "isEmailPasswordAuthenticationEnabled": true,
    "isUserNameAuthenticationEnabled": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get b2cAuthenticationMethodsPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
