---
title: 'riskyUser: dismiss'
description: Descartar um usuário arriscado
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d03d2199d11b2b9f285d8a425e01c70a6a49da35
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440084"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="15281-103">riskyUser: dismiss</span><span class="sxs-lookup"><span data-stu-id="15281-103">riskyUser: dismiss</span></span>
<span data-ttu-id="15281-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15281-104">Namespace: microsoft.graph</span></span>

><span data-ttu-id="15281-105">**Observação:** Usar a API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="15281-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="15281-106">Descartar o risco de um ou mais [objetos riskyUser.](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="15281-106">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="15281-107">Essa ação define o nível de risco do usuário direcionado como nenhum.</span><span class="sxs-lookup"><span data-stu-id="15281-107">This action sets the targeted user's risk level to none.</span></span>

## <a name="permissions"></a><span data-ttu-id="15281-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="15281-108">Permissions</span></span>
<span data-ttu-id="15281-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="15281-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="15281-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15281-111">Permission type</span></span>      | <span data-ttu-id="15281-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15281-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15281-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15281-113">Delegated (work or school account)</span></span> | <span data-ttu-id="15281-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15281-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="15281-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15281-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15281-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15281-116">Not supported.</span></span>    |
|<span data-ttu-id="15281-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15281-117">Application</span></span> | <span data-ttu-id="15281-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15281-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15281-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15281-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityProtection/riskyUsers/dismiss
```

## <a name="request-headers"></a><span data-ttu-id="15281-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15281-120">Request headers</span></span>
|<span data-ttu-id="15281-121">Nome</span><span class="sxs-lookup"><span data-stu-id="15281-121">Name</span></span>|<span data-ttu-id="15281-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="15281-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="15281-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="15281-123">Authorization</span></span>|<span data-ttu-id="15281-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15281-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="15281-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15281-126">Content-Type</span></span>|<span data-ttu-id="15281-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15281-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="15281-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15281-129">Request body</span></span>
<span data-ttu-id="15281-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="15281-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="15281-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="15281-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="15281-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="15281-132">Parameter</span></span>|<span data-ttu-id="15281-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="15281-133">Type</span></span>|<span data-ttu-id="15281-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="15281-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15281-135">userIds</span><span class="sxs-lookup"><span data-stu-id="15281-135">userIds</span></span>|<span data-ttu-id="15281-136">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="15281-136">String collection</span></span>|<span data-ttu-id="15281-137">Especifique os userIds a descartar no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15281-137">Specify the userIds to dismiss in the request body.</span></span>|



## <a name="response"></a><span data-ttu-id="15281-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="15281-138">Response</span></span>

<span data-ttu-id="15281-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="15281-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="15281-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="15281-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="15281-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15281-141">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="15281-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="15281-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


