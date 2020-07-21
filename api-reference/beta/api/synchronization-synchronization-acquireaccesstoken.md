---
title: 'sincronização: acquireAccessToken'
description: Adquirir um token de acesso OAuth para autorizar o serviço de provisionamento do Azure AD para provisionar usuários em um aplicativo
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c31da95c5da037717b1c10fc9908e41cc91392ea
ms.sourcegitcommit: 79267b6d78c3510ef609953c5a664e692794caaa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/21/2020
ms.locfileid: "45197451"
---
# <a name="acquireaccesstoken"></a><span data-ttu-id="10a85-103">acquireAccessToken</span><span class="sxs-lookup"><span data-stu-id="10a85-103">acquireAccessToken</span></span>
<span data-ttu-id="10a85-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10a85-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="10a85-105">Adquirir um token de acesso OAuth para autorizar o serviço de provisionamento do Azure AD para provisionar usuários em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="10a85-105">Acquire an OAuth Access token to authorize the Azure AD provisioning service to provision users into an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="10a85-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="10a85-106">Permissions</span></span>
<span data-ttu-id="10a85-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10a85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10a85-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10a85-109">Permission type</span></span>|<span data-ttu-id="10a85-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="10a85-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10a85-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10a85-111">Delegated (work or school account)</span></span>|<span data-ttu-id="10a85-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10a85-112">Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="10a85-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10a85-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10a85-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10a85-114">Not supported.</span></span>|
|<span data-ttu-id="10a85-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10a85-115">Application</span></span>|<span data-ttu-id="10a85-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10a85-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10a85-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10a85-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /applications/{applicationsId}/synchronization/acquireAccessToken
POST /servicePrincipals/{servicePrincipalsId}/synchronization/acquireAccessToken
```

## <a name="request-headers"></a><span data-ttu-id="10a85-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10a85-118">Request headers</span></span>
|<span data-ttu-id="10a85-119">Nome</span><span class="sxs-lookup"><span data-stu-id="10a85-119">Name</span></span>|<span data-ttu-id="10a85-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="10a85-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="10a85-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="10a85-121">Authorization</span></span>|<span data-ttu-id="10a85-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10a85-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="10a85-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10a85-124">Content-Type</span></span>|<span data-ttu-id="10a85-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10a85-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="10a85-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10a85-127">Request body</span></span>
<span data-ttu-id="10a85-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="10a85-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="10a85-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="10a85-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="10a85-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="10a85-130">Parameter</span></span>|<span data-ttu-id="10a85-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="10a85-131">Type</span></span>|<span data-ttu-id="10a85-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="10a85-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10a85-133">las</span><span class="sxs-lookup"><span data-stu-id="10a85-133">credentials</span></span>|<span data-ttu-id="10a85-134">coleção [synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="10a85-134">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="10a85-135">Representa um único valor secreto.</span><span class="sxs-lookup"><span data-stu-id="10a85-135">Represents a single secret value.</span></span>|



## <a name="response"></a><span data-ttu-id="10a85-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="10a85-136">Response</span></span>

<span data-ttu-id="10a85-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="10a85-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="10a85-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="10a85-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="10a85-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10a85-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronization_acquireaccesstoken"
}
-->
``` http
POST https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/acquireAccessToken
Content-Type: application/json
Content-length: 123

{
  "credentials": [
    {
      "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="10a85-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="10a85-140">Response</span></span>
<span data-ttu-id="10a85-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="10a85-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
