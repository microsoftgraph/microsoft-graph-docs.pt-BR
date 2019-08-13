---
title: Listar userCredentialUsageDetails
description: Obter uma lista de objetos userCredentialUsageDetails para um determinado locatário.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 60442e3fd4bfe8c1143b0560c80e827d8b8e518c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358290"
---
# <a name="list-usercredentialusagedetails"></a><span data-ttu-id="fa472-103">Listar userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="fa472-103">List userCredentialUsageDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa472-104">Obter uma lista de objetos [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) para um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="fa472-104">Get a list of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects for a given tenant.</span></span> <span data-ttu-id="fa472-105">Os detalhes incluem informações do usuário, status da redefinição e o motivo da falha.</span><span class="sxs-lookup"><span data-stu-id="fa472-105">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa472-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa472-106">Permissions</span></span>

<span data-ttu-id="fa472-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa472-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa472-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa472-109">Permission type</span></span>                        | <span data-ttu-id="fa472-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa472-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fa472-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa472-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa472-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa472-112">Reports.Read.All</span></span> |
| <span data-ttu-id="fa472-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa472-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa472-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa472-114">Not supported.</span></span> |
| <span data-ttu-id="fa472-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa472-115">Application</span></span>                            | <span data-ttu-id="fa472-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa472-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa472-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa472-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/userCredentialUsageDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa472-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fa472-118">Optional query parameters</span></span>

<span data-ttu-id="fa472-119">Essa função suporta o parâmetro de consulta OData opcional **$Filter**.</span><span class="sxs-lookup"><span data-stu-id="fa472-119">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="fa472-120">Você pode aplicar **$Filter** em uma ou mais das seguintes propriedades do recurso [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) .</span><span class="sxs-lookup"><span data-stu-id="fa472-120">You can apply **$filter** on one or more of the following properties of the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) resource.</span></span>

