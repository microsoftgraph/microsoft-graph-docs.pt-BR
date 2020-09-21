---
title: 'synchronizationJob: validateCredentials'
description: Valide se as credenciais são válidas no locatário.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ceb65ac10fed3dee257893e2629ca137c749cb13
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969197"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="86708-103">synchronizationJob: validateCredentials</span><span class="sxs-lookup"><span data-stu-id="86708-103">synchronizationJob: validateCredentials</span></span>

<span data-ttu-id="86708-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86708-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86708-105">Valide se as credenciais são válidas no locatário.</span><span class="sxs-lookup"><span data-stu-id="86708-105">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="86708-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="86708-106">Permissions</span></span>
<span data-ttu-id="86708-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86708-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86708-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86708-109">Permission type</span></span>                        | <span data-ttu-id="86708-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86708-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="86708-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86708-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="86708-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86708-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="86708-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86708-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="86708-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86708-114">Not supported.</span></span> |
|<span data-ttu-id="86708-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86708-115">Application</span></span>                            |<span data-ttu-id="86708-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86708-116">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="86708-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86708-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="86708-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86708-118">Request headers</span></span>
| <span data-ttu-id="86708-119">Nome</span><span class="sxs-lookup"><span data-stu-id="86708-119">Name</span></span>       | <span data-ttu-id="86708-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="86708-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="86708-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="86708-121">Authorization</span></span>  | <span data-ttu-id="86708-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="86708-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="86708-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86708-123">Request body</span></span>
<span data-ttu-id="86708-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86708-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="86708-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="86708-125">Parameter</span></span>    | <span data-ttu-id="86708-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="86708-126">Type</span></span>   |<span data-ttu-id="86708-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="86708-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86708-128">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="86708-128">useSavedCredentials</span></span>|<span data-ttu-id="86708-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="86708-129">Boolean</span></span>|<span data-ttu-id="86708-130">Quando `true` , o `credentials` parâmetro será ignorado e as credenciais salvas anteriormente (se houver alguma) serão validadas.</span><span class="sxs-lookup"><span data-stu-id="86708-130">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="86708-131">las</span><span class="sxs-lookup"><span data-stu-id="86708-131">credentials</span></span>|<span data-ttu-id="86708-132">coleção [synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="86708-132">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="86708-133">Credenciais a serem validadas.</span><span class="sxs-lookup"><span data-stu-id="86708-133">Credentials to validate.</span></span> <span data-ttu-id="86708-134">Ignorado quando o `useSavedCredentials` parâmetro é `true` .</span><span class="sxs-lookup"><span data-stu-id="86708-134">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="86708-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="86708-135">Response</span></span>
<span data-ttu-id="86708-136">Se a validação for bem-sucedida, este método retornará um `204, No Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="86708-136">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="86708-137">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86708-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86708-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86708-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="86708-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86708-139">Request</span></span>
<span data-ttu-id="86708-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="86708-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="86708-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="86708-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_validatecredentials"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials
Content-type: application/json
Content-length: 218

{ 
    credentials: [ 
        { key: "UserName", value: "user@domain.com" },
        { key: "Password", value: "password-value" }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="86708-142">C#</span><span class="sxs-lookup"><span data-stu-id="86708-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-validatecredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86708-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86708-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-validatecredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86708-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86708-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-validatecredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="86708-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="86708-145">Response</span></span>
<span data-ttu-id="86708-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="86708-146">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: validateCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


