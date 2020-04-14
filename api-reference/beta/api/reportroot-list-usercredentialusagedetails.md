---
title: Listar userCredentialUsageDetails
description: Obter uma lista de objetos userCredentialUsageDetails para um determinado locatário.
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: df98f62df4465c43dede5f6cd293145b6c644e94
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43386553"
---
# <a name="list-usercredentialusagedetails"></a><span data-ttu-id="fd99f-103">Listar userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="fd99f-103">List userCredentialUsageDetails</span></span>

<span data-ttu-id="fd99f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd99f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd99f-105">Obter uma lista de objetos [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) para um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="fd99f-105">Get a list of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects for a given tenant.</span></span> <span data-ttu-id="fd99f-106">Os detalhes incluem informações do usuário, status da redefinição e o motivo da falha.</span><span class="sxs-lookup"><span data-stu-id="fd99f-106">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd99f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fd99f-107">Permissions</span></span>

<span data-ttu-id="fd99f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd99f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fd99f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd99f-110">Permission type</span></span>                        | <span data-ttu-id="fd99f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fd99f-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fd99f-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd99f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fd99f-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd99f-113">Reports.Read.All</span></span> |
| <span data-ttu-id="fd99f-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd99f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd99f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd99f-115">Not supported.</span></span> |
| <span data-ttu-id="fd99f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd99f-116">Application</span></span>                            | <span data-ttu-id="fd99f-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd99f-117">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd99f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd99f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/userCredentialUsageDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd99f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fd99f-119">Optional query parameters</span></span>

<span data-ttu-id="fd99f-120">Essa função suporta o parâmetro de consulta OData opcional **$Filter**.</span><span class="sxs-lookup"><span data-stu-id="fd99f-120">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="fd99f-121">Você pode aplicar **$Filter** em uma ou mais das seguintes propriedades do recurso [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) .</span><span class="sxs-lookup"><span data-stu-id="fd99f-121">You can apply **$filter** on one or more of the following properties of the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) resource.</span></span>

