---
title: Excluir identityprovider de um b2cUserFlow
description: Excluir um identityprovider de um b2cUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 11bb612328c4fb65422624892bbd684c80aa893e
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319649"
---
# <a name="delete-an-identityprovider-from-a-b2cuserflow"></a><span data-ttu-id="f3191-103">Excluir um identityprovider de um b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="f3191-103">Delete an identityProvider from a b2cUserFlow</span></span>

<span data-ttu-id="f3191-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3191-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3191-105">Excluir um provedor de identidade de um objeto [b2cUserFlow](../resources/b2cuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="f3191-105">Delete an identity provider from a [b2cUserFlow](../resources/b2cuserflows.md) object.</span></span> <span data-ttu-id="f3191-106">Para obter mais informações sobre provedores de identidade disponíveis para fluxos de usuário, consulte a referência da API [identityProviders](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="f3191-106">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3191-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f3191-107">Permissions</span></span>

<span data-ttu-id="f3191-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3191-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3191-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3191-110">Permission type</span></span>      | <span data-ttu-id="f3191-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3191-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3191-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3191-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3191-113">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f3191-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="f3191-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3191-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f3191-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3191-115">Not supported.</span></span>|
|<span data-ttu-id="f3191-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3191-116">Application</span></span>| <span data-ttu-id="f3191-117">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f3191-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="f3191-118">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="f3191-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f3191-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="f3191-119">Global administrator</span></span>
* <span data-ttu-id="f3191-120">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="f3191-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f3191-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3191-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /b2cUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f3191-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3191-122">Request headers</span></span>

|<span data-ttu-id="f3191-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f3191-123">Name</span></span>|<span data-ttu-id="f3191-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3191-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f3191-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3191-125">Authorization</span></span>|<span data-ttu-id="f3191-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3191-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3191-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3191-128">Request body</span></span>

<span data-ttu-id="f3191-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f3191-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3191-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3191-130">Response</span></span>

<span data-ttu-id="f3191-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f3191-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="f3191-132">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="f3191-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="f3191-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3191-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3191-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3191-134">Request</span></span>

<span data-ttu-id="f3191-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3191-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/identityProviders/Facebook-OAUTH/$ref
```

### <a name="response"></a><span data-ttu-id="f3191-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3191-136">Response</span></span>

<span data-ttu-id="f3191-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f3191-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```