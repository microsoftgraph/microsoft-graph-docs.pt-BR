---
title: Excluir b2xIdentityUserFlow
description: Exclua um objeto b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 7742d2243f79e89b0d1df39e247d97ebff940dcb
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882771"
---
# <a name="delete-b2xidentityuserflow"></a><span data-ttu-id="72531-103">Excluir b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="72531-103">Delete b2xIdentityUserFlow</span></span>

<span data-ttu-id="72531-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72531-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="72531-105">[Exclua um objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="72531-105">Delete a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="72531-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="72531-106">Permissions</span></span>

<span data-ttu-id="72531-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72531-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72531-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72531-109">Permission type</span></span>      | <span data-ttu-id="72531-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72531-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72531-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72531-111">Delegated (work or school account)</span></span>|<span data-ttu-id="72531-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72531-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="72531-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72531-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="72531-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72531-114">Not supported.</span></span>|
|<span data-ttu-id="72531-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72531-115">Application</span></span>|<span data-ttu-id="72531-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72531-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="72531-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="72531-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="72531-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="72531-118">Global administrator</span></span>
* <span data-ttu-id="72531-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="72531-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="72531-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72531-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/b2xUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="72531-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72531-121">Request headers</span></span>

|<span data-ttu-id="72531-122">Nome</span><span class="sxs-lookup"><span data-stu-id="72531-122">Name</span></span>|<span data-ttu-id="72531-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="72531-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="72531-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="72531-124">Authorization</span></span>|<span data-ttu-id="72531-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72531-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="72531-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72531-127">Request body</span></span>

<span data-ttu-id="72531-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72531-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72531-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="72531-129">Response</span></span>

<span data-ttu-id="72531-130">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="72531-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="72531-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72531-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="72531-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72531-132">Request</span></span>

<span data-ttu-id="72531-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="72531-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows"
}
-->

``` http
DELETE https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner
```

### <a name="response"></a><span data-ttu-id="72531-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="72531-134">Response</span></span>

<span data-ttu-id="72531-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="72531-135">The following is an example of the response.</span></span>

<span data-ttu-id="72531-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="72531-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
