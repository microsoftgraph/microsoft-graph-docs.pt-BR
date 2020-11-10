---
title: Listar userCredentialUsageDetails
description: Obter uma lista de objetos userCredentialUsageDetails para um determinado locatário.
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: aa6c39f7f08be5f09d446214a9c34ba0d6e555a7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971477"
---
# <a name="list-usercredentialusagedetails"></a><span data-ttu-id="d0f9a-103">Listar userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="d0f9a-103">List userCredentialUsageDetails</span></span>

<span data-ttu-id="d0f9a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0f9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0f9a-105">Obter uma lista de objetos [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) para um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-105">Get a list of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects for a given tenant.</span></span> <span data-ttu-id="d0f9a-106">Os detalhes incluem informações do usuário, status da redefinição e o motivo da falha.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-106">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0f9a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0f9a-107">Permissions</span></span>

<span data-ttu-id="d0f9a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0f9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d0f9a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0f9a-110">Permission type</span></span>                        | <span data-ttu-id="d0f9a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0f9a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d0f9a-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0f9a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d0f9a-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0f9a-113">Reports.Read.All</span></span> |
| <span data-ttu-id="d0f9a-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0f9a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0f9a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-115">Not supported.</span></span> |
| <span data-ttu-id="d0f9a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0f9a-116">Application</span></span>                            | <span data-ttu-id="d0f9a-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0f9a-117">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0f9a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0f9a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/userCredentialUsageDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d0f9a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d0f9a-119">Optional query parameters</span></span>

<span data-ttu-id="d0f9a-120">Essa função suporta o parâmetro de consulta OData opcional **$Filter**.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-120">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="d0f9a-121">Você pode aplicar **$Filter** em uma ou mais das seguintes propriedades do recurso [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) .</span><span class="sxs-lookup"><span data-stu-id="d0f9a-121">You can apply **$filter** on one or more of the following properties of the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) resource.</span></span>

| <span data-ttu-id="d0f9a-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d0f9a-122">Properties</span></span> | <span data-ttu-id="d0f9a-123">Descrição e exemplo</span><span class="sxs-lookup"><span data-stu-id="d0f9a-123">Description and example</span></span> |
|:--------- |:----------- |
| <span data-ttu-id="d0f9a-124">apresentam</span><span class="sxs-lookup"><span data-stu-id="d0f9a-124">feature</span></span> | <span data-ttu-id="d0f9a-125">Filtra por tipo de dados de uso que você deseja (registro vs Reset).</span><span class="sxs-lookup"><span data-stu-id="d0f9a-125">Filter by type of usage data that you want (registration vs reset).</span></span> <span data-ttu-id="d0f9a-126">Por exemplo: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-126">For example: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="d0f9a-127">Operadores de filtro suportados: `eq`</span><span class="sxs-lookup"><span data-stu-id="d0f9a-127">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="d0f9a-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d0f9a-128">userDisplayName</span></span> | <span data-ttu-id="d0f9a-129">Filtrar por nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-129">Filter by user display name.</span></span> <span data-ttu-id="d0f9a-130">Por exemplo: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-130">For example: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="d0f9a-131">Operadores de filtro suportados: `eq` e `startswith()` .</span><span class="sxs-lookup"><span data-stu-id="d0f9a-131">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="d0f9a-132">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-132">Supports case insensitive.</span></span> |
| <span data-ttu-id="d0f9a-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d0f9a-133">userPrincipalName</span></span>  | <span data-ttu-id="d0f9a-134">Filtrar por nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-134">Filter by user principal name.</span></span> <span data-ttu-id="d0f9a-135">Por exemplo: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-135">For example: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span>    <span data-ttu-id="d0f9a-136">Operadores de filtro suportados: `eq` e `startswith()` .</span><span class="sxs-lookup"><span data-stu-id="d0f9a-136">Supported filter  operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="d0f9a-137">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-137">Supports case insensitive.</span></span> |
| <span data-ttu-id="d0f9a-138">IsSuccess</span><span class="sxs-lookup"><span data-stu-id="d0f9a-138">isSuccess</span></span> | <span data-ttu-id="d0f9a-139">Filtrar por status da atividade.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-139">Filter by status of the activity.</span></span> <span data-ttu-id="d0f9a-140">Por exemplo: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-140">For example: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span></span> <span data-ttu-id="d0f9a-141">Operadores de filtro suportados: `eq` e `orderby` .</span><span class="sxs-lookup"><span data-stu-id="d0f9a-141">Supported filter operators: `eq` and `orderby`.</span></span> |
| <span data-ttu-id="d0f9a-142">authMethod</span><span class="sxs-lookup"><span data-stu-id="d0f9a-142">authMethod</span></span>  | <span data-ttu-id="d0f9a-143">Filtrar pelos métodos de autenticação usando durante o registro.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-143">Filter by the authentication methods using during registration.</span></span> <span data-ttu-id="d0f9a-144">Por exemplo: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-144">For example: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span></span> <span data-ttu-id="d0f9a-145">Operadores de filtro suportados: `eq` .</span><span class="sxs-lookup"><span data-stu-id="d0f9a-145">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="d0f9a-146">failureReason</span><span class="sxs-lookup"><span data-stu-id="d0f9a-146">failureReason</span></span> | <span data-ttu-id="d0f9a-147">Filtrar por motivo da falha (se a atividade falhar).</span><span class="sxs-lookup"><span data-stu-id="d0f9a-147">Filter by failure reason (if the activity has failed).</span></span> <span data-ttu-id="d0f9a-148">Por exemplo: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-148">For example: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span></span> <span data-ttu-id="d0f9a-149">Operadores de filtro suportados: `eq` e `startswith()` .</span><span class="sxs-lookup"><span data-stu-id="d0f9a-149">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="d0f9a-150">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-150">Supports case insensitive.</span></span> |


