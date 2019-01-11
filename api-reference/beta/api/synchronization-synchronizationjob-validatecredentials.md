---
title: 'synchronizationJob: validateCredentials'
description: Valide se as credenciais são válidas no inquilino.
localization_priority: Normal
ms.openlocfilehash: b78d6f7b3ff197607897fbdce123aa1e7e646afc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834914"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="9aa80-103">synchronizationJob: validateCredentials</span><span class="sxs-lookup"><span data-stu-id="9aa80-103">synchronizationJob: validateCredentials</span></span>

> <span data-ttu-id="9aa80-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9aa80-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9aa80-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9aa80-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9aa80-106">Valide se as credenciais são válidas no inquilino.</span><span class="sxs-lookup"><span data-stu-id="9aa80-106">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="9aa80-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="9aa80-107">Permissions</span></span>
<span data-ttu-id="9aa80-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9aa80-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9aa80-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9aa80-110">Permission type</span></span>                        | <span data-ttu-id="9aa80-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9aa80-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9aa80-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9aa80-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="9aa80-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9aa80-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="9aa80-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9aa80-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="9aa80-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9aa80-115">Not supported.</span></span> |
|<span data-ttu-id="9aa80-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9aa80-116">Application</span></span>                            |<span data-ttu-id="9aa80-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9aa80-117">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="9aa80-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9aa80-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="9aa80-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9aa80-119">Request headers</span></span>
| <span data-ttu-id="9aa80-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9aa80-120">Name</span></span>       | <span data-ttu-id="9aa80-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9aa80-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9aa80-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9aa80-122">Authorization</span></span>  | <span data-ttu-id="9aa80-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9aa80-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9aa80-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9aa80-124">Request body</span></span>
<span data-ttu-id="9aa80-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9aa80-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9aa80-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9aa80-126">Parameter</span></span>    | <span data-ttu-id="9aa80-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="9aa80-127">Type</span></span>   |<span data-ttu-id="9aa80-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="9aa80-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9aa80-129">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="9aa80-129">useSavedCredentials</span></span>|<span data-ttu-id="9aa80-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="9aa80-130">Boolean</span></span>|<span data-ttu-id="9aa80-131">Quando `true`, o `credentials` parâmetro será ignorado e as credenciais salvas anteriormente (se houver) serão validadas em vez disso.</span><span class="sxs-lookup"><span data-stu-id="9aa80-131">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="9aa80-132">credenciais</span><span class="sxs-lookup"><span data-stu-id="9aa80-132">credentials</span></span>|<span data-ttu-id="9aa80-133">coleção [synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="9aa80-133">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="9aa80-134">Credenciais para validar.</span><span class="sxs-lookup"><span data-stu-id="9aa80-134">Credentials to validate.</span></span> <span data-ttu-id="9aa80-135">Ignorado quando o `useSavedCredentials` parâmetro é `true`.</span><span class="sxs-lookup"><span data-stu-id="9aa80-135">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="9aa80-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9aa80-136">Response</span></span>
<span data-ttu-id="9aa80-137">Se a validação for bem-sucedida, esse método retorna um `204, No Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="9aa80-137">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="9aa80-138">Ele não retornará nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9aa80-138">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9aa80-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9aa80-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9aa80-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9aa80-140">Request</span></span>
<span data-ttu-id="9aa80-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9aa80-141">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9aa80-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="9aa80-142">Response</span></span>
<span data-ttu-id="9aa80-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9aa80-143">The following is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob: validateCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
