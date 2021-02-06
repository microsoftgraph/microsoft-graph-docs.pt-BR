---
title: Listar credentialUserRegistrationDetails
description: Obter uma lista de objetos credentialUserRegistrationDetails para um determinado locatário.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: bf6e99722c44ff0054869056be09314d6befac59
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136665"
---
# <a name="list-credentialuserregistrationdetails"></a><span data-ttu-id="044d1-103">Listar credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="044d1-103">List credentialUserRegistrationDetails</span></span>

<span data-ttu-id="044d1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="044d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="044d1-105">Obter uma lista de [objetos credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) para um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="044d1-105">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="044d1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="044d1-106">Permissions</span></span>

<span data-ttu-id="044d1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="044d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="044d1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="044d1-109">Permission type</span></span>                        | <span data-ttu-id="044d1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="044d1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="044d1-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="044d1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="044d1-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="044d1-112">Reports.Read.All</span></span> |
| <span data-ttu-id="044d1-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="044d1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="044d1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="044d1-114">Not supported.</span></span> |
| <span data-ttu-id="044d1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="044d1-115">Application</span></span>                            | <span data-ttu-id="044d1-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="044d1-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="044d1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="044d1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/credentialUserRegistrationDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="044d1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="044d1-118">Optional query parameters</span></span>

<span data-ttu-id="044d1-119">Esta função dá suporte ao parâmetro opcional de consulta OData **$filter**.</span><span class="sxs-lookup"><span data-stu-id="044d1-119">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="044d1-120">Você pode aplicar **$filter** em uma ou mais das seguintes propriedades do [recurso credentialUserRegistrationDetails.](../resources/credentialuserregistrationdetails.md)</span><span class="sxs-lookup"><span data-stu-id="044d1-120">You can apply **$filter** on one or more of the following properties of the [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) resource.</span></span>

| <span data-ttu-id="044d1-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="044d1-121">Properties</span></span> | <span data-ttu-id="044d1-122">Descrição e exemplo</span><span class="sxs-lookup"><span data-stu-id="044d1-122">Description and example</span></span> |
| --------- | ----------------------- |
| <span data-ttu-id="044d1-123">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="044d1-123">userDisplayName</span></span> | <span data-ttu-id="044d1-124">Filtrar por nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="044d1-124">Filter by user name.</span></span> <span data-ttu-id="044d1-125">Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=userDisplayName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="044d1-125">For example: `/reports/credentialUserRegistrationDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="044d1-126">Operadores de filtro com suporte: `eq` e `startswith()` .</span><span class="sxs-lookup"><span data-stu-id="044d1-126">Supported filter operators: `eq`, and `startswith()`.</span></span> <span data-ttu-id="044d1-127">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="044d1-127">Supports case insensitive.</span></span> |
| <span data-ttu-id="044d1-128">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="044d1-128">userPrincipalName</span></span> | <span data-ttu-id="044d1-129">Filtrar pelo nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="044d1-129">Filter by user principal name.</span></span> <span data-ttu-id="044d1-130">Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=userPrincipalName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="044d1-130">For example: `/reports/credentialUserRegistrationDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span> <span data-ttu-id="044d1-131">Operadores de filtro com suporte: `eq` e `startswith()` .</span><span class="sxs-lookup"><span data-stu-id="044d1-131">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="044d1-132">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="044d1-132">Supports case insensitive.</span></span> |
| <span data-ttu-id="044d1-133">authMethods</span><span class="sxs-lookup"><span data-stu-id="044d1-133">authMethods</span></span> | <span data-ttu-id="044d1-134">Filtrar pelos métodos de autenticação usados durante o registro.</span><span class="sxs-lookup"><span data-stu-id="044d1-134">Filter by the authentication methods used during registration.</span></span> <span data-ttu-id="044d1-135">Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`.</span><span class="sxs-lookup"><span data-stu-id="044d1-135">For example: `/reports/credentialUserRegistrationDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`.</span></span> <span data-ttu-id="044d1-136">Operadores de filtro com suporte: `eq` .</span><span class="sxs-lookup"><span data-stu-id="044d1-136">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="044d1-137">isRegistered</span><span class="sxs-lookup"><span data-stu-id="044d1-137">isRegistered</span></span> | <span data-ttu-id="044d1-138">Filtro para usuários que se registraram para redefinição de senha de autoatendado (SSPR).</span><span class="sxs-lookup"><span data-stu-id="044d1-138">Filter for users who have registered for self-service password reset (SSPR).</span></span> <span data-ttu-id="044d1-139">Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=isRegistered eq true`.</span><span class="sxs-lookup"><span data-stu-id="044d1-139">For example: `/reports/credentialUserRegistrationDetails?$filter=isRegistered eq true`.</span></span> <span data-ttu-id="044d1-140">Operadores de filtro com suporte: `eq` .</span><span class="sxs-lookup"><span data-stu-id="044d1-140">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="044d1-141">isEnabled</span><span class="sxs-lookup"><span data-stu-id="044d1-141">isEnabled</span></span> | <span data-ttu-id="044d1-142">Filtro para usuários que foram habilitados para SSPR.</span><span class="sxs-lookup"><span data-stu-id="044d1-142">Filter for users who have been enabled for SSPR.</span></span> <span data-ttu-id="044d1-143">Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=isEnabled eq true`.</span><span class="sxs-lookup"><span data-stu-id="044d1-143">For example: `/reports/credentialUserRegistrationDetails?$filter=isEnabled eq true`.</span></span> <span data-ttu-id="044d1-144">Operadores de filtter com suporte: `eq` .</span><span class="sxs-lookup"><span data-stu-id="044d1-144">Supported filtter operators: `eq`.</span></span> |
| <span data-ttu-id="044d1-145">isCapable</span><span class="sxs-lookup"><span data-stu-id="044d1-145">isCapable</span></span> | <span data-ttu-id="044d1-146">Filtro para usuários que estão prontos para executar a redefinição de senha ou autenticação multifatória (MFA).</span><span class="sxs-lookup"><span data-stu-id="044d1-146">Filter for users who are ready to perform password reset or multi-factor authentication (MFA).</span></span> <span data-ttu-id="044d1-147">Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=isCapable eq true`.</span><span class="sxs-lookup"><span data-stu-id="044d1-147">For example: `/reports/credentialUserRegistrationDetails?$filter=isCapable eq true`.</span></span> <span data-ttu-id="044d1-148">Operadores de filtro com suporte: `eq`</span><span class="sxs-lookup"><span data-stu-id="044d1-148">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="044d1-149">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="044d1-149">isMfaRegistered</span></span> | <span data-ttu-id="044d1-150">Filtro para usuários que estão registrados para MFA.</span><span class="sxs-lookup"><span data-stu-id="044d1-150">Filter for users who are registered for MFA.</span></span> <span data-ttu-id="044d1-151">Por exemplo: `/reports/credentialUserRegistrationDetails?$filter=isMfaRegistered eq true`.</span><span class="sxs-lookup"><span data-stu-id="044d1-151">For example: `/reports/credentialUserRegistrationDetails?$filter=isMfaRegistered eq true`.</span></span> <span data-ttu-id="044d1-152">Operadores de filtro com suporte: `eq` .</span><span class="sxs-lookup"><span data-stu-id="044d1-152">Supported filter operators: `eq`.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="044d1-153">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="044d1-153">Request headers</span></span>