| <span data-ttu-id="fa472-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa472-121">Properties</span></span> | <span data-ttu-id="fa472-122">Descrição e exemplo</span><span class="sxs-lookup"><span data-stu-id="fa472-122">Description and example</span></span> |
|:--------- |:----------- |
| <span data-ttu-id="fa472-123">apresentam</span><span class="sxs-lookup"><span data-stu-id="fa472-123">feature</span></span> | <span data-ttu-id="fa472-124">Filtra por tipo de dados de uso que você deseja (registro vs Reset).</span><span class="sxs-lookup"><span data-stu-id="fa472-124">Filter by type of usage data that you want (registration vs reset).</span></span> <span data-ttu-id="fa472-125">Por exemplo: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span><span class="sxs-lookup"><span data-stu-id="fa472-125">For example: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="fa472-126">Operadores de filtro suportados:`eq`</span><span class="sxs-lookup"><span data-stu-id="fa472-126">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="fa472-127">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="fa472-127">userDisplayName</span></span> | <span data-ttu-id="fa472-128">Filtrar por nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="fa472-128">Filter by user display name.</span></span> <span data-ttu-id="fa472-129">Por exemplo: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="fa472-129">For example: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="fa472-130">Operadores de filtro suportados `eq` : `startswith()`e.</span><span class="sxs-lookup"><span data-stu-id="fa472-130">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="fa472-131">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="fa472-131">Supports case insensitive.</span></span> |
| <span data-ttu-id="fa472-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fa472-132">userPrincipalName</span></span>  | <span data-ttu-id="fa472-133">Filtrar por nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="fa472-133">Filter by user principal name.</span></span> <span data-ttu-id="fa472-134">Por exemplo: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="fa472-134">For example: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span>    <span data-ttu-id="fa472-135">Operadores de filtro suportados `eq` : `startswith()`e.</span><span class="sxs-lookup"><span data-stu-id="fa472-135">Supported filter  operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="fa472-136">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="fa472-136">Supports case insensitive.</span></span> |
| <span data-ttu-id="fa472-137">IsSuccess</span><span class="sxs-lookup"><span data-stu-id="fa472-137">isSuccess</span></span> | <span data-ttu-id="fa472-138">Filtrar por status da atividade.</span><span class="sxs-lookup"><span data-stu-id="fa472-138">Filter by status of the activity.</span></span> <span data-ttu-id="fa472-139">Por exemplo: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span><span class="sxs-lookup"><span data-stu-id="fa472-139">For example: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span></span> <span data-ttu-id="fa472-140">Operadores de filtro suportados `eq` : `orderby`e.</span><span class="sxs-lookup"><span data-stu-id="fa472-140">Supported filter operators: `eq` and `orderby`.</span></span> |
| <span data-ttu-id="fa472-141">authMethod</span><span class="sxs-lookup"><span data-stu-id="fa472-141">authMethod</span></span>  | <span data-ttu-id="fa472-142">Filtrar pelos métodos de autenticação usando durante o registro.</span><span class="sxs-lookup"><span data-stu-id="fa472-142">Filter by the authentication methods using during registration.</span></span> <span data-ttu-id="fa472-143">Por exemplo: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span><span class="sxs-lookup"><span data-stu-id="fa472-143">For example: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span></span> <span data-ttu-id="fa472-144">Operadores de filtro suportados `eq`:.</span><span class="sxs-lookup"><span data-stu-id="fa472-144">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="fa472-145">failureReason</span><span class="sxs-lookup"><span data-stu-id="fa472-145">failureReason</span></span> | <span data-ttu-id="fa472-146">Filtrar por motivo da falha (se a atividade falhar).</span><span class="sxs-lookup"><span data-stu-id="fa472-146">Filter by failure reason (if the activity has failed).</span></span> <span data-ttu-id="fa472-147">Por exemplo: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="fa472-147">For example: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span></span> <span data-ttu-id="fa472-148">Operadores de filtro suportados `eq` : `startswith()`e.</span><span class="sxs-lookup"><span data-stu-id="fa472-148">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="fa472-149">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="fa472-149">Supports case insensitive.</span></span> |


## <a name="request-headers"></a><span data-ttu-id="fa472-150">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa472-150">Request headers</span></span>

| <span data-ttu-id="fa472-151">Nome</span><span class="sxs-lookup"><span data-stu-id="fa472-151">Name</span></span>      |<span data-ttu-id="fa472-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa472-152">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fa472-153">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa472-153">Authorization</span></span> | <span data-ttu-id="fa472-154">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="fa472-154">Bearer {token}</span></span> |
| <span data-ttu-id="fa472-155">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa472-155">Content-Type</span></span> | <span data-ttu-id="fa472-156">application/json</span><span class="sxs-lookup"><span data-stu-id="fa472-156">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa472-157">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa472-157">Request body</span></span>

<span data-ttu-id="fa472-158">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa472-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa472-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa472-159">Response</span></span>

<span data-ttu-id="fa472-160">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa472-160">If successful, this method returns a `200 OK` response code and a collection of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa472-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fa472-161">Examples</span></span>

<span data-ttu-id="fa472-162">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="fa472-162">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="fa472-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa472-163">Request</span></span>

<span data-ttu-id="fa472-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa472-164">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fa472-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa472-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}-->

```http
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa472-166">C#</span><span class="sxs-lookup"><span data-stu-id="fa472-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usercredentialusagedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa472-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa472-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usercredentialusagedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa472-168">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fa472-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usercredentialusagedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fa472-169">Java</span><span class="sxs-lookup"><span data-stu-id="fa472-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usercredentialusagedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fa472-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa472-170">Response</span></span>

<span data-ttu-id="fa472-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fa472-171">The following is an example of the response.</span></span>

> <span data-ttu-id="fa472-172">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fa472-172">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fa472-173">Todas as propriedades são retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa472-173">All the properties are returned from an actual call.</span></span>

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
