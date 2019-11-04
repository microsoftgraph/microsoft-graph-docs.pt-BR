---
title: Listar logons
doc_type: apiPageType
description: Obtenha uma lista das entradas de usuário em um locatário do Azure Active Directory.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5fa97184a4858d3b8fee7b537310cc09270a749b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938362"
---
# <a name="list-signins"></a><span data-ttu-id="302f8-103">Listar logons</span><span class="sxs-lookup"><span data-stu-id="302f8-103">List signIns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="302f8-104">Obter uma lista de objetos de [entrada](../resources/signin.md) .</span><span class="sxs-lookup"><span data-stu-id="302f8-104">Get a list of [signIn](../resources/signin.md) objects.</span></span> <span data-ttu-id="302f8-105">A lista contém as entradas de usuário para o locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="302f8-105">The list contains the user sign-ins for your Azure Active Directory tenant.</span></span> <span data-ttu-id="302f8-106">Entradas onde um nome de usuário e senha são passados como parte do token de autorização, e os logins federados bem sucedidos estão atualmente incluídos nos logs de entrada.</span><span class="sxs-lookup"><span data-stu-id="302f8-106">Sign-ins where a username and password are passed as part of authorization token, and successful federated sign-ins are currently included in the sign-in logs.</span></span> <span data-ttu-id="302f8-107">As entradas mais recentes são retornadas primeiro.</span><span class="sxs-lookup"><span data-stu-id="302f8-107">The most recent sign-ins are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="302f8-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="302f8-108">Permissions</span></span>

<span data-ttu-id="302f8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="302f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="302f8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="302f8-111">Permission type</span></span> | <span data-ttu-id="302f8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="302f8-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="302f8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="302f8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="302f8-114">AuditLog. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="302f8-114">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="302f8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="302f8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="302f8-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="302f8-116">Not supported</span></span> |
| <span data-ttu-id="302f8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="302f8-117">Application</span></span> | <span data-ttu-id="302f8-118">AuditLog. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="302f8-118">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="302f8-119">Além disso, os aplicativos devem ser registrados corretamente no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="302f8-119">In addition, apps must be properly registered to Azure Active Directory.</span></span>

## <a name="http-request"></a><span data-ttu-id="302f8-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="302f8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="302f8-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="302f8-121">Optional query parameters</span></span>

<span data-ttu-id="302f8-122">Este método dá suporte aos seguintes Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="302f8-122">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="302f8-123">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="302f8-123">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

| <span data-ttu-id="302f8-124">Nome</span><span class="sxs-lookup"><span data-stu-id="302f8-124">Name</span></span> | <span data-ttu-id="302f8-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="302f8-125">Description</span></span> | <span data-ttu-id="302f8-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="302f8-126">Example</span></span> |
|:---- |:----------- |:------- |
| [<span data-ttu-id="302f8-127">$filter</span><span class="sxs-lookup"><span data-stu-id="302f8-127">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)| <span data-ttu-id="302f8-128">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="302f8-128">Filters results (rows).</span></span> | `/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24` |
| [<span data-ttu-id="302f8-129">$top</span><span class="sxs-lookup"><span data-stu-id="302f8-129">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter) | <span data-ttu-id="302f8-130">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="302f8-130">Sets the page size of results.</span></span> | `/auditLogs/signIns?$top=1` |
| [<span data-ttu-id="302f8-131">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="302f8-131">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter) | <span data-ttu-id="302f8-132">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas.</span><span class="sxs-lookup"><span data-stu-id="302f8-132">Retrieves the next page of results from result sets that span multiple pages.</span></span> |`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1` |

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="302f8-133">Atributos com suporte pelo parâmetro $filter</span><span class="sxs-lookup"><span data-stu-id="302f8-133">Attributes supported by $filter parameter</span></span>