| <span data-ttu-id="044d1-154">Nome</span><span class="sxs-lookup"><span data-stu-id="044d1-154">Name</span></span>      |<span data-ttu-id="044d1-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="044d1-155">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="044d1-156">Autorização</span><span class="sxs-lookup"><span data-stu-id="044d1-156">Authorization</span></span> | <span data-ttu-id="044d1-157">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="044d1-157">Bearer {token}</span></span> |
| <span data-ttu-id="044d1-158">Content-Type</span><span class="sxs-lookup"><span data-stu-id="044d1-158">Content-Type</span></span> | <span data-ttu-id="044d1-159">application/json</span><span class="sxs-lookup"><span data-stu-id="044d1-159">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="044d1-160">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="044d1-160">Request body</span></span>

<span data-ttu-id="044d1-161">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="044d1-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="044d1-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="044d1-162">Response</span></span>

<span data-ttu-id="044d1-163">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="044d1-163">If successful, this method returns a `200 OK` response code and a collection of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="044d1-164">Exemplos</span><span class="sxs-lookup"><span data-stu-id="044d1-164">Examples</span></span>

<span data-ttu-id="044d1-165">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="044d1-165">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="044d1-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="044d1-166">Request</span></span>

<span data-ttu-id="044d1-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="044d1-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="044d1-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="044d1-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
```
# <a name="c"></a>[<span data-ttu-id="044d1-169">C#</span><span class="sxs-lookup"><span data-stu-id="044d1-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-credentialuserregistrationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="044d1-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="044d1-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-credentialuserregistrationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="044d1-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="044d1-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-credentialuserregistrationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="044d1-172">Java</span><span class="sxs-lookup"><span data-stu-id="044d1-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-credentialuserregistrationdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="044d1-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="044d1-173">Response</span></span>

<span data-ttu-id="044d1-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="044d1-174">The following is an example of the response.</span></span>

> <span data-ttu-id="044d1-175">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="044d1-175">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="044d1-176">Todas as propriedades são retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="044d1-176">All the properties are returned from an actual call.</span></span>

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


