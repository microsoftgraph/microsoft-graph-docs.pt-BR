---
title: Listar logons
doc_type: apiPageType
description: Obter uma lista de logins do usuário em um locatário do Azure Active Directory.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
ms.openlocfilehash: b0662b88d8f6cca9ea8d602ee67073883f8504ef
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177029"
---
# <a name="list-signins"></a><span data-ttu-id="f0a87-103">Listar logons</span><span class="sxs-lookup"><span data-stu-id="f0a87-103">List signIns</span></span>

<span data-ttu-id="f0a87-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0a87-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0a87-105">Obter uma lista de [objetos signIn.](../resources/signin.md)</span><span class="sxs-lookup"><span data-stu-id="f0a87-105">Get a list of [signIn](../resources/signin.md) objects.</span></span> <span data-ttu-id="f0a87-106">A lista contém as ins loções de usuário para seu locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f0a87-106">The list contains the user sign-ins for your Azure Active Directory tenant.</span></span> <span data-ttu-id="f0a87-107">Sign-ins where a username and password are passed as part of authorization token, and successful federated sign-ins are currently included in the sign-in logs.</span><span class="sxs-lookup"><span data-stu-id="f0a87-107">Sign-ins where a username and password are passed as part of authorization token, and successful federated sign-ins are currently included in the sign-in logs.</span></span> <span data-ttu-id="f0a87-108">As insições mais recentes são retornadas primeiro.</span><span class="sxs-lookup"><span data-stu-id="f0a87-108">The most recent sign-ins are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0a87-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0a87-109">Permissions</span></span>

<span data-ttu-id="f0a87-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0a87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f0a87-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0a87-112">Permission type</span></span> | <span data-ttu-id="f0a87-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0a87-113">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="f0a87-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0a87-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f0a87-115">AuditLog.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0a87-115">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="f0a87-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0a87-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0a87-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f0a87-117">Not supported</span></span> |
| <span data-ttu-id="f0a87-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0a87-118">Application</span></span> | <span data-ttu-id="f0a87-119">AuditLog.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0a87-119">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="f0a87-120">Além disso, os aplicativos devem ser registrados corretamente no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f0a87-120">In addition, apps must be properly registered to Azure Active Directory.</span></span>

## <a name="http-request"></a><span data-ttu-id="f0a87-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0a87-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0a87-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f0a87-122">Optional query parameters</span></span>

<span data-ttu-id="f0a87-123">Este método dá suporte aos seguintes Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f0a87-123">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="f0a87-124">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="f0a87-124">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

