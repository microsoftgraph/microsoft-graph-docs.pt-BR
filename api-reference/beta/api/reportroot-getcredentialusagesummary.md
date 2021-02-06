---
title: 'reportRoot: getCredentialUsageSummary'
description: Relatar o estado atual de quantos usuários em sua organização estão usando recursos de redefinição de senha de autoatendado.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 56015afd7bc5589d518277df555ac511b7f91657
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131352"
---
# <a name="reportroot-getcredentialusagesummary"></a><span data-ttu-id="cf8b9-103">reportRoot: getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="cf8b9-103">reportRoot: getCredentialUsageSummary</span></span>

<span data-ttu-id="cf8b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf8b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf8b9-105">Relatar o estado atual de quantos usuários em sua organização usaram os recursos de redefinição de senha de autoatendado.</span><span class="sxs-lookup"><span data-stu-id="cf8b9-105">Report the current state of how many users in your organization used the self-service password reset capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf8b9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cf8b9-106">Permissions</span></span>

<span data-ttu-id="cf8b9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf8b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf8b9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf8b9-109">Permission type</span></span>                        | <span data-ttu-id="cf8b9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf8b9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cf8b9-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf8b9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf8b9-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf8b9-112">Reports.Read.All</span></span> |
| <span data-ttu-id="cf8b9-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf8b9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf8b9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf8b9-114">Not supported.</span></span> |
| <span data-ttu-id="cf8b9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf8b9-115">Application</span></span>                            | <span data-ttu-id="cf8b9-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf8b9-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf8b9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf8b9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUsageSummary
```

## <a name="function-parameters"></a><span data-ttu-id="cf8b9-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="cf8b9-118">Function parameters</span></span>

<span data-ttu-id="cf8b9-119">Você pode usar o parâmetro de função a seguir para ajustar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cf8b9-119">You can use the following function parameter to adjust the response.</span></span>

| <span data-ttu-id="cf8b9-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cf8b9-120">Parameter</span></span> | <span data-ttu-id="cf8b9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf8b9-121">Type</span></span> | <span data-ttu-id="cf8b9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf8b9-122">Description</span></span> |
|:--------- |:---- |:----------- |
| <span data-ttu-id="cf8b9-123">ponto</span><span class="sxs-lookup"><span data-stu-id="cf8b9-123">period</span></span> | <span data-ttu-id="cf8b9-124">String</span><span class="sxs-lookup"><span data-stu-id="cf8b9-124">String</span></span> | <span data-ttu-id="cf8b9-125">Especifica o período de tempo para o qual você precisa dos dados de uso.</span><span class="sxs-lookup"><span data-stu-id="cf8b9-125">Specifies the time period for which you need the usage data.</span></span> <span data-ttu-id="cf8b9-126">Por exemplo: `/reports/getCredentialUsageSummary(period='D30')`.</span><span class="sxs-lookup"><span data-stu-id="cf8b9-126">For example: `/reports/getCredentialUsageSummary(period='D30')`.</span></span> <span data-ttu-id="cf8b9-127">Períodos com suporte: `D1` `D7` , e `D30` .</span><span class="sxs-lookup"><span data-stu-id="cf8b9-127">Supported periods: `D1`, `D7`, and `D30`.</span></span> <span data-ttu-id="cf8b9-128">O ponto não faz falta de maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="cf8b9-128">Period is case insensitive.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="cf8b9-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cf8b9-129">Optional query parameters</span></span>

<span data-ttu-id="cf8b9-130">Esta função dá suporte ao parâmetro opcional de consulta OData **$filter**.</span><span class="sxs-lookup"><span data-stu-id="cf8b9-130">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="cf8b9-131">Você pode aplicar **$filter** em uma ou mais das seguintes propriedades do [recurso credentialUsageSummary.](../resources/credentialusagesummary.md)</span><span class="sxs-lookup"><span data-stu-id="cf8b9-131">You can apply **$filter** on one or more of the following properties of the [credentialUsageSummary](../resources/credentialusagesummary.md) resource.</span></span>

| <span data-ttu-id="cf8b9-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf8b9-132">Properties</span></span> | <span data-ttu-id="cf8b9-133">Descrição e exemplo</span><span class="sxs-lookup"><span data-stu-id="cf8b9-133">Description and example</span></span> |
|:---- |:----------- |
| <span data-ttu-id="cf8b9-134">recurso</span><span class="sxs-lookup"><span data-stu-id="cf8b9-134">feature</span></span> | <span data-ttu-id="cf8b9-135">Especifica o tipo de dados de uso que você deseja (registro versus redefinição).</span><span class="sxs-lookup"><span data-stu-id="cf8b9-135">Specifies the type of usage data you want (registration vs. reset).</span></span> <span data-ttu-id="cf8b9-136">Por exemplo: `/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'`.</span><span class="sxs-lookup"><span data-stu-id="cf8b9-136">For example: `/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="cf8b9-137">Operadores de filtro com suporte: `eq` .</span><span class="sxs-lookup"><span data-stu-id="cf8b9-137">Supported filter operators: `eq`.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="cf8b9-138">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf8b9-138">Request headers</span></span>

| <span data-ttu-id="cf8b9-139">Nome</span><span class="sxs-lookup"><span data-stu-id="cf8b9-139">Name</span></span>          | <span data-ttu-id="cf8b9-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf8b9-140">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cf8b9-141">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf8b9-141">Authorization</span></span> | <span data-ttu-id="cf8b9-142">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="cf8b9-142">Bearer {token}</span></span> |
| <span data-ttu-id="cf8b9-143">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cf8b9-143">Content-Type</span></span> | <span data-ttu-id="cf8b9-144">application/json</span><span class="sxs-lookup"><span data-stu-id="cf8b9-144">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf8b9-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf8b9-145">Request body</span></span>

<span data-ttu-id="cf8b9-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cf8b9-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf8b9-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf8b9-147">Response</span></span>

<span data-ttu-id="cf8b9-148">Se bem-sucedido, este método retorna um código de resposta e um novo objeto da coleção `200 OK` [credentialUsageSummary](../resources/credentialusagesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf8b9-148">If successful, this method returns a `200 OK` response code and a new [credentialUsageSummary](../resources/credentialusagesummary.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cf8b9-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cf8b9-149">Examples</span></span>

<span data-ttu-id="cf8b9-150">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="cf8b9-150">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="cf8b9-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf8b9-151">Request</span></span>

<span data-ttu-id="cf8b9-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf8b9-152">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf8b9-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf8b9-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialusagesummary"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'
```
# <a name="c"></a>[<span data-ttu-id="cf8b9-154">C#</span><span class="sxs-lookup"><span data-stu-id="cf8b9-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialusagesummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf8b9-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf8b9-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialusagesummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf8b9-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf8b9-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialusagesummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf8b9-157">Java</span><span class="sxs-lookup"><span data-stu-id="cf8b9-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getcredentialusagesummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cf8b9-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf8b9-158">Response</span></span>

<span data-ttu-id="cf8b9-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cf8b9-159">The following is an example of the response.</span></span>

> <span data-ttu-id="cf8b9-160">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cf8b9-160">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cf8b9-161">Todas as propriedades são retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf8b9-161">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.getCredentialUsageSummary)",
  "value":[
    {
      "id" : "id-value",
      "feature":"registration",
      "successfulActivityCount":12345,
      "failureActivityCount": 123,
      "authMethod": "email"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reportRoot: getCredentialUsageSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


