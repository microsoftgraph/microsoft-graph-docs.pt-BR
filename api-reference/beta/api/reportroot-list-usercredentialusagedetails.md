---
title: Listar userCredentialUsageDetails
description: Obter uma lista de objetos userCredentialUsageDetails para um determinado locatário.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: e64d98318bcf9b083005f79156bc425a3b0d0fbc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134481"
---
# <a name="list-usercredentialusagedetails"></a><span data-ttu-id="d2a7e-103">Listar userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="d2a7e-103">List userCredentialUsageDetails</span></span>

<span data-ttu-id="d2a7e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2a7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2a7e-105">Obter uma lista de [objetos userCredentialUsageDetails](../resources/usercredentialusagedetails.md) para um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-105">Get a list of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects for a given tenant.</span></span> <span data-ttu-id="d2a7e-106">Os detalhes incluem informações do usuário, status da redefinição e o motivo da falha.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-106">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2a7e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2a7e-107">Permissions</span></span>

<span data-ttu-id="d2a7e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2a7e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2a7e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2a7e-110">Permission type</span></span>                        | <span data-ttu-id="d2a7e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2a7e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d2a7e-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2a7e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2a7e-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2a7e-113">Reports.Read.All</span></span> |
| <span data-ttu-id="d2a7e-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2a7e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2a7e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-115">Not supported.</span></span> |
| <span data-ttu-id="d2a7e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2a7e-116">Application</span></span>                            | <span data-ttu-id="d2a7e-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2a7e-117">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2a7e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2a7e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/userCredentialUsageDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2a7e-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d2a7e-119">Optional query parameters</span></span>

<span data-ttu-id="d2a7e-120">Esta função dá suporte ao parâmetro opcional de consulta OData **$filter**.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-120">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="d2a7e-121">Você pode aplicar **$filter** em uma ou mais das seguintes propriedades do [recurso userCredentialUsageDetails.](../resources/usercredentialusagedetails.md)</span><span class="sxs-lookup"><span data-stu-id="d2a7e-121">You can apply **$filter** on one or more of the following properties of the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) resource.</span></span>

| <span data-ttu-id="d2a7e-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2a7e-122">Properties</span></span> | <span data-ttu-id="d2a7e-123">Descrição e exemplo</span><span class="sxs-lookup"><span data-stu-id="d2a7e-123">Description and example</span></span> |
|:--------- |:----------- |
| <span data-ttu-id="d2a7e-124">recurso</span><span class="sxs-lookup"><span data-stu-id="d2a7e-124">feature</span></span> | <span data-ttu-id="d2a7e-125">Filtrar por tipo de dados de uso que você deseja (registro versus redefinição).</span><span class="sxs-lookup"><span data-stu-id="d2a7e-125">Filter by type of usage data that you want (registration vs reset).</span></span> <span data-ttu-id="d2a7e-126">Por exemplo: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-126">For example: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="d2a7e-127">Operadores de filtro com suporte: `eq`</span><span class="sxs-lookup"><span data-stu-id="d2a7e-127">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="d2a7e-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d2a7e-128">userDisplayName</span></span> | <span data-ttu-id="d2a7e-129">Filtrar pelo nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-129">Filter by user display name.</span></span> <span data-ttu-id="d2a7e-130">Por exemplo: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-130">For example: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="d2a7e-131">Operadores de filtro com suporte: `eq` e `startswith()` .</span><span class="sxs-lookup"><span data-stu-id="d2a7e-131">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="d2a7e-132">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-132">Supports case insensitive.</span></span> |
| <span data-ttu-id="d2a7e-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d2a7e-133">userPrincipalName</span></span>  | <span data-ttu-id="d2a7e-134">Filtrar pelo nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-134">Filter by user principal name.</span></span> <span data-ttu-id="d2a7e-135">Por exemplo: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-135">For example: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span>    <span data-ttu-id="d2a7e-136">Operadores de filtro com suporte: `eq` e `startswith()` .</span><span class="sxs-lookup"><span data-stu-id="d2a7e-136">Supported filter  operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="d2a7e-137">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-137">Supports case insensitive.</span></span> |
| <span data-ttu-id="d2a7e-138">isSuccess</span><span class="sxs-lookup"><span data-stu-id="d2a7e-138">isSuccess</span></span> | <span data-ttu-id="d2a7e-139">Filtrar por status da atividade.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-139">Filter by status of the activity.</span></span> <span data-ttu-id="d2a7e-140">Por exemplo: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-140">For example: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span></span> <span data-ttu-id="d2a7e-141">Operadores de filtro com suporte: `eq` e `orderby` .</span><span class="sxs-lookup"><span data-stu-id="d2a7e-141">Supported filter operators: `eq` and `orderby`.</span></span> |
| <span data-ttu-id="d2a7e-142">authMethod</span><span class="sxs-lookup"><span data-stu-id="d2a7e-142">authMethod</span></span>  | <span data-ttu-id="d2a7e-143">Filtrar pelos métodos de autenticação que usam durante o registro.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-143">Filter by the authentication methods using during registration.</span></span> <span data-ttu-id="d2a7e-144">Por exemplo: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-144">For example: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span></span> <span data-ttu-id="d2a7e-145">Operadores de filtro com suporte: `eq` .</span><span class="sxs-lookup"><span data-stu-id="d2a7e-145">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="d2a7e-146">failureReason</span><span class="sxs-lookup"><span data-stu-id="d2a7e-146">failureReason</span></span> | <span data-ttu-id="d2a7e-147">Filtrar por motivo de falha (se a atividade tiver falhado).</span><span class="sxs-lookup"><span data-stu-id="d2a7e-147">Filter by failure reason (if the activity has failed).</span></span> <span data-ttu-id="d2a7e-148">Por exemplo: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-148">For example: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span></span> <span data-ttu-id="d2a7e-149">Operadores de filtro com suporte: `eq` e `startswith()` .</span><span class="sxs-lookup"><span data-stu-id="d2a7e-149">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="d2a7e-150">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-150">Supports case insensitive.</span></span> |


