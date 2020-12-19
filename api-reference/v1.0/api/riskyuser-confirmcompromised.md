---
title: 'riskyUser: confirmCompromised'
description: Confirmar um usuário como comprometido
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dbf80b5642616f9c48fbd3e3b80121ed77566a15
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719990"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="c136a-103">riskyUser: confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="c136a-103">riskyUser: confirmCompromised</span></span>
<span data-ttu-id="c136a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c136a-104">Namespace: microsoft.graph</span></span>

><span data-ttu-id="c136a-105">**Observação:** A API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="c136a-105">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="c136a-106">Confirme um ou mais objetos [riskyUser](../resources/riskyuser.md) como comprometidos.</span><span class="sxs-lookup"><span data-stu-id="c136a-106">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="c136a-107">Esta ação define o nível de risco do usuário de destino como alto.</span><span class="sxs-lookup"><span data-stu-id="c136a-107">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="c136a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c136a-108">Permissions</span></span>
<span data-ttu-id="c136a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="c136a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="c136a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c136a-111">Permission type</span></span>      | <span data-ttu-id="c136a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c136a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c136a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c136a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c136a-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c136a-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="c136a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c136a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c136a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c136a-116">Not supported.</span></span>    |
|<span data-ttu-id="c136a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c136a-117">Application</span></span> | <span data-ttu-id="c136a-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c136a-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c136a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c136a-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityProtection/riskyUsers/confirmCompromised
```

## <a name="request-headers"></a><span data-ttu-id="c136a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c136a-120">Request headers</span></span>
|<span data-ttu-id="c136a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c136a-121">Name</span></span>|<span data-ttu-id="c136a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c136a-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c136a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c136a-123">Authorization</span></span>|<span data-ttu-id="c136a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c136a-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c136a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c136a-126">Content-Type</span></span>|<span data-ttu-id="c136a-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c136a-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c136a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c136a-129">Request body</span></span>
<span data-ttu-id="c136a-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c136a-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c136a-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="c136a-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c136a-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c136a-132">Parameter</span></span>|<span data-ttu-id="c136a-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c136a-133">Type</span></span>|<span data-ttu-id="c136a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c136a-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c136a-135">userIds</span><span class="sxs-lookup"><span data-stu-id="c136a-135">userIds</span></span>|<span data-ttu-id="c136a-136">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c136a-136">String collection</span></span>|<span data-ttu-id="c136a-137">Especifique as IDs de usuário arriscadas a serem descartadas no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c136a-137">Specify the risky user IDs to dismiss in the request body.</span></span>|



## <a name="response"></a><span data-ttu-id="c136a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c136a-138">Response</span></span>

<span data-ttu-id="c136a-139">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c136a-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c136a-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c136a-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c136a-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c136a-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "riskyuser_confirmcompromised"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised
Content-Type: application/json
Content-length: 39

{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
}
```


### <a name="response"></a><span data-ttu-id="c136a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c136a-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


