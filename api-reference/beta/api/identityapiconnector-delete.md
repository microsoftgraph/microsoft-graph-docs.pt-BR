---
title: Excluir identityApiConnector
description: Exclui um objeto identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: da37c47620c82ee254b2e26ef97a72ecad4b8e3e
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720078"
---
# <a name="delete-identityapiconnector"></a><span data-ttu-id="9598d-103">Excluir identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="9598d-103">Delete identityApiConnector</span></span>

<span data-ttu-id="9598d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9598d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9598d-105">Exclui um objeto [identityApiConnector](../resources/identityapiconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="9598d-105">Deletes an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9598d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9598d-106">Permissions</span></span>

<span data-ttu-id="9598d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9598d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9598d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9598d-109">Permission type</span></span>                        | <span data-ttu-id="9598d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9598d-110">Permissions (from most to least privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="9598d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9598d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9598d-112">APIConnectors. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9598d-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="9598d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9598d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9598d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9598d-114">Not supported.</span></span>  |
| <span data-ttu-id="9598d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9598d-115">Application</span></span>                            | <span data-ttu-id="9598d-116">APIConnectors. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9598d-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="9598d-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="9598d-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="9598d-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="9598d-118">Global administrator</span></span>
* <span data-ttu-id="9598d-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="9598d-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="9598d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9598d-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="9598d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9598d-121">Request headers</span></span>
|<span data-ttu-id="9598d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9598d-122">Name</span></span>|<span data-ttu-id="9598d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9598d-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9598d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9598d-124">Authorization</span></span>|<span data-ttu-id="9598d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9598d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9598d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9598d-127">Request body</span></span>
<span data-ttu-id="9598d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9598d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9598d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9598d-129">Response</span></span>

<span data-ttu-id="9598d-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9598d-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9598d-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9598d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9598d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9598d-132">Request</span></span>

<span data-ttu-id="9598d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9598d-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityapiconnector"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/apiConnectors/{id}
```

### <a name="response"></a><span data-ttu-id="9598d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9598d-134">Response</span></span>

<span data-ttu-id="9598d-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9598d-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