## <a name="request-headers"></a><span data-ttu-id="d2a7e-151">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2a7e-151">Request headers</span></span>

| <span data-ttu-id="d2a7e-152">Nome</span><span class="sxs-lookup"><span data-stu-id="d2a7e-152">Name</span></span>      |<span data-ttu-id="d2a7e-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2a7e-153">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d2a7e-154">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2a7e-154">Authorization</span></span> | <span data-ttu-id="d2a7e-155">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="d2a7e-155">Bearer {token}</span></span> |
| <span data-ttu-id="d2a7e-156">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2a7e-156">Content-Type</span></span> | <span data-ttu-id="d2a7e-157">application/json</span><span class="sxs-lookup"><span data-stu-id="d2a7e-157">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2a7e-158">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2a7e-158">Request body</span></span>

<span data-ttu-id="d2a7e-159">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-159">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2a7e-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2a7e-160">Response</span></span>

<span data-ttu-id="d2a7e-161">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos userCredentialUsageDetails](../resources/usercredentialusagedetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-161">If successful, this method returns a `200 OK` response code and a collection of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2a7e-162">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d2a7e-162">Examples</span></span>

<span data-ttu-id="d2a7e-163">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-163">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d2a7e-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2a7e-164">Request</span></span>

<span data-ttu-id="d2a7e-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2a7e-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2a7e-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```
# <a name="c"></a>[<span data-ttu-id="d2a7e-167">C#</span><span class="sxs-lookup"><span data-stu-id="d2a7e-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usercredentialusagedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2a7e-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2a7e-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usercredentialusagedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2a7e-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2a7e-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usercredentialusagedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2a7e-170">Java</span><span class="sxs-lookup"><span data-stu-id="d2a7e-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usercredentialusagedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d2a7e-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2a7e-171">Response</span></span>

<span data-ttu-id="d2a7e-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-172">The following is an example of the response.</span></span>

> <span data-ttu-id="d2a7e-173">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-173">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d2a7e-174">Todas as propriedades são retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2a7e-174">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 258

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.getUserCredentialUsageDetails)",
  "value":[
    {
      "id" : "id-value",
      "feature":"registration",
      "userPrincipalName":"userPrincipalName-value",
      "userDisplayName": "userDisplayName-value",
      "isSuccess" : true,
      "authMethod": "email",
      "failureReason": "User contacted an admin after trying the email verification option",
      "eventDateTime" : "2019-04-01T00:00:00Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List userCredentialUsageDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