| <span data-ttu-id="302f8-134">Nome do Atributo</span><span class="sxs-lookup"><span data-stu-id="302f8-134">Attribute Name</span></span> | <span data-ttu-id="302f8-135">Operadores com suporte</span><span class="sxs-lookup"><span data-stu-id="302f8-135">Supported operators</span></span> |
|:-------------- |:------------------- |
| <span data-ttu-id="302f8-136">id</span><span class="sxs-lookup"><span data-stu-id="302f8-136">id</span></span> | <span data-ttu-id="302f8-137">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-137">eq</span></span> |
| <span data-ttu-id="302f8-138">userId</span><span class="sxs-lookup"><span data-stu-id="302f8-138">userId</span></span> | <span data-ttu-id="302f8-139">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-139">eq</span></span> |
| <span data-ttu-id="302f8-140">appId</span><span class="sxs-lookup"><span data-stu-id="302f8-140">appId</span></span> | <span data-ttu-id="302f8-141">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-141">eq</span></span> |
| <span data-ttu-id="302f8-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="302f8-142">createdDateTime</span></span> | <span data-ttu-id="302f8-143">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="302f8-143">eq, le, ge</span></span> |
| <span data-ttu-id="302f8-144">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="302f8-144">userDisplayName</span></span> | <span data-ttu-id="302f8-145">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="302f8-145">eq, startswith</span></span> |
| <span data-ttu-id="302f8-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="302f8-146">userPrincipalName</span></span> | <span data-ttu-id="302f8-147">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="302f8-147">eq, startswith</span></span> |
| <span data-ttu-id="302f8-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="302f8-148">appDisplayName</span></span> | <span data-ttu-id="302f8-149">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="302f8-149">eq, startswith</span></span> |
| <span data-ttu-id="302f8-150">ipAddress</span><span class="sxs-lookup"><span data-stu-id="302f8-150">ipAddress</span></span> | <span data-ttu-id="302f8-151">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="302f8-151">eq, startswith</span></span> |
| <span data-ttu-id="302f8-152">localização/cidade</span><span class="sxs-lookup"><span data-stu-id="302f8-152">location/city</span></span> | <span data-ttu-id="302f8-153">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="302f8-153">eq, startswith</span></span> |
| <span data-ttu-id="302f8-154">localização/estado</span><span class="sxs-lookup"><span data-stu-id="302f8-154">location/state</span></span> | <span data-ttu-id="302f8-155">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="302f8-155">eq, startswith</span></span> |
| <span data-ttu-id="302f8-156">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="302f8-156">location/countryOrRegion</span></span> | <span data-ttu-id="302f8-157">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="302f8-157">eq, startswith</span></span> |
| <span data-ttu-id="302f8-158">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="302f8-158">status/errorCode</span></span> | <span data-ttu-id="302f8-159">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-159">eq</span></span> |
| <span data-ttu-id="302f8-160">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="302f8-160">initiatedBy/user/id</span></span> | <span data-ttu-id="302f8-161">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-161">eq</span></span> |
| <span data-ttu-id="302f8-162">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="302f8-162">initiatedBy/user/displayName</span></span> | <span data-ttu-id="302f8-163">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-163">eq</span></span> |
| <span data-ttu-id="302f8-164">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="302f8-164">initiatedBy/user/userPrincipalName</span></span> | <span data-ttu-id="302f8-165">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="302f8-165">eq, startswith</span></span> |
| <span data-ttu-id="302f8-166">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="302f8-166">clientAppUsed</span></span> | <span data-ttu-id="302f8-167">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-167">eq</span></span> |
| <span data-ttu-id="302f8-168">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="302f8-168">conditionalAccessStatus</span></span> | <span data-ttu-id="302f8-169">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-169">eq</span></span> |
| <span data-ttu-id="302f8-170">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="302f8-170">deviceDetail/browser</span></span> | <span data-ttu-id="302f8-171">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="302f8-171">eq, startswith</span></span> |
| <span data-ttu-id="302f8-172">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="302f8-172">deviceDetail/operatingSystem</span></span> | <span data-ttu-id="302f8-173">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="302f8-173">eq, startswith</span></span> |
| <span data-ttu-id="302f8-174">correlationId</span><span class="sxs-lookup"><span data-stu-id="302f8-174">correlationId</span></span> | <span data-ttu-id="302f8-175">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-175">eq</span></span> |
| <span data-ttu-id="302f8-176">riskDetail</span><span class="sxs-lookup"><span data-stu-id="302f8-176">riskDetail</span></span> | <span data-ttu-id="302f8-177">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-177">eq</span></span> |
| <span data-ttu-id="302f8-178">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="302f8-178">riskLevelAggregated</span></span> | <span data-ttu-id="302f8-179">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-179">eq</span></span> |
| <span data-ttu-id="302f8-180">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="302f8-180">riskLevelDuringSignIn</span></span> | <span data-ttu-id="302f8-181">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-181">eq</span></span> |
| <span data-ttu-id="302f8-182">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="302f8-182">riskEventTypes</span></span> | <span data-ttu-id="302f8-183">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-183">eq</span></span> |
| <span data-ttu-id="302f8-184">riskState</span><span class="sxs-lookup"><span data-stu-id="302f8-184">riskState</span></span> | <span data-ttu-id="302f8-185">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-185">eq</span></span> |
| <span data-ttu-id="302f8-186">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="302f8-186">originalRequestId</span></span> | <span data-ttu-id="302f8-187">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-187">eq</span></span> |
| <span data-ttu-id="302f8-188">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="302f8-188">tokenIssuerName</span></span> | <span data-ttu-id="302f8-189">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-189">eq</span></span> |
| <span data-ttu-id="302f8-190">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="302f8-190">tokenIssuerType</span></span> | <span data-ttu-id="302f8-191">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-191">eq</span></span> |
| <span data-ttu-id="302f8-192">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="302f8-192">resourceDisplayName</span></span> | <span data-ttu-id="302f8-193">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-193">eq</span></span> |
| <span data-ttu-id="302f8-194">resourceId</span><span class="sxs-lookup"><span data-stu-id="302f8-194">resourceId</span></span> | <span data-ttu-id="302f8-195">eq</span><span class="sxs-lookup"><span data-stu-id="302f8-195">eq</span></span> |
| <span data-ttu-id="302f8-196">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="302f8-196">servicePrincipalId</span></span> | <span data-ttu-id="302f8-197">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="302f8-197">eq, startswith</span></span> |
| <span data-ttu-id="302f8-198">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="302f8-198">servicePrincipalName</span></span> | <span data-ttu-id="302f8-199">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="302f8-199">eq, startswith</span></span> |
| <span data-ttu-id="302f8-200">userAgent</span><span class="sxs-lookup"><span data-stu-id="302f8-200">userAgent</span></span> | <span data-ttu-id="302f8-201">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="302f8-201">eq, startswith</span></span> |
| <span data-ttu-id="302f8-202">alternateSignInName</span><span class="sxs-lookup"><span data-stu-id="302f8-202">alternateSignInName</span></span> | <span data-ttu-id="302f8-203">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="302f8-203">eq, startswith</span></span> |

