---
title: 'sincronização: acquireAccessToken'
description: Adquirir um token de Acesso OAuth para autorizar o serviço de provisionamento do Azure AD para provisionar usuários em um aplicativo
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: da06e05145949a4001600bae87d2322a532544f0
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128243"
---
# <a name="acquireaccesstoken"></a><span data-ttu-id="76e3f-103">acquireAccessToken</span><span class="sxs-lookup"><span data-stu-id="76e3f-103">acquireAccessToken</span></span>
<span data-ttu-id="76e3f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76e3f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="76e3f-105">Adquira um token de Acesso OAuth para autorizar o serviço de provisionamento do Azure AD para provisionar usuários em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="76e3f-105">Acquire an OAuth Access token to authorize the Azure AD provisioning service to provision users into an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="76e3f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="76e3f-106">Permissions</span></span>
<span data-ttu-id="76e3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76e3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76e3f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76e3f-109">Permission type</span></span>|<span data-ttu-id="76e3f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76e3f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76e3f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76e3f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="76e3f-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76e3f-112">Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="76e3f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76e3f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76e3f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76e3f-114">Not supported.</span></span>|
|<span data-ttu-id="76e3f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76e3f-115">Application</span></span>|<span data-ttu-id="76e3f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76e3f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76e3f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76e3f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /applications/{applicationsId}/synchronization/acquireAccessToken
POST /servicePrincipals/{servicePrincipalsId}/synchronization/acquireAccessToken
```

## <a name="request-headers"></a><span data-ttu-id="76e3f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76e3f-118">Request headers</span></span>
|<span data-ttu-id="76e3f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="76e3f-119">Name</span></span>|<span data-ttu-id="76e3f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="76e3f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="76e3f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="76e3f-121">Authorization</span></span>|<span data-ttu-id="76e3f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76e3f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="76e3f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76e3f-124">Content-Type</span></span>|<span data-ttu-id="76e3f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76e3f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="76e3f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76e3f-127">Request body</span></span>
<span data-ttu-id="76e3f-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="76e3f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="76e3f-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="76e3f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="76e3f-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="76e3f-130">Parameter</span></span>|<span data-ttu-id="76e3f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="76e3f-131">Type</span></span>|<span data-ttu-id="76e3f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="76e3f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76e3f-133">credenciais</span><span class="sxs-lookup"><span data-stu-id="76e3f-133">credentials</span></span>|<span data-ttu-id="76e3f-134">[Coleção synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="76e3f-134">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="76e3f-135">Representa um valor secreto único.</span><span class="sxs-lookup"><span data-stu-id="76e3f-135">Represents a single secret value.</span></span>|



## <a name="response"></a><span data-ttu-id="76e3f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="76e3f-136">Response</span></span>

<span data-ttu-id="76e3f-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="76e3f-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="76e3f-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="76e3f-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="76e3f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76e3f-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="76e3f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="76e3f-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="76e3f-141">C#</span><span class="sxs-lookup"><span data-stu-id="76e3f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronization-acquireaccesstoken-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="76e3f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76e3f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronization-acquireaccesstoken-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76e3f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76e3f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronization-acquireaccesstoken-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="76e3f-144">Java</span><span class="sxs-lookup"><span data-stu-id="76e3f-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronization-acquireaccesstoken-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="76e3f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="76e3f-145">Response</span></span>
<span data-ttu-id="76e3f-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="76e3f-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