| <span data-ttu-id="fd99f-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd99f-122">Properties</span></span> | <span data-ttu-id="fd99f-123">Descrição e exemplo</span><span class="sxs-lookup"><span data-stu-id="fd99f-123">Description and example</span></span> |
|:--------- |:----------- |
| <span data-ttu-id="fd99f-124">apresentam</span><span class="sxs-lookup"><span data-stu-id="fd99f-124">feature</span></span> | <span data-ttu-id="fd99f-125">Filtra por tipo de dados de uso que você deseja (registro vs Reset).</span><span class="sxs-lookup"><span data-stu-id="fd99f-125">Filter by type of usage data that you want (registration vs reset).</span></span> <span data-ttu-id="fd99f-126">Por exemplo: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span><span class="sxs-lookup"><span data-stu-id="fd99f-126">For example: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="fd99f-127">Operadores de filtro suportados:`eq`</span><span class="sxs-lookup"><span data-stu-id="fd99f-127">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="fd99f-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="fd99f-128">userDisplayName</span></span> | <span data-ttu-id="fd99f-129">Filtrar por nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="fd99f-129">Filter by user display name.</span></span> <span data-ttu-id="fd99f-130">Por exemplo: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="fd99f-130">For example: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="fd99f-131">Operadores de filtro suportados `eq` : `startswith()`e.</span><span class="sxs-lookup"><span data-stu-id="fd99f-131">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="fd99f-132">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="fd99f-132">Supports case insensitive.</span></span> |
| <span data-ttu-id="fd99f-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fd99f-133">userPrincipalName</span></span>  | <span data-ttu-id="fd99f-134">Filtrar por nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="fd99f-134">Filter by user principal name.</span></span> <span data-ttu-id="fd99f-135">Por exemplo: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="fd99f-135">For example: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span>    <span data-ttu-id="fd99f-136">Operadores de filtro suportados `eq` : `startswith()`e.</span><span class="sxs-lookup"><span data-stu-id="fd99f-136">Supported filter  operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="fd99f-137">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="fd99f-137">Supports case insensitive.</span></span> |
| <span data-ttu-id="fd99f-138">IsSuccess</span><span class="sxs-lookup"><span data-stu-id="fd99f-138">isSuccess</span></span> | <span data-ttu-id="fd99f-139">Filtrar por status da atividade.</span><span class="sxs-lookup"><span data-stu-id="fd99f-139">Filter by status of the activity.</span></span> <span data-ttu-id="fd99f-140">Por exemplo: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span><span class="sxs-lookup"><span data-stu-id="fd99f-140">For example: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span></span> <span data-ttu-id="fd99f-141">Operadores de filtro suportados `eq` : `orderby`e.</span><span class="sxs-lookup"><span data-stu-id="fd99f-141">Supported filter operators: `eq` and `orderby`.</span></span> |
| <span data-ttu-id="fd99f-142">authMethod</span><span class="sxs-lookup"><span data-stu-id="fd99f-142">authMethod</span></span>  | <span data-ttu-id="fd99f-143">Filtrar pelos métodos de autenticação usando durante o registro.</span><span class="sxs-lookup"><span data-stu-id="fd99f-143">Filter by the authentication methods using during registration.</span></span> <span data-ttu-id="fd99f-144">Por exemplo: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span><span class="sxs-lookup"><span data-stu-id="fd99f-144">For example: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span></span> <span data-ttu-id="fd99f-145">Operadores de filtro suportados `eq`:.</span><span class="sxs-lookup"><span data-stu-id="fd99f-145">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="fd99f-146">failureReason</span><span class="sxs-lookup"><span data-stu-id="fd99f-146">failureReason</span></span> | <span data-ttu-id="fd99f-147">Filtrar por motivo da falha (se a atividade falhar).</span><span class="sxs-lookup"><span data-stu-id="fd99f-147">Filter by failure reason (if the activity has failed).</span></span> <span data-ttu-id="fd99f-148">Por exemplo: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="fd99f-148">For example: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span></span> <span data-ttu-id="fd99f-149">Operadores de filtro suportados `eq` : `startswith()`e.</span><span class="sxs-lookup"><span data-stu-id="fd99f-149">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="fd99f-150">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="fd99f-150">Supports case insensitive.</span></span> |


## <a name="request-headers"></a><span data-ttu-id="fd99f-151">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd99f-151">Request headers</span></span>

| <span data-ttu-id="fd99f-152">Nome</span><span class="sxs-lookup"><span data-stu-id="fd99f-152">Name</span></span>      |<span data-ttu-id="fd99f-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd99f-153">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fd99f-154">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd99f-154">Authorization</span></span> | <span data-ttu-id="fd99f-155">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="fd99f-155">Bearer {token}</span></span> |
| <span data-ttu-id="fd99f-156">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd99f-156">Content-Type</span></span> | <span data-ttu-id="fd99f-157">application/json</span><span class="sxs-lookup"><span data-stu-id="fd99f-157">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd99f-158">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd99f-158">Request body</span></span>

<span data-ttu-id="fd99f-159">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fd99f-159">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd99f-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd99f-160">Response</span></span>

<span data-ttu-id="fd99f-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd99f-161">If successful, this method returns a `200 OK` response code and a collection of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fd99f-162">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fd99f-162">Examples</span></span>

<span data-ttu-id="fd99f-163">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="fd99f-163">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="fd99f-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd99f-164">Request</span></span>

<span data-ttu-id="fd99f-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd99f-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fd99f-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd99f-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```
# <a name="c"></a>[<span data-ttu-id="fd99f-167">C#</span><span class="sxs-lookup"><span data-stu-id="fd99f-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usercredentialusagedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fd99f-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd99f-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usercredentialusagedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd99f-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd99f-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usercredentialusagedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fd99f-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd99f-170">Response</span></span>

<span data-ttu-id="fd99f-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fd99f-171">The following is an example of the response.</span></span>

> <span data-ttu-id="fd99f-172">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fd99f-172">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fd99f-173">Todas as propriedades são retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd99f-173">All the properties are returned from an actual call.</span></span>

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