## <a name="request-headers"></a><span data-ttu-id="302f8-204">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="302f8-204">Request headers</span></span>

| <span data-ttu-id="302f8-205">Nome</span><span class="sxs-lookup"><span data-stu-id="302f8-205">Name</span></span>      |<span data-ttu-id="302f8-206">Descrição</span><span class="sxs-lookup"><span data-stu-id="302f8-206">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="302f8-207">Autorização</span><span class="sxs-lookup"><span data-stu-id="302f8-207">Authorization</span></span> | <span data-ttu-id="302f8-208">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="302f8-208">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="302f8-209">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="302f8-209">Request body</span></span>

<span data-ttu-id="302f8-210">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="302f8-210">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="302f8-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="302f8-211">Response</span></span>

<span data-ttu-id="302f8-212">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos de [logon](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="302f8-212">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="302f8-213">Exemplos</span><span class="sxs-lookup"><span data-stu-id="302f8-213">Examples</span></span>

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a><span data-ttu-id="302f8-214">Exemplo 1: o usuário faz logon usando MFA, que é disparada por uma política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="302f8-214">Example 1: User signs in using MFA, which is triggered by a conditional access policy.</span></span> <span data-ttu-id="302f8-215">A autenticação principal é por meio do FIDO.</span><span class="sxs-lookup"><span data-stu-id="302f8-215">Primary authentication is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="302f8-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="302f8-216">Request</span></span>

<span data-ttu-id="302f8-217">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="302f8-217">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="302f8-218">HTTP</span><span class="sxs-lookup"><span data-stu-id="302f8-218">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="302f8-219">C#</span><span class="sxs-lookup"><span data-stu-id="302f8-219">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="302f8-220">JavaScript</span><span class="sxs-lookup"><span data-stu-id="302f8-220">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="302f8-221">Objective-C</span><span class="sxs-lookup"><span data-stu-id="302f8-221">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="302f8-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="302f8-222">Response</span></span>

<span data-ttu-id="302f8-223">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="302f8-223">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "value": [
    {
      "id":"b01b1726-0147-425e-a7f7-21f252050400",
      "createdDateTime":"2018-11-06T18:48:33.8527147Z",
      "userDisplayName":"Jon Doe",
      "userPrincipalName":"jdoe@www.contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
      "ipAddress":"207.254.19.10",
      "clientAppUsed":"Browser",
      "authenticationDetails": [
        {
          "authenticationStepDateTime":"2018-11-06T18:48:03.8313489Z",
          "authenticationMethod":"FIDO2",
          "authenticationMethodDetail":"1G54395783",
          "succeeded":true,
          "authenticationStepResultDetail":"methodSucceeded",
          "authenticationStepRequirement":"Primary authentication"
        },
        {
          "authenticationStepDateTime":"2018-11-06T18:48:12.94725647Z",
          "authenticationMethod":"Claim in access token",
          "authenticationMethodDetail":null,
          "succeeded":true,
          "authenticationStepResultDetail":"methodSucceeded",
          "authenticationStepRequirement":"MFA"
        }
      ],
      "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
      "conditionalAccessStatus":"applied",
      "isInteractive":true,
      "tokenIssuerName":null,
      "tokenIssuerType":"AzureAD",
      "processingTimeInMilliseconds":100,
      "riskDetail":"none",
      "riskLevelAggregated":"none",
      "riskLevelDuringsignIn":"none",
      "riskState":"none",
      "riskEventTypes":[],
      "resourceDisplayName":"windows azure service management api",
      "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
      "status":{},
      "deviceDetail": {
        "deviceId":null,
        "displayName":null,
        "operatingSystem":"Windows 7",
        "browser":"Chrome 63.0.3239",
        "isCompliant":null,
        "isManaged":null,
        "trustType":null
      },
      "location": {
        "city":"Lithia Springs",
        "state":"Georgia",
        "countryOrRegion":"US",
        "geoCoordinates": {
          "altitude":null,
          "latitude":33.7930908203125,
          "longitude":-84.445358276367188
        }
      },
      "appliedConditionalAccessPolicies": [
        {
          "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
          "displayName":"MFA policy",
          "enforcedGrantControls": [
            "Mfa",
            "RequireCompliantDevice"
          ],
          "enforcedSessionControls":[],
          "result":"applied"
        },
        {
          "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
          "displayName":"PipelineTest4",
          "enforcedGrantControls":[],
          "enforcedSessionControls":[],
          "result":"notEnabled"
        }
      ],
      "authenticationProcessingDetails":[],
      "networkLocationDetails":[]
    }
  ]
}
```
### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a><span data-ttu-id="302f8-224">Exemplo 2: o usuário entra no com somente autenticação principal.</span><span class="sxs-lookup"><span data-stu-id="302f8-224">Example 2: User signs in with only primary authentication.</span></span> <span data-ttu-id="302f8-225">A autenticação principal é por meio da senha da nuvem.</span><span class="sxs-lookup"><span data-stu-id="302f8-225">Primary authentication is through cloud password.</span></span>

#### <a name="request"></a><span data-ttu-id="302f8-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="302f8-226">Request</span></span>

<span data-ttu-id="302f8-227">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="302f8-227">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signins_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```

