---
title: Listar userCredentialUsageDetails
description: Obter uma lista de objetos userCredentialUsageDetails para um determinado locatário.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 17e273395e9ae2aa7dd46611f9843359f8456aa3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453912"
---
# <a name="list-usercredentialusagedetails"></a><span data-ttu-id="d522b-103">Listar userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="d522b-103">List userCredentialUsageDetails</span></span>

<span data-ttu-id="d522b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d522b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d522b-105">Obter uma lista de objetos [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) para um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="d522b-105">Get a list of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects for a given tenant.</span></span> <span data-ttu-id="d522b-106">Os detalhes incluem informações do usuário, status da redefinição e o motivo da falha.</span><span class="sxs-lookup"><span data-stu-id="d522b-106">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="permissions"></a><span data-ttu-id="d522b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d522b-107">Permissions</span></span>

<span data-ttu-id="d522b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d522b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d522b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d522b-110">Permission type</span></span>                        | <span data-ttu-id="d522b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d522b-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d522b-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d522b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d522b-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d522b-113">Reports.Read.All</span></span> |
| <span data-ttu-id="d522b-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d522b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d522b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d522b-115">Not supported.</span></span> |
| <span data-ttu-id="d522b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d522b-116">Application</span></span>                            | <span data-ttu-id="d522b-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d522b-117">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d522b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d522b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/userCredentialUsageDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d522b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d522b-119">Optional query parameters</span></span>

<span data-ttu-id="d522b-120">Essa função suporta o parâmetro de consulta OData opcional **$Filter**.</span><span class="sxs-lookup"><span data-stu-id="d522b-120">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="d522b-121">Você pode aplicar **$Filter** em uma ou mais das seguintes propriedades do recurso [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) .</span><span class="sxs-lookup"><span data-stu-id="d522b-121">You can apply **$filter** on one or more of the following properties of the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) resource.</span></span>

