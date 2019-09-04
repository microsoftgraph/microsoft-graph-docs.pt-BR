---
title: 'reportRoot: getCredentialUsageSummary'
description: Informe o estado atual de quantos usuários da sua organização estão usando recursos de redefinição de senha de autoatendimento.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 05eb1ecbc8ceb8474cdc1af3d7dabcb6a75aa44a
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36725357"
---
# <a name="reportroot-getcredentialusagesummary"></a><span data-ttu-id="79f43-103">reportRoot: getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="79f43-103">reportRoot: getCredentialUsageSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79f43-104">Informe o estado atual de quantos usuários da sua organização usaram as funcionalidades de redefinição de senha de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="79f43-104">Report the current state of how many users in your organization used the self-service password reset capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="79f43-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="79f43-105">Permissions</span></span>

<span data-ttu-id="79f43-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79f43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79f43-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79f43-108">Permission type</span></span>                        | <span data-ttu-id="79f43-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79f43-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="79f43-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79f43-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="79f43-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="79f43-111">Reports.Read.All</span></span> |
| <span data-ttu-id="79f43-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79f43-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79f43-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79f43-113">Not supported.</span></span> |
| <span data-ttu-id="79f43-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79f43-114">Application</span></span>                            | <span data-ttu-id="79f43-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="79f43-115">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79f43-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79f43-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUsageSummary
```

## <a name="function-parameters"></a><span data-ttu-id="79f43-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="79f43-117">Function parameters</span></span>

<span data-ttu-id="79f43-118">Você pode usar o seguinte parâmetro de função para ajustar a resposta.</span><span class="sxs-lookup"><span data-stu-id="79f43-118">You can use the following function parameter to adjust the response.</span></span>

| <span data-ttu-id="79f43-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="79f43-119">Parameter</span></span> | <span data-ttu-id="79f43-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="79f43-120">Type</span></span> | <span data-ttu-id="79f43-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="79f43-121">Description</span></span> |
|:--------- |:---- |:----------- |
| <span data-ttu-id="79f43-122">ponto</span><span class="sxs-lookup"><span data-stu-id="79f43-122">period</span></span> | <span data-ttu-id="79f43-123">String</span><span class="sxs-lookup"><span data-stu-id="79f43-123">String</span></span> | <span data-ttu-id="79f43-124">Especifica o período de tempo para o qual você precisa dos dados de uso.</span><span class="sxs-lookup"><span data-stu-id="79f43-124">Specifies the time period for which you need the usage data.</span></span> <span data-ttu-id="79f43-125">Por exemplo: `/reports/getCredentialUsageSummary(period='D30')`.</span><span class="sxs-lookup"><span data-stu-id="79f43-125">For example: `/reports/getCredentialUsageSummary(period='D30')`.</span></span> <span data-ttu-id="79f43-126">Períodos suportados: `D1`, `D7`, e `D30`.</span><span class="sxs-lookup"><span data-stu-id="79f43-126">Supported periods: `D1`, `D7`, and `D30`.</span></span> <span data-ttu-id="79f43-127">O período não diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="79f43-127">Period is case insensitive.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="79f43-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="79f43-128">Optional query parameters</span></span>

<span data-ttu-id="79f43-129">Essa função suporta o parâmetro de consulta OData opcional **$Filter**.</span><span class="sxs-lookup"><span data-stu-id="79f43-129">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="79f43-130">Você pode aplicar **$Filter** em uma ou mais das seguintes propriedades do recurso [credentialUsageSummary](../resources/credentialusagesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="79f43-130">You can apply **$filter** on one or more of the following properties of the [credentialUsageSummary](../resources/credentialusagesummary.md) resource.</span></span>

| <span data-ttu-id="79f43-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79f43-131">Properties</span></span> | <span data-ttu-id="79f43-132">Descrição e exemplo</span><span class="sxs-lookup"><span data-stu-id="79f43-132">Description and example</span></span> |
|:---- |:----------- |
| <span data-ttu-id="79f43-133">apresentam</span><span class="sxs-lookup"><span data-stu-id="79f43-133">feature</span></span> | <span data-ttu-id="79f43-134">Especifica o tipo de dados de uso que você deseja (registro versus redefinição).</span><span class="sxs-lookup"><span data-stu-id="79f43-134">Specifies the type of usage data you want (registration vs. reset).</span></span> <span data-ttu-id="79f43-135">Por exemplo: `/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'`.</span><span class="sxs-lookup"><span data-stu-id="79f43-135">For example: `/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="79f43-136">Operadores de filtro suportados `eq`:.</span><span class="sxs-lookup"><span data-stu-id="79f43-136">Supported filter operators: `eq`.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="79f43-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79f43-137">Request headers</span></span>

| <span data-ttu-id="79f43-138">Nome</span><span class="sxs-lookup"><span data-stu-id="79f43-138">Name</span></span>          | <span data-ttu-id="79f43-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="79f43-139">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="79f43-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="79f43-140">Authorization</span></span> | <span data-ttu-id="79f43-141">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="79f43-141">Bearer {token}</span></span> |
| <span data-ttu-id="79f43-142">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79f43-142">Content-Type</span></span> | <span data-ttu-id="79f43-143">application/json</span><span class="sxs-lookup"><span data-stu-id="79f43-143">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="79f43-144">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79f43-144">Request body</span></span>

<span data-ttu-id="79f43-145">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79f43-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79f43-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="79f43-146">Response</span></span>

<span data-ttu-id="79f43-147">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto da coleção [credentialUsageSummary](../resources/credentialusagesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79f43-147">If successful, this method returns a `200 OK` response code and a new [credentialUsageSummary](../resources/credentialusagesummary.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79f43-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="79f43-148">Examples</span></span>

<span data-ttu-id="79f43-149">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="79f43-149">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="79f43-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79f43-150">Request</span></span>

<span data-ttu-id="79f43-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="79f43-151">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="79f43-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="79f43-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialusagesummary"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="79f43-153">C#</span><span class="sxs-lookup"><span data-stu-id="79f43-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialusagesummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79f43-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79f43-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialusagesummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79f43-155">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="79f43-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialusagesummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="79f43-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="79f43-156">Response</span></span>

<span data-ttu-id="79f43-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79f43-157">The following is an example of the response.</span></span>

> <span data-ttu-id="79f43-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="79f43-158">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="79f43-159">Todas as propriedades são retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79f43-159">All the properties are returned from an actual call.</span></span>

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