#### <a name="response"></a><span data-ttu-id="302f8-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="302f8-228">Response</span></span>

<span data-ttu-id="302f8-229">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="302f8-229">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "value": [
    {
      "id":"b01b1726-0147-425e-a7f7-21f252050400",
      "createdDateTime":"2018-11-06T18:48:33.8527147Z",
      "userDisplayName":"Jon Doe",
      "userPrincipalName":"jdoe@www.contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
      "ipAddress":"207.254.19.10",
      "clientAppUsed":"Browser",
      "authenticationDetails": [ 
        {
          "authenticationStepDateTime":"2018-11-06T18:48:03.8313489Z",
          "authenticationMethod":"Password",
          "authenticationMethodDetail":"Cloud password",
          "succeeded":true,
          "authenticationStepResultDetail":"methodSucceeded",
          "authenticationStepRequirement":"Primary authentication"
        }
      ],
      "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
      "conditionalAccessStatus":"applied",
      "isInteractive":true,
      "tokenIssuerName":null,
      "tokenIssuerType":"AzureAD",
      "processingTimeInMilliseconds":100,
      "riskDetail":"none",
      "riskLevelAggregated":"none",
      "riskLevelDuringsignIn":"none",
      "riskState":"none",
      "riskEventTypes":[],
      "resourceDisplayName":"windows azure service management api",
      "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
      "status":{},
      "deviceDetail": {
        "deviceId":null,
        "displayName":null,
        "operatingSystem":"Windows 7",
        "browser":"Chrome 63.0.3239",
        "isCompliant":null,
        "isManaged":null,
        "trustType":null
      },
      "location": {
        "city":"Lithia Springs",
        "state":"Georgia",
        "countryOrRegion":"US",
        "geoCoordinates": {
          "altitude":null,
          "latitude":33.7930908203125,
          "longitude":-84.445358276367188
        }
      },
      "appliedConditionalAccessPolicies": [
        {
          "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
          "displayName":"MFA policy",
          "enforcedGrantControls": [
            "Mfa",
            "RequireCompliantDevice"
          ],
          "enforcedSessionControls":[],
          "result":"notApplied"
        },
        {
          "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
          "displayName":"PipelineTest4",
          "enforcedGrantControls":[],
          "enforcedSessionControls":[],
          "result":"notEnabled"
        }
      ],
      "authenticationProcessingDetails":[],
      "networkLocationDetails":[]
    }
  ]
}
```