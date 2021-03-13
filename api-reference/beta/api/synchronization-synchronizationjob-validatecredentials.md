---
title: 'synchronizationJob: validateCredentials'
description: Valide se as credenciais são válidas no locatário.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: ce507c989ee842040787c77f772d6188d9444a03
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50773554"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="115f7-103">synchronizationJob: validateCredentials</span><span class="sxs-lookup"><span data-stu-id="115f7-103">synchronizationJob: validateCredentials</span></span>

<span data-ttu-id="115f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="115f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="115f7-105">Valide se as credenciais são válidas no locatário.</span><span class="sxs-lookup"><span data-stu-id="115f7-105">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="115f7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="115f7-106">Permissions</span></span>
<span data-ttu-id="115f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="115f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="115f7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="115f7-109">Permission type</span></span>                        | <span data-ttu-id="115f7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="115f7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="115f7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="115f7-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="115f7-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="115f7-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="115f7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="115f7-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="115f7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="115f7-114">Not supported.</span></span> |
|<span data-ttu-id="115f7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="115f7-115">Application</span></span>                            |<span data-ttu-id="115f7-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="115f7-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="115f7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="115f7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="115f7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="115f7-118">Request headers</span></span>
| <span data-ttu-id="115f7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="115f7-119">Name</span></span>       | <span data-ttu-id="115f7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="115f7-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="115f7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="115f7-121">Authorization</span></span>  | <span data-ttu-id="115f7-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="115f7-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="115f7-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="115f7-123">Request body</span></span>
<span data-ttu-id="115f7-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="115f7-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="115f7-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="115f7-125">Parameter</span></span>    | <span data-ttu-id="115f7-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="115f7-126">Type</span></span>   |<span data-ttu-id="115f7-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="115f7-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="115f7-128">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="115f7-128">useSavedCredentials</span></span>|<span data-ttu-id="115f7-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="115f7-129">Boolean</span></span>|<span data-ttu-id="115f7-130">Quando , o parâmetro será ignorado e as credenciais `true` `credentials` salvas anteriormente (se alguma) serão validadas.</span><span class="sxs-lookup"><span data-stu-id="115f7-130">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="115f7-131">credenciais</span><span class="sxs-lookup"><span data-stu-id="115f7-131">credentials</span></span>|<span data-ttu-id="115f7-132">[coleção synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="115f7-132">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="115f7-133">Credenciais para validar.</span><span class="sxs-lookup"><span data-stu-id="115f7-133">Credentials to validate.</span></span> <span data-ttu-id="115f7-134">Ignorado quando o `useSavedCredentials` parâmetro é `true` .</span><span class="sxs-lookup"><span data-stu-id="115f7-134">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="115f7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="115f7-135">Response</span></span>
<span data-ttu-id="115f7-136">Se a validação for bem-sucedida, este método retornará `204, No Content` um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="115f7-136">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="115f7-137">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="115f7-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="115f7-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="115f7-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="115f7-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="115f7-139">Request</span></span>
<span data-ttu-id="115f7-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="115f7-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="115f7-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="115f7-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="115f7-142">C#</span><span class="sxs-lookup"><span data-stu-id="115f7-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-validatecredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="115f7-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="115f7-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-validatecredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="115f7-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="115f7-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-validatecredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="115f7-145">Java</span><span class="sxs-lookup"><span data-stu-id="115f7-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-validatecredentials-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="115f7-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="115f7-146">Response</span></span>
<span data-ttu-id="115f7-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="115f7-147">The following is an example of the response.</span></span> 
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


