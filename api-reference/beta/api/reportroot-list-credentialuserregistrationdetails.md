---
title: Listar credentialUserRegistrationDetails
description: Obter uma lista de objetos credentialUserRegistrationDetails para um determinado locatário.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: dff76db70f1ccebb6f420575ab793a4bdf7c2b97
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358297"
---
# <a name="list-credentialuserregistrationdetails"></a><span data-ttu-id="9a75c-103">Listar credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="9a75c-103">List credentialUserRegistrationDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a75c-104">Obter uma lista de objetos [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) para um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="9a75c-104">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a75c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a75c-105">Permissions</span></span>

<span data-ttu-id="9a75c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a75c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a75c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a75c-108">Permission type</span></span>                        | <span data-ttu-id="9a75c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a75c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9a75c-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a75c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a75c-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a75c-111">Reports.Read.All</span></span> |
| <span data-ttu-id="9a75c-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a75c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a75c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a75c-113">Not supported.</span></span> |
| <span data-ttu-id="9a75c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a75c-114">Application</span></span>                            | <span data-ttu-id="9a75c-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a75c-115">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a75c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a75c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/credentialUserRegistrationDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9a75c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9a75c-117">Optional query parameters</span></span>

<span data-ttu-id="9a75c-118">Essa função suporta o parâmetro de consulta OData opcional **$Filter**.</span><span class="sxs-lookup"><span data-stu-id="9a75c-118">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="9a75c-119">Você pode aplicar **$Filter** em uma ou mais das seguintes propriedades do recurso [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="9a75c-119">You can apply **$filter** on one or more of the following properties of the [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) resource.</span></span>

| <span data-ttu-id="9a75c-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a75c-120">Properties</span></span> | <span data-ttu-id="9a75c-121">Descrição e exemplo</span><span class="sxs-lookup"><span data-stu-id="9a75c-121">Description and example</span></span> |
| --------- | ----------------------- |
| <span data-ttu-id="9a75c-122">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="9a75c-122">userDisplayName</span></span> | <span data-ttu-id="9a75c-123">Filtrar por nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="9a75c-123">Filter by user name.</span></span> <span data-ttu-id="9a75c-124">Por exemplo: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="9a75c-124">For example: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="9a75c-125">Operadores de filtro suportados `eq`:, `startswith()`e.</span><span class="sxs-lookup"><span data-stu-id="9a75c-125">Supported filter operators: `eq`, and `startswith()`.</span></span> <span data-ttu-id="9a75c-126">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9a75c-126">Supports case insensitive.</span></span> |
| <span data-ttu-id="9a75c-127">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9a75c-127">userPrincipalName</span></span> | <span data-ttu-id="9a75c-128">Filtrar por nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="9a75c-128">Filter by user principal name.</span></span> <span data-ttu-id="9a75c-129">Por exemplo: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="9a75c-129">For example: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span> <span data-ttu-id="9a75c-130">Operadores de filtro suportados `eq` : `startswith()`e.</span><span class="sxs-lookup"><span data-stu-id="9a75c-130">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="9a75c-131">Dá suporte a maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9a75c-131">Supports case insensitive.</span></span> |
| <span data-ttu-id="9a75c-132">authMethods</span><span class="sxs-lookup"><span data-stu-id="9a75c-132">authMethods</span></span> | <span data-ttu-id="9a75c-133">Filtrar pelos métodos de autenticação usados durante o registro.</span><span class="sxs-lookup"><span data-stu-id="9a75c-133">Filter by the authentication methods used during registration.</span></span> <span data-ttu-id="9a75c-134">Por exemplo: `/reports/userCredentialUsageDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`.</span><span class="sxs-lookup"><span data-stu-id="9a75c-134">For example: `/reports/userCredentialUsageDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`.</span></span> <span data-ttu-id="9a75c-135">Operadores de filtro suportados `eq`:.</span><span class="sxs-lookup"><span data-stu-id="9a75c-135">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="9a75c-136">IsRegistered</span><span class="sxs-lookup"><span data-stu-id="9a75c-136">isRegistered</span></span> | <span data-ttu-id="9a75c-137">Filtro para usuários que registraram a redefinição de senha de autoatendimento (SSPR).</span><span class="sxs-lookup"><span data-stu-id="9a75c-137">Filter for users who have registered for self-service password reset (SSPR).</span></span> <span data-ttu-id="9a75c-138">Por exemplo: `/reports/userCredentialUsageDetails?$filter=isRegistered eq true`.</span><span class="sxs-lookup"><span data-stu-id="9a75c-138">For example: `/reports/userCredentialUsageDetails?$filter=isRegistered eq true`.</span></span> <span data-ttu-id="9a75c-139">Operadores de filtro suportados `eq`:.</span><span class="sxs-lookup"><span data-stu-id="9a75c-139">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="9a75c-140">isEnabled</span><span class="sxs-lookup"><span data-stu-id="9a75c-140">isEnabled</span></span> | <span data-ttu-id="9a75c-141">Filtro para usuários que foram habilitados para o SSPR.</span><span class="sxs-lookup"><span data-stu-id="9a75c-141">Filter for users who have been enabled for SSPR.</span></span> <span data-ttu-id="9a75c-142">Por exemplo: `/reports/userCredentialUsageDetails?$filter=isEnabled eq true`.</span><span class="sxs-lookup"><span data-stu-id="9a75c-142">For example: `/reports/userCredentialUsageDetails?$filter=isEnabled eq true`.</span></span> <span data-ttu-id="9a75c-143">Operadores filtter com suporte `eq`:.</span><span class="sxs-lookup"><span data-stu-id="9a75c-143">Supported filtter operators: `eq`.</span></span> |
| <span data-ttu-id="9a75c-144">iscapable</span><span class="sxs-lookup"><span data-stu-id="9a75c-144">isCapable</span></span> | <span data-ttu-id="9a75c-145">Filtro para usuários que estão prontos para executar redefinição de senha ou a autenticação multifator (MFA).</span><span class="sxs-lookup"><span data-stu-id="9a75c-145">Filter for users who are ready to perform password reset or multi-factor authentication (MFA).</span></span> <span data-ttu-id="9a75c-146">Por exemplo: `/reports/userCredentialUsageDetails?$filter=isCapable eq true`.</span><span class="sxs-lookup"><span data-stu-id="9a75c-146">For example: `/reports/userCredentialUsageDetails?$filter=isCapable eq true`.</span></span> <span data-ttu-id="9a75c-147">Operadores de filtro suportados:`eq`</span><span class="sxs-lookup"><span data-stu-id="9a75c-147">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="9a75c-148">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="9a75c-148">isMfaRegistered</span></span> | <span data-ttu-id="9a75c-149">Filtro para usuários registrados para MFA.</span><span class="sxs-lookup"><span data-stu-id="9a75c-149">Filter for users who are registered for MFA.</span></span> <span data-ttu-id="9a75c-150">Por exemplo: `/reports/userCredentialUsageDetails?$filter=isMfaRegistered eq true`.</span><span class="sxs-lookup"><span data-stu-id="9a75c-150">For example: `/reports/userCredentialUsageDetails?$filter=isMfaRegistered eq true`.</span></span> <span data-ttu-id="9a75c-151">Operadores de filtro suportados `eq`:.</span><span class="sxs-lookup"><span data-stu-id="9a75c-151">Supported filter operators: `eq`.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9a75c-152">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a75c-152">Request headers</span></span>

| <span data-ttu-id="9a75c-153">Nome</span><span class="sxs-lookup"><span data-stu-id="9a75c-153">Name</span></span>      |<span data-ttu-id="9a75c-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a75c-154">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9a75c-155">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a75c-155">Authorization</span></span> | <span data-ttu-id="9a75c-156">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="9a75c-156">Bearer {token}</span></span> |
| <span data-ttu-id="9a75c-157">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9a75c-157">Content-Type</span></span> | <span data-ttu-id="9a75c-158">application/json</span><span class="sxs-lookup"><span data-stu-id="9a75c-158">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a75c-159">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a75c-159">Request body</span></span>

<span data-ttu-id="9a75c-160">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9a75c-160">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a75c-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a75c-161">Response</span></span>

<span data-ttu-id="9a75c-162">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a75c-162">If successful, this method returns a `200 OK` response code and a collection of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a75c-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9a75c-163">Examples</span></span>

<span data-ttu-id="9a75c-164">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="9a75c-164">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="9a75c-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a75c-165">Request</span></span>

<span data-ttu-id="9a75c-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a75c-166">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9a75c-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a75c-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}-->

```http
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a75c-168">C#</span><span class="sxs-lookup"><span data-stu-id="9a75c-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-credentialuserregistrationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a75c-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a75c-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-credentialuserregistrationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a75c-170">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9a75c-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-credentialuserregistrationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9a75c-171">Java</span><span class="sxs-lookup"><span data-stu-id="9a75c-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-credentialuserregistrationdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9a75c-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a75c-172">Response</span></span>

<span data-ttu-id="9a75c-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9a75c-173">The following is an example of the response.</span></span>

> <span data-ttu-id="9a75c-174">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9a75c-174">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9a75c-175">Todas as propriedades são retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a75c-175">All the properties are returned from an actual call.</span></span>

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
