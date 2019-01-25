---
title: 'synchronizationJob: validateCredentials'
description: Valide se as credenciais são válidas no inquilino.
localization_priority: Normal
ms.openlocfilehash: 122d673e89f15697b2fdeefbcefb516cf9ad89ca
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519000"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="87ae5-103">synchronizationJob: validateCredentials</span><span class="sxs-lookup"><span data-stu-id="87ae5-103">synchronizationJob: validateCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87ae5-104">Valide se as credenciais são válidas no inquilino.</span><span class="sxs-lookup"><span data-stu-id="87ae5-104">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="87ae5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="87ae5-105">Permissions</span></span>
<span data-ttu-id="87ae5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87ae5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87ae5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87ae5-108">Permission type</span></span>                        | <span data-ttu-id="87ae5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87ae5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="87ae5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87ae5-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="87ae5-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87ae5-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="87ae5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87ae5-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="87ae5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87ae5-113">Not supported.</span></span> |
|<span data-ttu-id="87ae5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87ae5-114">Application</span></span>                            |<span data-ttu-id="87ae5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87ae5-115">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="87ae5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87ae5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="87ae5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87ae5-117">Request headers</span></span>
| <span data-ttu-id="87ae5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="87ae5-118">Name</span></span>       | <span data-ttu-id="87ae5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="87ae5-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="87ae5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="87ae5-120">Authorization</span></span>  | <span data-ttu-id="87ae5-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="87ae5-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="87ae5-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87ae5-122">Request body</span></span>
<span data-ttu-id="87ae5-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87ae5-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="87ae5-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="87ae5-124">Parameter</span></span>    | <span data-ttu-id="87ae5-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="87ae5-125">Type</span></span>   |<span data-ttu-id="87ae5-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="87ae5-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87ae5-127">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="87ae5-127">useSavedCredentials</span></span>|<span data-ttu-id="87ae5-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="87ae5-128">Boolean</span></span>|<span data-ttu-id="87ae5-129">Quando `true`, o `credentials` parâmetro será ignorado e as credenciais salvas anteriormente (se houver) serão validadas em vez disso.</span><span class="sxs-lookup"><span data-stu-id="87ae5-129">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="87ae5-130">credenciais</span><span class="sxs-lookup"><span data-stu-id="87ae5-130">credentials</span></span>|<span data-ttu-id="87ae5-131">coleção [synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="87ae5-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="87ae5-132">Credenciais para validar.</span><span class="sxs-lookup"><span data-stu-id="87ae5-132">Credentials to validate.</span></span> <span data-ttu-id="87ae5-133">Ignorado quando o `useSavedCredentials` parâmetro é `true`.</span><span class="sxs-lookup"><span data-stu-id="87ae5-133">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="87ae5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="87ae5-134">Response</span></span>
<span data-ttu-id="87ae5-135">Se a validação for bem-sucedida, esse método retorna um `204, No Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="87ae5-135">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="87ae5-136">Ele não retornará nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87ae5-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87ae5-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87ae5-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="87ae5-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87ae5-138">Request</span></span>
<span data-ttu-id="87ae5-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="87ae5-139">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="87ae5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="87ae5-140">Response</span></span>
<span data-ttu-id="87ae5-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="87ae5-141">The following is an example of the response.</span></span> 
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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-validatecredentials.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
