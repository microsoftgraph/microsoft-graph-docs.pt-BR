---
title: Listar logons
doc_type: apiPageType
description: Obtenha uma lista das entradas de usuário em um locatário do Azure Active Directory.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 33b72a0361776a991f0f29675fced77379e3e215
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453265"
---
# <a name="list-signins"></a><span data-ttu-id="00d1a-103">Listar logons</span><span class="sxs-lookup"><span data-stu-id="00d1a-103">List signIns</span></span>

<span data-ttu-id="00d1a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00d1a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00d1a-105">Obter uma lista de objetos de [entrada](../resources/signin.md) .</span><span class="sxs-lookup"><span data-stu-id="00d1a-105">Get a list of [signIn](../resources/signin.md) objects.</span></span> <span data-ttu-id="00d1a-106">A lista contém as entradas de usuário para o locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="00d1a-106">The list contains the user sign-ins for your Azure Active Directory tenant.</span></span> <span data-ttu-id="00d1a-107">Entradas onde um nome de usuário e senha são passados como parte do token de autorização, e os logins federados bem sucedidos estão atualmente incluídos nos logs de entrada.</span><span class="sxs-lookup"><span data-stu-id="00d1a-107">Sign-ins where a username and password are passed as part of authorization token, and successful federated sign-ins are currently included in the sign-in logs.</span></span> <span data-ttu-id="00d1a-108">As entradas mais recentes são retornadas primeiro.</span><span class="sxs-lookup"><span data-stu-id="00d1a-108">The most recent sign-ins are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="00d1a-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="00d1a-109">Permissions</span></span>

<span data-ttu-id="00d1a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00d1a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="00d1a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00d1a-112">Permission type</span></span> | <span data-ttu-id="00d1a-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="00d1a-113">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="00d1a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00d1a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="00d1a-115">AuditLog. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="00d1a-115">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="00d1a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00d1a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00d1a-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="00d1a-117">Not supported</span></span> |
| <span data-ttu-id="00d1a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00d1a-118">Application</span></span> | <span data-ttu-id="00d1a-119">AuditLog. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="00d1a-119">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="00d1a-120">Além disso, os aplicativos devem ser registrados corretamente no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="00d1a-120">In addition, apps must be properly registered to Azure Active Directory.</span></span>

## <a name="http-request"></a><span data-ttu-id="00d1a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00d1a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00d1a-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="00d1a-122">Optional query parameters</span></span>

<span data-ttu-id="00d1a-123">Este método dá suporte aos seguintes Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="00d1a-123">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="00d1a-124">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="00d1a-124">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

