---
title: 'synchronizationJob: validateCredentials'
description: Valide se as credenciais são válidas no locatário.
localization_priority: Normal
ms.openlocfilehash: 2437cfcf8a0c028d31aeb09ec1c319916de9efb2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457006"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="39462-103">synchronizationJob: validateCredentials</span><span class="sxs-lookup"><span data-stu-id="39462-103">synchronizationJob: validateCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39462-104">Valide se as credenciais são válidas no locatário.</span><span class="sxs-lookup"><span data-stu-id="39462-104">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="39462-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="39462-105">Permissions</span></span>
<span data-ttu-id="39462-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39462-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39462-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39462-108">Permission type</span></span>                        | <span data-ttu-id="39462-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="39462-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="39462-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39462-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="39462-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39462-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="39462-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39462-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="39462-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39462-113">Not supported.</span></span> |
|<span data-ttu-id="39462-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39462-114">Application</span></span>                            |<span data-ttu-id="39462-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39462-115">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="39462-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39462-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="39462-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39462-117">Request headers</span></span>
| <span data-ttu-id="39462-118">Nome</span><span class="sxs-lookup"><span data-stu-id="39462-118">Name</span></span>       | <span data-ttu-id="39462-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="39462-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="39462-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="39462-120">Authorization</span></span>  | <span data-ttu-id="39462-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="39462-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="39462-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39462-122">Request body</span></span>
<span data-ttu-id="39462-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="39462-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="39462-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="39462-124">Parameter</span></span>    | <span data-ttu-id="39462-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="39462-125">Type</span></span>   |<span data-ttu-id="39462-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="39462-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39462-127">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="39462-127">useSavedCredentials</span></span>|<span data-ttu-id="39462-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="39462-128">Boolean</span></span>|<span data-ttu-id="39462-129">Quando `true`, o `credentials` parâmetro será ignorado e as credenciais salvas anteriormente (se houver alguma) serão validadas.</span><span class="sxs-lookup"><span data-stu-id="39462-129">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="39462-130">las</span><span class="sxs-lookup"><span data-stu-id="39462-130">credentials</span></span>|<span data-ttu-id="39462-131">coleção [synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="39462-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="39462-132">Credenciais a serem validadas.</span><span class="sxs-lookup"><span data-stu-id="39462-132">Credentials to validate.</span></span> <span data-ttu-id="39462-133">Ignorado quando o `useSavedCredentials` parâmetro é `true`.</span><span class="sxs-lookup"><span data-stu-id="39462-133">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="39462-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="39462-134">Response</span></span>
<span data-ttu-id="39462-135">Se a validação for bem-sucedida, este método retornará `204, No Content` um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="39462-135">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="39462-136">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39462-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39462-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39462-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="39462-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39462-138">Request</span></span>
<span data-ttu-id="39462-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="39462-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="39462-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="39462-140">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="39462-141">C#</span><span class="sxs-lookup"><span data-stu-id="39462-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-validatecredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="39462-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="39462-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-validatecredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="39462-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="39462-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-validatecredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="39462-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="39462-144">Response</span></span>
<span data-ttu-id="39462-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="39462-145">The following is an example of the response.</span></span> 
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
