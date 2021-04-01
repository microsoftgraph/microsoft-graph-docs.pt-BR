---
title: Excluir identityProvider
description: Exclua um identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: cdacaf4495d6856bc39465d4bed990a20cd264e7
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491046"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="b3508-103">Excluir identityProvider</span><span class="sxs-lookup"><span data-stu-id="b3508-103">Delete identityProvider</span></span>
<span data-ttu-id="b3508-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3508-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3508-105">[Exclua um objeto socialIdentityProvider](../resources/socialidentityprovider.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b3508-105">Delete a [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD.</span></span>

<span data-ttu-id="b3508-106">No Azure AD B2C, exclua [um objeto socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) ou [um objeto appleIdentityProvider.](../resources/appleidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="b3508-106">In Azure AD B2C, delete a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3508-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3508-107">Permissions</span></span>

<span data-ttu-id="b3508-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3508-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3508-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3508-110">Permission type</span></span>      | <span data-ttu-id="b3508-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3508-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3508-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3508-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3508-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3508-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="b3508-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3508-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b3508-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3508-115">Not supported.</span></span>|
|<span data-ttu-id="b3508-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3508-116">Application</span></span>|<span data-ttu-id="b3508-117">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3508-117">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="b3508-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="b3508-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="b3508-119">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="b3508-119">Global Administrator</span></span>
* <span data-ttu-id="b3508-120">Administrador do Provedor de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="b3508-120">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="b3508-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3508-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b3508-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3508-122">Request headers</span></span>

|<span data-ttu-id="b3508-123">Nome</span><span class="sxs-lookup"><span data-stu-id="b3508-123">Name</span></span>|<span data-ttu-id="b3508-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3508-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b3508-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3508-125">Authorization</span></span>|<span data-ttu-id="b3508-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3508-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3508-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3508-128">Request body</span></span>

<span data-ttu-id="b3508-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b3508-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3508-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3508-130">Response</span></span>

<span data-ttu-id="b3508-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b3508-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b3508-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3508-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3508-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3508-133">Request</span></span>

<span data-ttu-id="b3508-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3508-134">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/identityProviders/{id}
```

### <a name="response"></a><span data-ttu-id="b3508-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3508-135">Response</span></span>

<span data-ttu-id="b3508-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3508-136">The following is an example of the response.</span></span>

<span data-ttu-id="b3508-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b3508-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