## <a name="request-headers"></a><span data-ttu-id="d0f9a-151">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0f9a-151">Request headers</span></span>

| <span data-ttu-id="d0f9a-152">Nome</span><span class="sxs-lookup"><span data-stu-id="d0f9a-152">Name</span></span>      |<span data-ttu-id="d0f9a-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0f9a-153">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d0f9a-154">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0f9a-154">Authorization</span></span> | <span data-ttu-id="d0f9a-155">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="d0f9a-155">Bearer {token}</span></span> |
| <span data-ttu-id="d0f9a-156">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0f9a-156">Content-Type</span></span> | <span data-ttu-id="d0f9a-157">application/json</span><span class="sxs-lookup"><span data-stu-id="d0f9a-157">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0f9a-158">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0f9a-158">Request body</span></span>

<span data-ttu-id="d0f9a-159">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-159">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0f9a-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0f9a-160">Response</span></span>

<span data-ttu-id="d0f9a-161">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-161">If successful, this method returns a `200 OK` response code and a collection of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d0f9a-162">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d0f9a-162">Examples</span></span>

<span data-ttu-id="d0f9a-163">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-163">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d0f9a-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0f9a-164">Request</span></span>

<span data-ttu-id="d0f9a-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d0f9a-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0f9a-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```
# <a name="c"></a>[<span data-ttu-id="d0f9a-167">C#</span><span class="sxs-lookup"><span data-stu-id="d0f9a-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usercredentialusagedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0f9a-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0f9a-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usercredentialusagedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0f9a-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0f9a-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usercredentialusagedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0f9a-170">Java</span><span class="sxs-lookup"><span data-stu-id="d0f9a-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usercredentialusagedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d0f9a-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0f9a-171">Response</span></span>

<span data-ttu-id="d0f9a-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-172">The following is an example of the response.</span></span>

> <span data-ttu-id="d0f9a-173">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-173">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d0f9a-174">Todas as propriedades são retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0f9a-174">All the properties are returned from an actual call.</span></span>

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