| <span data-ttu-id="f0a87-125">Nome</span><span class="sxs-lookup"><span data-stu-id="f0a87-125">Name</span></span> | <span data-ttu-id="f0a87-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0a87-126">Description</span></span> | <span data-ttu-id="f0a87-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0a87-127">Example</span></span> |
|:---- |:----------- |:------- |
| [<span data-ttu-id="f0a87-128">$filter</span><span class="sxs-lookup"><span data-stu-id="f0a87-128">$filter</span></span>](/graph/query-parameters#filter-parameter)| <span data-ttu-id="f0a87-129">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="f0a87-129">Filters results (rows).</span></span> | `/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24` |
| [<span data-ttu-id="f0a87-130">$top</span><span class="sxs-lookup"><span data-stu-id="f0a87-130">$top</span></span>](/graph/query-parameters#top-parameter) | <span data-ttu-id="f0a87-131">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="f0a87-131">Sets the page size of results.</span></span> | `/auditLogs/signIns?$top=1` |
| [<span data-ttu-id="f0a87-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="f0a87-132">$skiptoken</span></span>](/graph/query-parameters#skiptoken-parameter) | <span data-ttu-id="f0a87-133">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas.</span><span class="sxs-lookup"><span data-stu-id="f0a87-133">Retrieves the next page of results from result sets that span multiple pages.</span></span> |`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1` |

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="f0a87-134">Atributos com suporte $filter parâmetro</span><span class="sxs-lookup"><span data-stu-id="f0a87-134">Attributes supported by $filter parameter</span></span>

| <span data-ttu-id="f0a87-135">Nome do Atributo</span><span class="sxs-lookup"><span data-stu-id="f0a87-135">Attribute Name</span></span> | <span data-ttu-id="f0a87-136">Operadores com suporte</span><span class="sxs-lookup"><span data-stu-id="f0a87-136">Supported operators</span></span> |
|:-------------- |:------------------- |
| <span data-ttu-id="f0a87-137">id</span><span class="sxs-lookup"><span data-stu-id="f0a87-137">id</span></span> | <span data-ttu-id="f0a87-138">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-138">eq</span></span> |
| <span data-ttu-id="f0a87-139">userId</span><span class="sxs-lookup"><span data-stu-id="f0a87-139">userId</span></span> | <span data-ttu-id="f0a87-140">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-140">eq</span></span> |
| <span data-ttu-id="f0a87-141">appId</span><span class="sxs-lookup"><span data-stu-id="f0a87-141">appId</span></span> | <span data-ttu-id="f0a87-142">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-142">eq</span></span> |
| <span data-ttu-id="f0a87-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0a87-143">createdDateTime</span></span> | <span data-ttu-id="f0a87-144">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="f0a87-144">eq, le, ge</span></span> |
| <span data-ttu-id="f0a87-145">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f0a87-145">userDisplayName</span></span> | <span data-ttu-id="f0a87-146">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f0a87-146">eq, startswith</span></span> |
| <span data-ttu-id="f0a87-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f0a87-147">userPrincipalName</span></span> | <span data-ttu-id="f0a87-148">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f0a87-148">eq, startswith</span></span> |
| <span data-ttu-id="f0a87-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="f0a87-149">appDisplayName</span></span> | <span data-ttu-id="f0a87-150">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f0a87-150">eq, startswith</span></span> |
| <span data-ttu-id="f0a87-151">authenticationRequirement</span><span class="sxs-lookup"><span data-stu-id="f0a87-151">authenticationRequirement</span></span> |<span data-ttu-id="f0a87-152">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f0a87-152">eq, startswith</span></span> |
| <span data-ttu-id="f0a87-153">ipAddress</span><span class="sxs-lookup"><span data-stu-id="f0a87-153">ipAddress</span></span> | <span data-ttu-id="f0a87-154">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f0a87-154">eq, startswith</span></span> |
| <span data-ttu-id="f0a87-155">localização/cidade</span><span class="sxs-lookup"><span data-stu-id="f0a87-155">location/city</span></span> | <span data-ttu-id="f0a87-156">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f0a87-156">eq, startswith</span></span> |
| <span data-ttu-id="f0a87-157">localização/estado</span><span class="sxs-lookup"><span data-stu-id="f0a87-157">location/state</span></span> | <span data-ttu-id="f0a87-158">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f0a87-158">eq, startswith</span></span> |
| <span data-ttu-id="f0a87-159">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="f0a87-159">location/countryOrRegion</span></span> | <span data-ttu-id="f0a87-160">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f0a87-160">eq, startswith</span></span> |
| <span data-ttu-id="f0a87-161">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="f0a87-161">status/errorCode</span></span> | <span data-ttu-id="f0a87-162">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-162">eq</span></span> |
| <span data-ttu-id="f0a87-163">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="f0a87-163">initiatedBy/user/id</span></span> | <span data-ttu-id="f0a87-164">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-164">eq</span></span> |
| <span data-ttu-id="f0a87-165">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="f0a87-165">initiatedBy/user/displayName</span></span> | <span data-ttu-id="f0a87-166">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-166">eq</span></span> |
| <span data-ttu-id="f0a87-167">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f0a87-167">initiatedBy/user/userPrincipalName</span></span> | <span data-ttu-id="f0a87-168">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f0a87-168">eq, startswith</span></span> |
| <span data-ttu-id="f0a87-169">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="f0a87-169">clientAppUsed</span></span> | <span data-ttu-id="f0a87-170">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-170">eq</span></span> |
| <span data-ttu-id="f0a87-171">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="f0a87-171">conditionalAccessStatus</span></span> | <span data-ttu-id="f0a87-172">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-172">eq</span></span> |
| <span data-ttu-id="f0a87-173">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="f0a87-173">deviceDetail/browser</span></span> | <span data-ttu-id="f0a87-174">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f0a87-174">eq, startswith</span></span> |
| <span data-ttu-id="f0a87-175">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="f0a87-175">deviceDetail/operatingSystem</span></span> | <span data-ttu-id="f0a87-176">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f0a87-176">eq, startswith</span></span> |
| <span data-ttu-id="f0a87-177">correlationId</span><span class="sxs-lookup"><span data-stu-id="f0a87-177">correlationId</span></span> | <span data-ttu-id="f0a87-178">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-178">eq</span></span> |
| <span data-ttu-id="f0a87-179">riskDetail</span><span class="sxs-lookup"><span data-stu-id="f0a87-179">riskDetail</span></span> | <span data-ttu-id="f0a87-180">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-180">eq</span></span> |
| <span data-ttu-id="f0a87-181">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="f0a87-181">riskLevelAggregated</span></span> | <span data-ttu-id="f0a87-182">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-182">eq</span></span> |
| <span data-ttu-id="f0a87-183">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="f0a87-183">riskLevelDuringSignIn</span></span> | <span data-ttu-id="f0a87-184">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-184">eq</span></span> |
| <span data-ttu-id="f0a87-185">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="f0a87-185">riskEventTypes</span></span> | <span data-ttu-id="f0a87-186">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-186">eq</span></span> |
| <span data-ttu-id="f0a87-187">riskEventTypes_v2</span><span class="sxs-lookup"><span data-stu-id="f0a87-187">riskEventTypes_v2</span></span> | <span data-ttu-id="f0a87-188">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f0a87-188">eq, startswith</span></span> |
| <span data-ttu-id="f0a87-189">riskState</span><span class="sxs-lookup"><span data-stu-id="f0a87-189">riskState</span></span> | <span data-ttu-id="f0a87-190">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-190">eq</span></span> |
| <span data-ttu-id="f0a87-191">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="f0a87-191">originalRequestId</span></span> | <span data-ttu-id="f0a87-192">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-192">eq</span></span> |
| <span data-ttu-id="f0a87-193">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="f0a87-193">tokenIssuerName</span></span> | <span data-ttu-id="f0a87-194">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-194">eq</span></span> |
| <span data-ttu-id="f0a87-195">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="f0a87-195">tokenIssuerType</span></span> | <span data-ttu-id="f0a87-196">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-196">eq</span></span> |
| <span data-ttu-id="f0a87-197">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f0a87-197">resourceDisplayName</span></span> | <span data-ttu-id="f0a87-198">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-198">eq</span></span> |
| <span data-ttu-id="f0a87-199">resourceId</span><span class="sxs-lookup"><span data-stu-id="f0a87-199">resourceId</span></span> | <span data-ttu-id="f0a87-200">eq</span><span class="sxs-lookup"><span data-stu-id="f0a87-200">eq</span></span> |
| <span data-ttu-id="f0a87-201">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="f0a87-201">servicePrincipalId</span></span> | <span data-ttu-id="f0a87-202">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f0a87-202">eq, startswith</span></span> |
| <span data-ttu-id="f0a87-203">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="f0a87-203">servicePrincipalName</span></span> | <span data-ttu-id="f0a87-204">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f0a87-204">eq, startswith</span></span> |
| <span data-ttu-id="f0a87-205">userAgent</span><span class="sxs-lookup"><span data-stu-id="f0a87-205">userAgent</span></span> | <span data-ttu-id="f0a87-206">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f0a87-206">eq, startswith</span></span> |
| <span data-ttu-id="f0a87-207">alternateSignInName</span><span class="sxs-lookup"><span data-stu-id="f0a87-207">alternateSignInName</span></span> | <span data-ttu-id="f0a87-208">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f0a87-208">eq, startswith</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f0a87-209">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0a87-209">Request headers</span></span>

| <span data-ttu-id="f0a87-210">Nome</span><span class="sxs-lookup"><span data-stu-id="f0a87-210">Name</span></span>      |<span data-ttu-id="f0a87-211">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0a87-211">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f0a87-212">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0a87-212">Authorization</span></span> | <span data-ttu-id="f0a87-213">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="f0a87-213">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0a87-214">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0a87-214">Request body</span></span>

<span data-ttu-id="f0a87-215">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f0a87-215">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0a87-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0a87-216">Response</span></span>

<span data-ttu-id="f0a87-217">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos de [logon](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0a87-217">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span> <span data-ttu-id="f0a87-218">A coleção de objetos é listada em ordem decrescente com base em **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="f0a87-218">The collection of objects is listed in descending order based on **createdDateTime**.</span></span>

## <a name="examples"></a><span data-ttu-id="f0a87-219">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f0a87-219">Examples</span></span>

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a><span data-ttu-id="f0a87-220">Exemplo 1: o usuário faz o acesso usando a MFA, que é disparada por uma política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="f0a87-220">Example 1: User signs in using MFA, which is triggered by a conditional access policy.</span></span> <span data-ttu-id="f0a87-221">A autenticação principal é por meio do FIDO.</span><span class="sxs-lookup"><span data-stu-id="f0a87-221">Primary authentication is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="f0a87-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0a87-222">Request</span></span>

<span data-ttu-id="f0a87-223">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0a87-223">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f0a87-224">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0a87-224">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="f0a87-225">C#</span><span class="sxs-lookup"><span data-stu-id="f0a87-225">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0a87-226">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0a87-226">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0a87-227">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0a87-227">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0a87-228">Java</span><span class="sxs-lookup"><span data-stu-id="f0a87-228">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signins-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f0a87-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0a87-229">Response</span></span>

<span data-ttu-id="f0a87-230">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f0a87-230">The following is an example of the response.</span></span>

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
            "id": "66ea54eb-blah-4ee5-be62-ff5a759b0100",
            "createdDateTime": "2020-03-13T19:15:41.6195833Z",
            "userDisplayName": "Test contoso",
            "userPrincipalName": "testaccount1@contoso.com",
            "userId": "26be570a-1111-5555-b4e2-a37c6808512d",
            "appId": "de8bc8b5-5555-6666-a8ad-b748da725064",
            "appDisplayName": "Graph explorer",
            "authenticationRequirement": "multiFactorAuthentication",
            "ipAddress": "131.107.159.37",
            "clientAppUsed": "Browser",
            "userAgent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.132 Safari/537.36 Edg/80.0.361.66",
            "correlationId": "d79f5bee-blah-4832-928f-3133e22ae912",
            "conditionalAccessStatus": "notApplied",
            "originalRequestId": "66ea54eb-blah-4ee5-be62-ff5a759b0100",
            "isInteractive": true,
            "tokenIssuerName": "",
            "tokenIssuerType": "AzureAD",
            "processingTimeInMilliseconds": 541,
            "riskDetail": "none",
            "riskLevelAggregated": "none",
            "riskLevelDuringSignIn": "none",
            "riskState": "none",
            "riskEventTypes": [],
            "riskEventTypes_v2": [],
            "resourceDisplayName": "Microsoft Graph",
            "resourceId": "00000003-0000-0000-c000-000000000000",
            "authenticationMethodsUsed": [],
            "alternateSignInName": "testaccount2.contoso.com",
            "servicePrincipalName": null,
            "servicePrincipalId": "",
            "mfaDetail": null,
            "status": {
                "errorCode": 0,
                "failureReason": null,
                "additionalDetails": null
            },
            "deviceDetail": {
                "deviceId": "",
                "displayName": null,
                "operatingSystem": "Windows 10",
                "browser": "Edge 80.0.361",
                "isCompliant": null,
                "isManaged": null,
                "trustType": null
            },
            "location": {
                "city": "Redmond",
                "state": "Washington",
                "countryOrRegion": "US",
                "geoCoordinates": {
                    "altitude": null,
                    "latitude": 47.68050003051758,
                    "longitude": -122.12094116210938
                }
            },
            "appliedConditionalAccessPolicies": [
                {
                    "id": "de7e60eb-ed89-4d73-8205-2227def6b7c9",
                    "displayName": "SharePoint limited access for guest workers",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled",
                    "conditionsSatisfied": "none",
                    "conditionsNotSatisfied": "none"
                },
                {
                    "id": "6701123a-b4c6-48af-8565-565c8bf7cabc",
                    "displayName": "Medium signin risk block",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled",
                    "conditionsSatisfied": "none",
                    "conditionsNotSatisfied": "none"
                },
               
            ],
            "authenticationProcessingDetails": [],
            "networkLocationDetails": [],
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
            "authenticationRequirementPolicies": []
        }
    ]
}
```
### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a><span data-ttu-id="f0a87-231">Exemplo 2: o usuário se insi com apenas a autenticação principal.</span><span class="sxs-lookup"><span data-stu-id="f0a87-231">Example 2: User signs in with only primary authentication.</span></span> <span data-ttu-id="f0a87-232">A autenticação principal é por meio da senha da nuvem.</span><span class="sxs-lookup"><span data-stu-id="f0a87-232">Primary authentication is through cloud password.</span></span>

#### <a name="request"></a><span data-ttu-id="f0a87-233">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0a87-233">Request</span></span>

<span data-ttu-id="f0a87-234">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0a87-234">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f0a87-235">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0a87-235">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="f0a87-236">C#</span><span class="sxs-lookup"><span data-stu-id="f0a87-236">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0a87-237">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0a87-237">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0a87-238">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0a87-238">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0a87-239">Java</span><span class="sxs-lookup"><span data-stu-id="f0a87-239">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signins-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f0a87-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0a87-240">Response</span></span>

<span data-ttu-id="f0a87-241">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f0a87-241">The following is an example of the response.</span></span>

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
      "userPrincipalName":"jdoe@contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
       "authenticationRequirement": "singleFactorAuthentication",
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
