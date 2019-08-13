---
title: 'reportRoot: getSkypeForBusinessActivityUserCounts'
description: Obtenha as tendências de quantos usuários únicos organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business. O relatório também inclui o número de sessões ponto a ponto.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: b4d6c70f2c6dc8045696982ec2b402a2d899076c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359653"
---
# <a name="reportroot-getskypeforbusinessactivityusercounts"></a><span data-ttu-id="78f54-104">reportRoot: getSkypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="78f54-104">reportRoot: getSkypeForBusinessActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78f54-105">Obtenha as tendências de quantos usuários únicos organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="78f54-105">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="78f54-106">O relatório também inclui o número de sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="78f54-106">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="78f54-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="78f54-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="78f54-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="78f54-108">Permissions</span></span>

<span data-ttu-id="78f54-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78f54-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="78f54-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78f54-111">Permission type</span></span>                        | <span data-ttu-id="78f54-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78f54-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="78f54-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78f54-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="78f54-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="78f54-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="78f54-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78f54-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78f54-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78f54-116">Not supported.</span></span>                           |
| <span data-ttu-id="78f54-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78f54-117">Application</span></span>                            | <span data-ttu-id="78f54-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="78f54-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="78f54-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78f54-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="78f54-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="78f54-120">Function parameters</span></span>

<span data-ttu-id="78f54-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="78f54-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="78f54-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="78f54-122">Parameter</span></span> | <span data-ttu-id="78f54-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="78f54-123">Type</span></span>   | <span data-ttu-id="78f54-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="78f54-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="78f54-125">ponto</span><span class="sxs-lookup"><span data-stu-id="78f54-125">period</span></span>    | <span data-ttu-id="78f54-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78f54-126">string</span></span> | <span data-ttu-id="78f54-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="78f54-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="78f54-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="78f54-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="78f54-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="78f54-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="78f54-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78f54-130">Required.</span></span> |

<span data-ttu-id="78f54-131">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="78f54-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="78f54-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="78f54-132">The default output type is text/csv.</span></span> <span data-ttu-id="78f54-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="78f54-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78f54-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78f54-134">Request headers</span></span>

| <span data-ttu-id="78f54-135">Nome</span><span class="sxs-lookup"><span data-stu-id="78f54-135">Name</span></span>          | <span data-ttu-id="78f54-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="78f54-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="78f54-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="78f54-137">Authorization</span></span> | <span data-ttu-id="78f54-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78f54-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="78f54-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="78f54-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="78f54-141">CSV</span><span class="sxs-lookup"><span data-stu-id="78f54-141">CSV</span></span>

<span data-ttu-id="78f54-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="78f54-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="78f54-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="78f54-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="78f54-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="78f54-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="78f54-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="78f54-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="78f54-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="78f54-146">Report Refresh Date</span></span>
- <span data-ttu-id="78f54-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="78f54-147">Report Date</span></span>
- <span data-ttu-id="78f54-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="78f54-148">Report Period</span></span>
- <span data-ttu-id="78f54-149">Ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="78f54-149">Peer-to-peer</span></span>
- <span data-ttu-id="78f54-150">Organizadas</span><span class="sxs-lookup"><span data-stu-id="78f54-150">Organized</span></span>
- <span data-ttu-id="78f54-151">Participadas</span><span class="sxs-lookup"><span data-stu-id="78f54-151">Participated</span></span>

### <a name="json"></a><span data-ttu-id="78f54-152">JSON</span><span class="sxs-lookup"><span data-stu-id="78f54-152">JSON</span></span>

<span data-ttu-id="78f54-153">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78f54-153">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78f54-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78f54-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="78f54-155">CSV</span><span class="sxs-lookup"><span data-stu-id="78f54-155">CSV</span></span>

<span data-ttu-id="78f54-156">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="78f54-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="78f54-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78f54-157">Request</span></span>

<span data-ttu-id="78f54-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="78f54-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="78f54-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="78f54-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="78f54-160">C#</span><span class="sxs-lookup"><span data-stu-id="78f54-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="78f54-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78f54-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="78f54-162">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="78f54-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="78f54-163">Java</span><span class="sxs-lookup"><span data-stu-id="78f54-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessactivityusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="78f54-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="78f54-164">Response</span></span>

<span data-ttu-id="78f54-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="78f54-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="78f54-166">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="78f54-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
```

### <a name="json"></a><span data-ttu-id="78f54-167">JSON</span><span class="sxs-lookup"><span data-stu-id="78f54-167">JSON</span></span>

<span data-ttu-id="78f54-168">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="78f54-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="78f54-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78f54-169">Request</span></span>

<span data-ttu-id="78f54-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="78f54-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="78f54-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="78f54-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="78f54-172">C#</span><span class="sxs-lookup"><span data-stu-id="78f54-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="78f54-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78f54-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="78f54-174">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="78f54-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="78f54-175">Java</span><span class="sxs-lookup"><span data-stu-id="78f54-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessactivityusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="78f54-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="78f54-176">Response</span></span>

<span data-ttu-id="78f54-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="78f54-177">The following is an example of the response.</span></span>

> <span data-ttu-id="78f54-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78f54-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 266

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessActivityUserCounts)", 
  "value": [
    {
      "peerToPeer": 413, 
      "organized": 30, 
      "participated": 91, 
      "reportRefreshDate": "2017-09-01", 
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
