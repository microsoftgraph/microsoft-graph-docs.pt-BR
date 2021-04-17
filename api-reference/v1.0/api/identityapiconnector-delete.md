---
title: Excluir identityApiConnector
description: Exclua um objeto identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 37217db3bce0a8cf9c7b7d998a88ca4d63e5d41e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882785"
---
# <a name="delete-identityapiconnector"></a><span data-ttu-id="7d7ae-103">Excluir identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="7d7ae-103">Delete identityApiConnector</span></span>

<span data-ttu-id="7d7ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d7ae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7d7ae-105">[Exclua um objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="7d7ae-105">Delete an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d7ae-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7d7ae-106">Permissions</span></span>

<span data-ttu-id="7d7ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d7ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7d7ae-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d7ae-109">Permission type</span></span>                        | <span data-ttu-id="7d7ae-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d7ae-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="7d7ae-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d7ae-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7d7ae-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d7ae-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="7d7ae-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d7ae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d7ae-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d7ae-114">Not supported.</span></span>  |
| <span data-ttu-id="7d7ae-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d7ae-115">Application</span></span>                            | <span data-ttu-id="7d7ae-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d7ae-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="7d7ae-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="7d7ae-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="7d7ae-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="7d7ae-118">Global administrator</span></span>
* <span data-ttu-id="7d7ae-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="7d7ae-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="7d7ae-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d7ae-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="7d7ae-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d7ae-121">Request headers</span></span>

|<span data-ttu-id="7d7ae-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7d7ae-122">Name</span></span>|<span data-ttu-id="7d7ae-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d7ae-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7d7ae-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d7ae-124">Authorization</span></span>|<span data-ttu-id="7d7ae-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d7ae-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d7ae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d7ae-127">Request body</span></span>

<span data-ttu-id="7d7ae-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d7ae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d7ae-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d7ae-129">Response</span></span>

<span data-ttu-id="7d7ae-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7d7ae-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7d7ae-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7d7ae-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7d7ae-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d7ae-132">Request</span></span>

<span data-ttu-id="7d7ae-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d7ae-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityapiconnector"
}
-->

``` http
DELETE https://graph.microsoft.com/v1.0/identity/apiConnectors/370eeb68-dfd3-4a47-8160-8824c2358321
```

### <a name="response"></a><span data-ttu-id="7d7ae-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d7ae-134">Response</span></span>

<span data-ttu-id="7d7ae-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7d7ae-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
