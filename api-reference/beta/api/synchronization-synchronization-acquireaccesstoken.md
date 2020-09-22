---
title: 'sincronização: acquireAccessToken'
description: Adquirir um token de acesso OAuth para autorizar o serviço de provisionamento do Azure AD para provisionar usuários em um aplicativo
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a7ed5ab3870224e9bd37a9f9e2f75031d942cc78
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004415"
---
# <a name="acquireaccesstoken"></a><span data-ttu-id="ee7c9-103">acquireAccessToken</span><span class="sxs-lookup"><span data-stu-id="ee7c9-103">acquireAccessToken</span></span>
<span data-ttu-id="ee7c9-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ee7c9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee7c9-105">Adquirir um token de acesso OAuth para autorizar o serviço de provisionamento do Azure AD para provisionar usuários em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ee7c9-105">Acquire an OAuth Access token to authorize the Azure AD provisioning service to provision users into an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee7c9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee7c9-106">Permissions</span></span>
<span data-ttu-id="ee7c9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee7c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee7c9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee7c9-109">Permission type</span></span>|<span data-ttu-id="ee7c9-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ee7c9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee7c9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee7c9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ee7c9-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee7c9-112">Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="ee7c9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee7c9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee7c9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee7c9-114">Not supported.</span></span>|
|<span data-ttu-id="ee7c9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee7c9-115">Application</span></span>|<span data-ttu-id="ee7c9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee7c9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee7c9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee7c9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /applications/{applicationsId}/synchronization/acquireAccessToken
POST /servicePrincipals/{servicePrincipalsId}/synchronization/acquireAccessToken
```

## <a name="request-headers"></a><span data-ttu-id="ee7c9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee7c9-118">Request headers</span></span>
|<span data-ttu-id="ee7c9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ee7c9-119">Name</span></span>|<span data-ttu-id="ee7c9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee7c9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ee7c9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee7c9-121">Authorization</span></span>|<span data-ttu-id="ee7c9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee7c9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ee7c9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee7c9-124">Content-Type</span></span>|<span data-ttu-id="ee7c9-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee7c9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee7c9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee7c9-127">Request body</span></span>
<span data-ttu-id="ee7c9-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ee7c9-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ee7c9-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ee7c9-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ee7c9-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ee7c9-130">Parameter</span></span>|<span data-ttu-id="ee7c9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee7c9-131">Type</span></span>|<span data-ttu-id="ee7c9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee7c9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee7c9-133">las</span><span class="sxs-lookup"><span data-stu-id="ee7c9-133">credentials</span></span>|<span data-ttu-id="ee7c9-134">coleção [synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ee7c9-134">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="ee7c9-135">Representa um único valor secreto.</span><span class="sxs-lookup"><span data-stu-id="ee7c9-135">Represents a single secret value.</span></span>|



## <a name="response"></a><span data-ttu-id="ee7c9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee7c9-136">Response</span></span>

<span data-ttu-id="ee7c9-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ee7c9-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ee7c9-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ee7c9-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ee7c9-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee7c9-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ee7c9-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee7c9-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ee7c9-141">C#</span><span class="sxs-lookup"><span data-stu-id="ee7c9-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronization-acquireaccesstoken-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee7c9-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee7c9-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronization-acquireaccesstoken-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee7c9-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee7c9-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronization-acquireaccesstoken-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ee7c9-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee7c9-144">Response</span></span>
<span data-ttu-id="ee7c9-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ee7c9-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


