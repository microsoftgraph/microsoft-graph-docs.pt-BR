---
title: Excluir identityProvider
description: Excluir um identityprovider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c7e1d81f7a8e117bc31f9e827f83cc90bbb8db59
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509760"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="f7637-103">Excluir identityProvider</span><span class="sxs-lookup"><span data-stu-id="f7637-103">Delete identityProvider</span></span>

<span data-ttu-id="f7637-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7637-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7637-105">Excluir um [identityprovider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="f7637-105">Delete an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f7637-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7637-106">Permissions</span></span>

<span data-ttu-id="f7637-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7637-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7637-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7637-109">Permission type</span></span>      | <span data-ttu-id="f7637-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7637-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7637-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7637-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f7637-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7637-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="f7637-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7637-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f7637-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7637-114">Not supported.</span></span>|
|<span data-ttu-id="f7637-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7637-115">Application</span></span>|<span data-ttu-id="f7637-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7637-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="f7637-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="f7637-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="f7637-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="f7637-118">Global administrator</span></span>
* <span data-ttu-id="f7637-119">Administrador do provedor de identidade externa</span><span class="sxs-lookup"><span data-stu-id="f7637-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f7637-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7637-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f7637-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7637-121">Request headers</span></span>

|<span data-ttu-id="f7637-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f7637-122">Name</span></span>|<span data-ttu-id="f7637-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7637-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f7637-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7637-124">Authorization</span></span>|<span data-ttu-id="f7637-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7637-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7637-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7637-127">Request body</span></span>

<span data-ttu-id="f7637-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7637-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7637-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7637-129">Response</span></span>

<span data-ttu-id="f7637-130">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f7637-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f7637-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7637-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7637-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7637-132">Request</span></span>

<span data-ttu-id="f7637-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7637-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identityProviders/{id}
```


### <a name="response"></a><span data-ttu-id="f7637-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7637-134">Response</span></span>

<span data-ttu-id="f7637-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f7637-135">The following is an example of the response.</span></span>

<span data-ttu-id="f7637-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f7637-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