| <span data-ttu-id="00d1a-125">Nome</span><span class="sxs-lookup"><span data-stu-id="00d1a-125">Name</span></span> | <span data-ttu-id="00d1a-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="00d1a-126">Description</span></span> | <span data-ttu-id="00d1a-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00d1a-127">Example</span></span> |
|:---- |:----------- |:------- |
| [<span data-ttu-id="00d1a-128">$filter</span><span class="sxs-lookup"><span data-stu-id="00d1a-128">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)| <span data-ttu-id="00d1a-129">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="00d1a-129">Filters results (rows).</span></span> | `/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24` |
| [<span data-ttu-id="00d1a-130">$top</span><span class="sxs-lookup"><span data-stu-id="00d1a-130">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter) | <span data-ttu-id="00d1a-131">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="00d1a-131">Sets the page size of results.</span></span> | `/auditLogs/signIns?$top=1` |
| [<span data-ttu-id="00d1a-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="00d1a-132">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter) | <span data-ttu-id="00d1a-133">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas.</span><span class="sxs-lookup"><span data-stu-id="00d1a-133">Retrieves the next page of results from result sets that span multiple pages.</span></span> |`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1` |

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="00d1a-134">Atributos com suporte pelo parâmetro $filter</span><span class="sxs-lookup"><span data-stu-id="00d1a-134">Attributes supported by $filter parameter</span></span>

| <span data-ttu-id="00d1a-135">Nome do Atributo</span><span class="sxs-lookup"><span data-stu-id="00d1a-135">Attribute Name</span></span> | <span data-ttu-id="00d1a-136">Operadores com suporte</span><span class="sxs-lookup"><span data-stu-id="00d1a-136">Supported operators</span></span> |
|:-------------- |:------------------- |
| <span data-ttu-id="00d1a-137">id</span><span class="sxs-lookup"><span data-stu-id="00d1a-137">id</span></span> | <span data-ttu-id="00d1a-138">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-138">eq</span></span> |
| <span data-ttu-id="00d1a-139">userId</span><span class="sxs-lookup"><span data-stu-id="00d1a-139">userId</span></span> | <span data-ttu-id="00d1a-140">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-140">eq</span></span> |
| <span data-ttu-id="00d1a-141">appId</span><span class="sxs-lookup"><span data-stu-id="00d1a-141">appId</span></span> | <span data-ttu-id="00d1a-142">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-142">eq</span></span> |
| <span data-ttu-id="00d1a-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00d1a-143">createdDateTime</span></span> | <span data-ttu-id="00d1a-144">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="00d1a-144">eq, le, ge</span></span> |
| <span data-ttu-id="00d1a-145">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="00d1a-145">userDisplayName</span></span> | <span data-ttu-id="00d1a-146">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="00d1a-146">eq, startswith</span></span> |
| <span data-ttu-id="00d1a-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="00d1a-147">userPrincipalName</span></span> | <span data-ttu-id="00d1a-148">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="00d1a-148">eq, startswith</span></span> |
| <span data-ttu-id="00d1a-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="00d1a-149">appDisplayName</span></span> | <span data-ttu-id="00d1a-150">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="00d1a-150">eq, startswith</span></span> |
| <span data-ttu-id="00d1a-151">ipAddress</span><span class="sxs-lookup"><span data-stu-id="00d1a-151">ipAddress</span></span> | <span data-ttu-id="00d1a-152">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="00d1a-152">eq, startswith</span></span> |
| <span data-ttu-id="00d1a-153">localização/cidade</span><span class="sxs-lookup"><span data-stu-id="00d1a-153">location/city</span></span> | <span data-ttu-id="00d1a-154">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="00d1a-154">eq, startswith</span></span> |
| <span data-ttu-id="00d1a-155">localização/estado</span><span class="sxs-lookup"><span data-stu-id="00d1a-155">location/state</span></span> | <span data-ttu-id="00d1a-156">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="00d1a-156">eq, startswith</span></span> |
| <span data-ttu-id="00d1a-157">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="00d1a-157">location/countryOrRegion</span></span> | <span data-ttu-id="00d1a-158">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="00d1a-158">eq, startswith</span></span> |
| <span data-ttu-id="00d1a-159">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="00d1a-159">status/errorCode</span></span> | <span data-ttu-id="00d1a-160">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-160">eq</span></span> |
| <span data-ttu-id="00d1a-161">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="00d1a-161">initiatedBy/user/id</span></span> | <span data-ttu-id="00d1a-162">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-162">eq</span></span> |
| <span data-ttu-id="00d1a-163">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="00d1a-163">initiatedBy/user/displayName</span></span> | <span data-ttu-id="00d1a-164">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-164">eq</span></span> |
| <span data-ttu-id="00d1a-165">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="00d1a-165">initiatedBy/user/userPrincipalName</span></span> | <span data-ttu-id="00d1a-166">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="00d1a-166">eq, startswith</span></span> |
| <span data-ttu-id="00d1a-167">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="00d1a-167">clientAppUsed</span></span> | <span data-ttu-id="00d1a-168">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-168">eq</span></span> |
| <span data-ttu-id="00d1a-169">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="00d1a-169">conditionalAccessStatus</span></span> | <span data-ttu-id="00d1a-170">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-170">eq</span></span> |
| <span data-ttu-id="00d1a-171">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="00d1a-171">deviceDetail/browser</span></span> | <span data-ttu-id="00d1a-172">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="00d1a-172">eq, startswith</span></span> |
| <span data-ttu-id="00d1a-173">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="00d1a-173">deviceDetail/operatingSystem</span></span> | <span data-ttu-id="00d1a-174">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="00d1a-174">eq, startswith</span></span> |
| <span data-ttu-id="00d1a-175">correlationId</span><span class="sxs-lookup"><span data-stu-id="00d1a-175">correlationId</span></span> | <span data-ttu-id="00d1a-176">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-176">eq</span></span> |
| <span data-ttu-id="00d1a-177">riskDetail</span><span class="sxs-lookup"><span data-stu-id="00d1a-177">riskDetail</span></span> | <span data-ttu-id="00d1a-178">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-178">eq</span></span> |
| <span data-ttu-id="00d1a-179">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="00d1a-179">riskLevelAggregated</span></span> | <span data-ttu-id="00d1a-180">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-180">eq</span></span> |
| <span data-ttu-id="00d1a-181">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="00d1a-181">riskLevelDuringSignIn</span></span> | <span data-ttu-id="00d1a-182">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-182">eq</span></span> |
| <span data-ttu-id="00d1a-183">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="00d1a-183">riskEventTypes</span></span> | <span data-ttu-id="00d1a-184">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-184">eq</span></span> |
| <span data-ttu-id="00d1a-185">riskState</span><span class="sxs-lookup"><span data-stu-id="00d1a-185">riskState</span></span> | <span data-ttu-id="00d1a-186">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-186">eq</span></span> |
| <span data-ttu-id="00d1a-187">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="00d1a-187">originalRequestId</span></span> | <span data-ttu-id="00d1a-188">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-188">eq</span></span> |
| <span data-ttu-id="00d1a-189">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="00d1a-189">tokenIssuerName</span></span> | <span data-ttu-id="00d1a-190">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-190">eq</span></span> |
| <span data-ttu-id="00d1a-191">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="00d1a-191">tokenIssuerType</span></span> | <span data-ttu-id="00d1a-192">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-192">eq</span></span> |
| <span data-ttu-id="00d1a-193">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="00d1a-193">resourceDisplayName</span></span> | <span data-ttu-id="00d1a-194">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-194">eq</span></span> |
| <span data-ttu-id="00d1a-195">resourceId</span><span class="sxs-lookup"><span data-stu-id="00d1a-195">resourceId</span></span> | <span data-ttu-id="00d1a-196">eq</span><span class="sxs-lookup"><span data-stu-id="00d1a-196">eq</span></span> |
| <span data-ttu-id="00d1a-197">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="00d1a-197">servicePrincipalId</span></span> | <span data-ttu-id="00d1a-198">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="00d1a-198">eq, startswith</span></span> |
| <span data-ttu-id="00d1a-199">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="00d1a-199">servicePrincipalName</span></span> | <span data-ttu-id="00d1a-200">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="00d1a-200">eq, startswith</span></span> |
| <span data-ttu-id="00d1a-201">userAgent</span><span class="sxs-lookup"><span data-stu-id="00d1a-201">userAgent</span></span> | <span data-ttu-id="00d1a-202">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="00d1a-202">eq, startswith</span></span> |
| <span data-ttu-id="00d1a-203">alternateSignInName</span><span class="sxs-lookup"><span data-stu-id="00d1a-203">alternateSignInName</span></span> | <span data-ttu-id="00d1a-204">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="00d1a-204">eq, startswith</span></span> |

## <a name="request-headers"></a><span data-ttu-id="00d1a-205">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00d1a-205">Request headers</span></span>

| <span data-ttu-id="00d1a-206">Nome</span><span class="sxs-lookup"><span data-stu-id="00d1a-206">Name</span></span>      |<span data-ttu-id="00d1a-207">Descrição</span><span class="sxs-lookup"><span data-stu-id="00d1a-207">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="00d1a-208">Autorização</span><span class="sxs-lookup"><span data-stu-id="00d1a-208">Authorization</span></span> | <span data-ttu-id="00d1a-209">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="00d1a-209">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="00d1a-210">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00d1a-210">Request body</span></span>

<span data-ttu-id="00d1a-211">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="00d1a-211">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00d1a-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="00d1a-212">Response</span></span>

<span data-ttu-id="00d1a-213">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos de [logon](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00d1a-213">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="00d1a-214">Exemplos</span><span class="sxs-lookup"><span data-stu-id="00d1a-214">Examples</span></span>

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a><span data-ttu-id="00d1a-215">Exemplo 1: o usuário faz logon usando MFA, que é disparada por uma política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="00d1a-215">Example 1: User signs in using MFA, which is triggered by a conditional access policy.</span></span> <span data-ttu-id="00d1a-216">A autenticação principal é por meio do FIDO.</span><span class="sxs-lookup"><span data-stu-id="00d1a-216">Primary authentication is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="00d1a-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00d1a-217">Request</span></span>

<span data-ttu-id="00d1a-218">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="00d1a-218">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="00d1a-219">HTTP</span><span class="sxs-lookup"><span data-stu-id="00d1a-219">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="00d1a-220">C#</span><span class="sxs-lookup"><span data-stu-id="00d1a-220">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00d1a-221">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00d1a-221">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00d1a-222">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00d1a-222">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="00d1a-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="00d1a-223">Response</span></span>

<span data-ttu-id="00d1a-224">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="00d1a-224">The following is an example of the response.</span></span>

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
### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a><span data-ttu-id="00d1a-225">Exemplo 2: o usuário entra no com somente autenticação principal.</span><span class="sxs-lookup"><span data-stu-id="00d1a-225">Example 2: User signs in with only primary authentication.</span></span> <span data-ttu-id="00d1a-226">A autenticação principal é por meio da senha da nuvem.</span><span class="sxs-lookup"><span data-stu-id="00d1a-226">Primary authentication is through cloud password.</span></span>

#### <a name="request"></a><span data-ttu-id="00d1a-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00d1a-227">Request</span></span>

<span data-ttu-id="00d1a-228">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="00d1a-228">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="00d1a-229">HTTP</span><span class="sxs-lookup"><span data-stu-id="00d1a-229">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="00d1a-230">C#</span><span class="sxs-lookup"><span data-stu-id="00d1a-230">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00d1a-231">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00d1a-231">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00d1a-232">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00d1a-232">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="00d1a-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="00d1a-233">Response</span></span>

<span data-ttu-id="00d1a-234">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="00d1a-234">The following is an example of the response.</span></span>

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
