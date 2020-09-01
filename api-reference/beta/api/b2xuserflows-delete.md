---
title: Excluir b2xUserFlow
description: Excluir um objeto b2xUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2e408c96d70efc04168954cbe82448a9e6a71cd1
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319635"
---
# <a name="delete-b2xuserflow"></a><span data-ttu-id="39b72-103">Excluir b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="39b72-103">Delete b2xUserFlow</span></span>

<span data-ttu-id="39b72-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39b72-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39b72-105">Excluir um objeto [b2xUserFlow](../resources/b2xuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="39b72-105">Delete a [b2xUserFlow](../resources/b2xuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="39b72-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="39b72-106">Permissions</span></span>

<span data-ttu-id="39b72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39b72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39b72-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39b72-109">Permission type</span></span>      | <span data-ttu-id="39b72-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="39b72-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39b72-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39b72-111">Delegated (work or school account)</span></span>|<span data-ttu-id="39b72-112">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="39b72-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="39b72-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39b72-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="39b72-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39b72-114">Not supported.</span></span>|
|<span data-ttu-id="39b72-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39b72-115">Application</span></span>|<span data-ttu-id="39b72-116">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="39b72-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="39b72-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="39b72-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="39b72-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="39b72-118">Global administrator</span></span>
* <span data-ttu-id="39b72-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="39b72-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="39b72-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39b72-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/b2xUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="39b72-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39b72-121">Request headers</span></span>

|<span data-ttu-id="39b72-122">Nome</span><span class="sxs-lookup"><span data-stu-id="39b72-122">Name</span></span>|<span data-ttu-id="39b72-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="39b72-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="39b72-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="39b72-124">Authorization</span></span>|<span data-ttu-id="39b72-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39b72-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="39b72-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39b72-127">Request body</span></span>

<span data-ttu-id="39b72-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="39b72-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39b72-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="39b72-129">Response</span></span>

<span data-ttu-id="39b72-130">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="39b72-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="39b72-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39b72-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="39b72-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39b72-132">Request</span></span>

<span data-ttu-id="39b72-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="39b72-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}
```

### <a name="response"></a><span data-ttu-id="39b72-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="39b72-134">Response</span></span>

<span data-ttu-id="39b72-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="39b72-135">The following is an example of the response.</span></span>

<span data-ttu-id="39b72-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="39b72-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