| <span data-ttu-id="d522b-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d522b-122">Properties</span></span> | <span data-ttu-id="d522b-123">Descrição e exemplo</span><span class="sxs-lookup"><span data-stu-id="d522b-123">Description and example</span></span> |
|:--------- |:----------- |
| <span data-ttu-id="d522b-124">apresentam</span><span class="sxs-lookup"><span data-stu-id="d522b-124">feature</span></span> | <span data-ttu-id="d522b-125">Filtra por tipo de dados de uso que você deseja (registro vs Reset).</span><span class="sxs-lookup"><span data-stu-id="d522b-125">Filter by type of usage data that you want (registration vs reset).</span></span> <span data-ttu-id="d522b-126">Por exemplo: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span><span class="sxs-lookup"><span data-stu-id="d522b-126">For example: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="d522b-127">Operadores de filtro suportados:`eq`</span><span class="sxs-lookup"><span data-stu-id="d522b-127">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="d522b-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d522b-128">userDisplayName</span></span> | <span data-ttu-id="d522b-129">Filtrar por nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="d522b-129">Filter by user display name.</span></span> <span data-ttu-id="d522b-130">Por exemplo: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="d522b-130">For example: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="d522b-131">Operadores de filtro suportados `eq` : `startswith()`e.</span><span class="sxs-lookup"><span data-stu-id="d522b-131">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="d522b-132">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d522b-132">Supports case insensitive.</span></span> |
| <span data-ttu-id="d522b-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d522b-133">userPrincipalName</span></span>  | <span data-ttu-id="d522b-134">Filtrar por nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="d522b-134">Filter by user principal name.</span></span> <span data-ttu-id="d522b-135">Por exemplo: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="d522b-135">For example: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span>    <span data-ttu-id="d522b-136">Operadores de filtro suportados `eq` : `startswith()`e.</span><span class="sxs-lookup"><span data-stu-id="d522b-136">Supported filter  operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="d522b-137">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d522b-137">Supports case insensitive.</span></span> |
| <span data-ttu-id="d522b-138">IsSuccess</span><span class="sxs-lookup"><span data-stu-id="d522b-138">isSuccess</span></span> | <span data-ttu-id="d522b-139">Filtrar por status da atividade.</span><span class="sxs-lookup"><span data-stu-id="d522b-139">Filter by status of the activity.</span></span> <span data-ttu-id="d522b-140">Por exemplo: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span><span class="sxs-lookup"><span data-stu-id="d522b-140">For example: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span></span> <span data-ttu-id="d522b-141">Operadores de filtro suportados `eq` : `orderby`e.</span><span class="sxs-lookup"><span data-stu-id="d522b-141">Supported filter operators: `eq` and `orderby`.</span></span> |
| <span data-ttu-id="d522b-142">authMethod</span><span class="sxs-lookup"><span data-stu-id="d522b-142">authMethod</span></span>  | <span data-ttu-id="d522b-143">Filtrar pelos métodos de autenticação usando durante o registro.</span><span class="sxs-lookup"><span data-stu-id="d522b-143">Filter by the authentication methods using during registration.</span></span> <span data-ttu-id="d522b-144">Por exemplo: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span><span class="sxs-lookup"><span data-stu-id="d522b-144">For example: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span></span> <span data-ttu-id="d522b-145">Operadores de filtro suportados `eq`:.</span><span class="sxs-lookup"><span data-stu-id="d522b-145">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="d522b-146">failureReason</span><span class="sxs-lookup"><span data-stu-id="d522b-146">failureReason</span></span> | <span data-ttu-id="d522b-147">Filtrar por motivo da falha (se a atividade falhar).</span><span class="sxs-lookup"><span data-stu-id="d522b-147">Filter by failure reason (if the activity has failed).</span></span> <span data-ttu-id="d522b-148">Por exemplo: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="d522b-148">For example: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span></span> <span data-ttu-id="d522b-149">Operadores de filtro suportados `eq` : `startswith()`e.</span><span class="sxs-lookup"><span data-stu-id="d522b-149">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="d522b-150">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d522b-150">Supports case insensitive.</span></span> |


## <a name="request-headers"></a><span data-ttu-id="d522b-151">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d522b-151">Request headers</span></span>

| <span data-ttu-id="d522b-152">Nome</span><span class="sxs-lookup"><span data-stu-id="d522b-152">Name</span></span>      |<span data-ttu-id="d522b-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="d522b-153">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d522b-154">Autorização</span><span class="sxs-lookup"><span data-stu-id="d522b-154">Authorization</span></span> | <span data-ttu-id="d522b-155">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="d522b-155">Bearer {token}</span></span> |
| <span data-ttu-id="d522b-156">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d522b-156">Content-Type</span></span> | <span data-ttu-id="d522b-157">application/json</span><span class="sxs-lookup"><span data-stu-id="d522b-157">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d522b-158">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d522b-158">Request body</span></span>

<span data-ttu-id="d522b-159">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d522b-159">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d522b-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="d522b-160">Response</span></span>

<span data-ttu-id="d522b-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d522b-161">If successful, this method returns a `200 OK` response code and a collection of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d522b-162">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d522b-162">Examples</span></span>

<span data-ttu-id="d522b-163">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d522b-163">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d522b-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d522b-164">Request</span></span>

<span data-ttu-id="d522b-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d522b-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d522b-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="d522b-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```
# <a name="c"></a>[<span data-ttu-id="d522b-167">C#</span><span class="sxs-lookup"><span data-stu-id="d522b-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usercredentialusagedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d522b-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d522b-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usercredentialusagedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d522b-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d522b-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usercredentialusagedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d522b-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="d522b-170">Response</span></span>

<span data-ttu-id="d522b-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d522b-171">The following is an example of the response.</span></span>

> <span data-ttu-id="d522b-172">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d522b-172">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d522b-173">Todas as propriedades são retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d522b-173">All the properties are returned from an actual call.</span></span>

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
