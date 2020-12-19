---
title: 'riskyUser: fechar'
description: Ignorar um usuário arriscado
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f0b1d2b7b911ef4c946a6d3a3603465d6495de73
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719969"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="3a762-103">riskyUser: fechar</span><span class="sxs-lookup"><span data-stu-id="3a762-103">riskyUser: dismiss</span></span>
<span data-ttu-id="3a762-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a762-104">Namespace: microsoft.graph</span></span>

><span data-ttu-id="3a762-105">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="3a762-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="3a762-106">Descarte o risco de um ou mais objetos [riskyUser](../resources/riskyuser.md) .</span><span class="sxs-lookup"><span data-stu-id="3a762-106">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="3a762-107">Esta ação define o nível de risco do usuário de destino como nenhum.</span><span class="sxs-lookup"><span data-stu-id="3a762-107">This action sets the targeted user's risk level to none.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a762-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a762-108">Permissions</span></span>
<span data-ttu-id="3a762-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="3a762-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="3a762-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a762-111">Permission type</span></span>      | <span data-ttu-id="3a762-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a762-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a762-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a762-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3a762-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a762-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="3a762-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a762-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a762-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a762-116">Not supported.</span></span>    |
|<span data-ttu-id="3a762-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a762-117">Application</span></span> | <span data-ttu-id="3a762-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a762-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a762-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a762-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityProtection/riskyUsers/dismiss
```

## <a name="request-headers"></a><span data-ttu-id="3a762-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a762-120">Request headers</span></span>
|<span data-ttu-id="3a762-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3a762-121">Name</span></span>|<span data-ttu-id="3a762-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a762-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3a762-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a762-123">Authorization</span></span>|<span data-ttu-id="3a762-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a762-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3a762-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a762-126">Content-Type</span></span>|<span data-ttu-id="3a762-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a762-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a762-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a762-129">Request body</span></span>
<span data-ttu-id="3a762-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3a762-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3a762-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3a762-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3a762-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3a762-132">Parameter</span></span>|<span data-ttu-id="3a762-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a762-133">Type</span></span>|<span data-ttu-id="3a762-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a762-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a762-135">userIds</span><span class="sxs-lookup"><span data-stu-id="3a762-135">userIds</span></span>|<span data-ttu-id="3a762-136">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a762-136">String collection</span></span>|<span data-ttu-id="3a762-137">Especifique as userIds a serem descartadas no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a762-137">Specify the userIds to dismiss in the request body.</span></span>|



## <a name="response"></a><span data-ttu-id="3a762-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a762-138">Response</span></span>

<span data-ttu-id="3a762-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3a762-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3a762-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3a762-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3a762-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a762-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "riskyuser_dismiss"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss
Content-Type: application/json
Content-length: 39

{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
}
```


### <a name="response"></a><span data-ttu-id="3a762-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a762-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


