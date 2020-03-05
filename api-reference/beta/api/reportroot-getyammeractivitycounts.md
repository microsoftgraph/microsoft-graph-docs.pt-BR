---
title: 'reportRoot: getYammerActivityCounts'
description: Obtenha as tendências da quantidade de atividade do Yammer em sua organização por quantas mensagens foram postadas, lidas e curtidas.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: aa86597db27f2621f7a480cf7bc41229cb0737e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453993"
---
# <a name="reportroot-getyammeractivitycounts"></a><span data-ttu-id="0d1b9-103">reportRoot: getYammerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="0d1b9-103">reportRoot: getYammerActivityCounts</span></span>

<span data-ttu-id="0d1b9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0d1b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d1b9-105">Obtenha as tendências da quantidade de atividade do Yammer em sua organização por quantas mensagens foram postadas, lidas e curtidas.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-105">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span>

> <span data-ttu-id="0d1b9-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades do Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="0d1b9-106">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="0d1b9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d1b9-107">Permissions</span></span>

<span data-ttu-id="0d1b9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d1b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d1b9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d1b9-110">Permission type</span></span>                        | <span data-ttu-id="0d1b9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d1b9-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0d1b9-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d1b9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d1b9-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d1b9-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0d1b9-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d1b9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d1b9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-115">Not supported.</span></span>                           |
| <span data-ttu-id="0d1b9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d1b9-116">Application</span></span>                            | <span data-ttu-id="0d1b9-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d1b9-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="0d1b9-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="0d1b9-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="0d1b9-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="0d1b9-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d1b9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0d1b9-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="0d1b9-121">Function parameters</span></span>

<span data-ttu-id="0d1b9-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0d1b9-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0d1b9-123">Parameter</span></span> | <span data-ttu-id="0d1b9-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d1b9-124">Type</span></span>   | <span data-ttu-id="0d1b9-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d1b9-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0d1b9-126">ponto</span><span class="sxs-lookup"><span data-stu-id="0d1b9-126">period</span></span>    | <span data-ttu-id="0d1b9-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d1b9-127">string</span></span> | <span data-ttu-id="0d1b9-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0d1b9-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0d1b9-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0d1b9-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-131">Required.</span></span> |

<span data-ttu-id="0d1b9-132">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0d1b9-133">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-133">The default output type is text/csv.</span></span> <span data-ttu-id="0d1b9-134">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d1b9-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d1b9-135">Request headers</span></span>

| <span data-ttu-id="0d1b9-136">Nome</span><span class="sxs-lookup"><span data-stu-id="0d1b9-136">Name</span></span>          | <span data-ttu-id="0d1b9-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d1b9-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0d1b9-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d1b9-138">Authorization</span></span> | <span data-ttu-id="0d1b9-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0d1b9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d1b9-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0d1b9-142">CSV</span><span class="sxs-lookup"><span data-stu-id="0d1b9-142">CSV</span></span>

<span data-ttu-id="0d1b9-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0d1b9-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0d1b9-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0d1b9-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0d1b9-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="0d1b9-147">Report Refresh Date</span></span>
- <span data-ttu-id="0d1b9-148">Curtidos</span><span class="sxs-lookup"><span data-stu-id="0d1b9-148">Liked</span></span>
- <span data-ttu-id="0d1b9-149">Postados</span><span class="sxs-lookup"><span data-stu-id="0d1b9-149">Posted</span></span>
- <span data-ttu-id="0d1b9-150">Ler</span><span class="sxs-lookup"><span data-stu-id="0d1b9-150">Read</span></span>
- <span data-ttu-id="0d1b9-151">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="0d1b9-151">Report Date</span></span>
- <span data-ttu-id="0d1b9-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="0d1b9-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0d1b9-153">JSON</span><span class="sxs-lookup"><span data-stu-id="0d1b9-153">JSON</span></span>

<span data-ttu-id="0d1b9-154">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerActivitySummary](../resources/yammeractivitysummary.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-154">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d1b9-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d1b9-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0d1b9-156">CSV</span><span class="sxs-lookup"><span data-stu-id="0d1b9-156">CSV</span></span>

<span data-ttu-id="0d1b9-157">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0d1b9-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d1b9-158">Request</span></span>

<span data-ttu-id="0d1b9-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-159">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0d1b9-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d1b9-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityCounts(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="0d1b9-161">C#</span><span class="sxs-lookup"><span data-stu-id="0d1b9-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d1b9-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d1b9-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d1b9-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d1b9-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0d1b9-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d1b9-164">Response</span></span>

<span data-ttu-id="0d1b9-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0d1b9-166">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="0d1b9-167">JSON</span><span class="sxs-lookup"><span data-stu-id="0d1b9-167">JSON</span></span>

<span data-ttu-id="0d1b9-168">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0d1b9-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d1b9-169">Request</span></span>

<span data-ttu-id="0d1b9-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0d1b9-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d1b9-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityCounts(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="0d1b9-172">C#</span><span class="sxs-lookup"><span data-stu-id="0d1b9-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d1b9-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d1b9-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d1b9-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d1b9-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0d1b9-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d1b9-175">Response</span></span>

<span data-ttu-id="0d1b9-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-176">The following is an example of the response.</span></span>

> <span data-ttu-id="0d1b9-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d1b9-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 47, 
      "posted": 59, 
      "read": 986, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
