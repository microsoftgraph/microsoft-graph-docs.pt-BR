---
title: 'synchronizationJob: validateCredentials'
description: Valide se as credenciais são válidas no locatário.
localization_priority: Normal
ms.openlocfilehash: aede9dbb505ce43eee3399972ad26958cb9ff1b8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271313"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="3fef2-103">synchronizationJob: validateCredentials</span><span class="sxs-lookup"><span data-stu-id="3fef2-103">synchronizationJob: validateCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fef2-104">Valide se as credenciais são válidas no locatário.</span><span class="sxs-lookup"><span data-stu-id="3fef2-104">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fef2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3fef2-105">Permissions</span></span>
<span data-ttu-id="3fef2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fef2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fef2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3fef2-108">Permission type</span></span>                        | <span data-ttu-id="3fef2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3fef2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fef2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3fef2-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="3fef2-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fef2-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="3fef2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3fef2-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="3fef2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fef2-113">Not supported.</span></span> |
|<span data-ttu-id="3fef2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3fef2-114">Application</span></span>                            |<span data-ttu-id="3fef2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fef2-115">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="3fef2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3fef2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="3fef2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3fef2-117">Request headers</span></span>
| <span data-ttu-id="3fef2-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3fef2-118">Name</span></span>       | <span data-ttu-id="3fef2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fef2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3fef2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fef2-120">Authorization</span></span>  | <span data-ttu-id="3fef2-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="3fef2-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fef2-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3fef2-122">Request body</span></span>
<span data-ttu-id="3fef2-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3fef2-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3fef2-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3fef2-124">Parameter</span></span>    | <span data-ttu-id="3fef2-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fef2-125">Type</span></span>   |<span data-ttu-id="3fef2-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fef2-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3fef2-127">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="3fef2-127">useSavedCredentials</span></span>|<span data-ttu-id="3fef2-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fef2-128">Boolean</span></span>|<span data-ttu-id="3fef2-129">Quando `true`, o `credentials` parâmetro será ignorado e as credenciais salvas anteriormente (se houver alguma) serão validadas.</span><span class="sxs-lookup"><span data-stu-id="3fef2-129">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="3fef2-130">las</span><span class="sxs-lookup"><span data-stu-id="3fef2-130">credentials</span></span>|<span data-ttu-id="3fef2-131">coleção [synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="3fef2-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="3fef2-132">Credenciais a serem validadas.</span><span class="sxs-lookup"><span data-stu-id="3fef2-132">Credentials to validate.</span></span> <span data-ttu-id="3fef2-133">Ignorado quando o `useSavedCredentials` parâmetro é `true`.</span><span class="sxs-lookup"><span data-stu-id="3fef2-133">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="3fef2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fef2-134">Response</span></span>
<span data-ttu-id="3fef2-135">Se a validação for bem-sucedida, este método retornará `204, No Content` um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="3fef2-135">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="3fef2-136">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3fef2-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fef2-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3fef2-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3fef2-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3fef2-138">Request</span></span>
<span data-ttu-id="3fef2-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3fef2-139">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="3fef2-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fef2-140">Response</span></span>
<span data-ttu-id="3fef2-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3fef2-141">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3fef2-142">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="3fef2-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3fef2-143">C#</span><span class="sxs-lookup"><span data-stu-id="3fef2-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/synchronizationjob_validatecredentials-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3fef2-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="3fef2-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/synchronizationjob_validatecredentials-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3fef2-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3fef2-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/synchronizationjob_validatecredentials-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-validatecredentials.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-validatecredentials.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-validatecredentials.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
