---
title: Listar credentialUserRegistrationDetails
description: Obter uma lista de objetos credentialUserRegistrationDetails para um determinado locatário.
localization_priority: Normal
author: besiler
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: d37e7f568424854ddb3dd9f96ea14f5be7a61999
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523861"
---
# <a name="list-credentialuserregistrationdetails"></a><span data-ttu-id="9349c-103">Listar credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="9349c-103">List credentialUserRegistrationDetails</span></span>

<span data-ttu-id="9349c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9349c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9349c-105">Obter uma lista de objetos [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) para um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="9349c-105">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="9349c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9349c-106">Permissions</span></span>

<span data-ttu-id="9349c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9349c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9349c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9349c-109">Permission type</span></span>                        | <span data-ttu-id="9349c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9349c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9349c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9349c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9349c-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9349c-112">Reports.Read.All</span></span> |
| <span data-ttu-id="9349c-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9349c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9349c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9349c-114">Not supported.</span></span> |
| <span data-ttu-id="9349c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9349c-115">Application</span></span>                            | <span data-ttu-id="9349c-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9349c-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9349c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9349c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/credentialUserRegistrationDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9349c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9349c-118">Optional query parameters</span></span>

<span data-ttu-id="9349c-119">Essa função suporta o parâmetro de consulta OData opcional **$Filter**.</span><span class="sxs-lookup"><span data-stu-id="9349c-119">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="9349c-120">Você pode aplicar **$Filter** em uma ou mais das seguintes propriedades do recurso [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="9349c-120">You can apply **$filter** on one or more of the following properties of the [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) resource.</span></span>

| <span data-ttu-id="9349c-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9349c-121">Properties</span></span> | <span data-ttu-id="9349c-122">Descrição e exemplo</span><span class="sxs-lookup"><span data-stu-id="9349c-122">Description and example</span></span> |
| --------- | ----------------------- |
| <span data-ttu-id="9349c-123">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="9349c-123">userDisplayName</span></span> | <span data-ttu-id="9349c-124">Filtrar por nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="9349c-124">Filter by user name.</span></span> <span data-ttu-id="9349c-125">Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=userDisplayName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="9349c-125">For example: `/reports/credentialUserRegistrationDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="9349c-126">Operadores de filtro suportados: `eq` , e `startswith()` .</span><span class="sxs-lookup"><span data-stu-id="9349c-126">Supported filter operators: `eq`, and `startswith()`.</span></span> <span data-ttu-id="9349c-127">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9349c-127">Supports case insensitive.</span></span> |
| <span data-ttu-id="9349c-128">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9349c-128">userPrincipalName</span></span> | <span data-ttu-id="9349c-129">Filtrar por nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="9349c-129">Filter by user principal name.</span></span> <span data-ttu-id="9349c-130">Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=userPrincipalName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="9349c-130">For example: `/reports/credentialUserRegistrationDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span> <span data-ttu-id="9349c-131">Operadores de filtro suportados: `eq` e `startswith()` .</span><span class="sxs-lookup"><span data-stu-id="9349c-131">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="9349c-132">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9349c-132">Supports case insensitive.</span></span> |
| <span data-ttu-id="9349c-133">authMethods</span><span class="sxs-lookup"><span data-stu-id="9349c-133">authMethods</span></span> | <span data-ttu-id="9349c-134">Filtrar pelos métodos de autenticação usados durante o registro.</span><span class="sxs-lookup"><span data-stu-id="9349c-134">Filter by the authentication methods used during registration.</span></span> <span data-ttu-id="9349c-135">Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`.</span><span class="sxs-lookup"><span data-stu-id="9349c-135">For example: `/reports/credentialUserRegistrationDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`.</span></span> <span data-ttu-id="9349c-136">Operadores de filtro suportados: `eq` .</span><span class="sxs-lookup"><span data-stu-id="9349c-136">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="9349c-137">IsRegistered</span><span class="sxs-lookup"><span data-stu-id="9349c-137">isRegistered</span></span> | <span data-ttu-id="9349c-138">Filtro para usuários que registraram a redefinição de senha de autoatendimento (SSPR).</span><span class="sxs-lookup"><span data-stu-id="9349c-138">Filter for users who have registered for self-service password reset (SSPR).</span></span> <span data-ttu-id="9349c-139">Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=isRegistered eq true`.</span><span class="sxs-lookup"><span data-stu-id="9349c-139">For example: `/reports/credentialUserRegistrationDetails?$filter=isRegistered eq true`.</span></span> <span data-ttu-id="9349c-140">Operadores de filtro suportados: `eq` .</span><span class="sxs-lookup"><span data-stu-id="9349c-140">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="9349c-141">isEnabled</span><span class="sxs-lookup"><span data-stu-id="9349c-141">isEnabled</span></span> | <span data-ttu-id="9349c-142">Filtro para usuários que foram habilitados para o SSPR.</span><span class="sxs-lookup"><span data-stu-id="9349c-142">Filter for users who have been enabled for SSPR.</span></span> <span data-ttu-id="9349c-143">Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=isEnabled eq true`.</span><span class="sxs-lookup"><span data-stu-id="9349c-143">For example: `/reports/credentialUserRegistrationDetails?$filter=isEnabled eq true`.</span></span> <span data-ttu-id="9349c-144">Operadores filtter com suporte: `eq` .</span><span class="sxs-lookup"><span data-stu-id="9349c-144">Supported filtter operators: `eq`.</span></span> |
| <span data-ttu-id="9349c-145">iscapable</span><span class="sxs-lookup"><span data-stu-id="9349c-145">isCapable</span></span> | <span data-ttu-id="9349c-146">Filtro para usuários que estão prontos para executar redefinição de senha ou a autenticação multifator (MFA).</span><span class="sxs-lookup"><span data-stu-id="9349c-146">Filter for users who are ready to perform password reset or multi-factor authentication (MFA).</span></span> <span data-ttu-id="9349c-147">Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=isCapable eq true`.</span><span class="sxs-lookup"><span data-stu-id="9349c-147">For example: `/reports/credentialUserRegistrationDetails?$filter=isCapable eq true`.</span></span> <span data-ttu-id="9349c-148">Operadores de filtro suportados: `eq`</span><span class="sxs-lookup"><span data-stu-id="9349c-148">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="9349c-149">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="9349c-149">isMfaRegistered</span></span> | <span data-ttu-id="9349c-150">Filtro para usuários registrados para MFA.</span><span class="sxs-lookup"><span data-stu-id="9349c-150">Filter for users who are registered for MFA.</span></span> <span data-ttu-id="9349c-151">Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=isMfaRegistered eq true`.</span><span class="sxs-lookup"><span data-stu-id="9349c-151">For example: `/reports/credentialUserRegistrationDetails?$filter=isMfaRegistered eq true`.</span></span> <span data-ttu-id="9349c-152">Operadores de filtro suportados: `eq` .</span><span class="sxs-lookup"><span data-stu-id="9349c-152">Supported filter operators: `eq`.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9349c-153">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9349c-153">Request headers</span></span>

| <span data-ttu-id="9349c-154">Nome</span><span class="sxs-lookup"><span data-stu-id="9349c-154">Name</span></span>      |<span data-ttu-id="9349c-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="9349c-155">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9349c-156">Autorização</span><span class="sxs-lookup"><span data-stu-id="9349c-156">Authorization</span></span> | <span data-ttu-id="9349c-157">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="9349c-157">Bearer {token}</span></span> |
| <span data-ttu-id="9349c-158">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9349c-158">Content-Type</span></span> | <span data-ttu-id="9349c-159">application/json</span><span class="sxs-lookup"><span data-stu-id="9349c-159">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9349c-160">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9349c-160">Request body</span></span>

<span data-ttu-id="9349c-161">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9349c-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9349c-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="9349c-162">Response</span></span>

<span data-ttu-id="9349c-163">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9349c-163">If successful, this method returns a `200 OK` response code and a collection of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9349c-164">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9349c-164">Examples</span></span>

<span data-ttu-id="9349c-165">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="9349c-165">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="9349c-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9349c-166">Request</span></span>

<span data-ttu-id="9349c-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9349c-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9349c-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="9349c-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
```
# <a name="c"></a>[<span data-ttu-id="9349c-169">C#</span><span class="sxs-lookup"><span data-stu-id="9349c-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-credentialuserregistrationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9349c-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9349c-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-credentialuserregistrationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9349c-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9349c-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-credentialuserregistrationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9349c-172">Java</span><span class="sxs-lookup"><span data-stu-id="9349c-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-credentialuserregistrationdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9349c-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="9349c-173">Response</span></span>

<span data-ttu-id="9349c-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9349c-174">The following is an example of the response.</span></span>

> <span data-ttu-id="9349c-175">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9349c-175">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9349c-176">Todas as propriedades são retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9349c-176">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.credentialUserRegistrationDetails)",
  "value":[
    {
      "id" : "id-value",
      "userPrincipalName":"userPrincipalName",
      "userDisplayName": "userDisplayName-value",
      "authMethods": ["email", "mobileSMS"],
      "isRegistered" : false,
      "isEnabled" : true,
      "isCapable" : false,
      "isMfaRegistered" : true
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List credentialUserRegistrationDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


