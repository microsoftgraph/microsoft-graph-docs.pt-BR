---
title: 'reportRoot: getOneDriveUsageStorage'
description: Obtenha a tendência da quantidade de armazenamento que você está usando no OneDrive for Business.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 656e1980e98cc713c97b3e2154145c043e792d8b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872904"
---
# <a name="reportroot-getonedriveusagestorage"></a><span data-ttu-id="b3753-103">reportRoot: getOneDriveUsageStorage</span><span class="sxs-lookup"><span data-stu-id="b3753-103">reportRoot: getOneDriveUsageStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3753-104">Obtenha a tendência da quantidade de armazenamento que você está usando no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="b3753-104">Get the trend on the amount of storage you are using in OneDrive for Business.</span></span>

> <span data-ttu-id="b3753-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="b3753-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="b3753-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3753-106">Permissions</span></span>

<span data-ttu-id="b3753-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3753-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3753-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3753-109">Permission type</span></span>                        | <span data-ttu-id="b3753-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3753-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b3753-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3753-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3753-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3753-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b3753-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3753-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3753-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3753-114">Not supported.</span></span>                           |
| <span data-ttu-id="b3753-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3753-115">Application</span></span>                            | <span data-ttu-id="b3753-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3753-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b3753-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3753-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b3753-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b3753-118">Function parameters</span></span>

<span data-ttu-id="b3753-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="b3753-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b3753-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b3753-120">Parameter</span></span> | <span data-ttu-id="b3753-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3753-121">Type</span></span>   | <span data-ttu-id="b3753-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3753-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b3753-123">ponto</span><span class="sxs-lookup"><span data-stu-id="b3753-123">period</span></span>    | <span data-ttu-id="b3753-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3753-124">string</span></span> | <span data-ttu-id="b3753-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b3753-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b3753-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="b3753-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b3753-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b3753-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b3753-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3753-128">Required.</span></span> |

<span data-ttu-id="b3753-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b3753-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b3753-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="b3753-130">The default output type is text/csv.</span></span> <span data-ttu-id="b3753-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="b3753-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3753-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3753-132">Request headers</span></span>

| <span data-ttu-id="b3753-133">Nome</span><span class="sxs-lookup"><span data-stu-id="b3753-133">Name</span></span>          | <span data-ttu-id="b3753-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3753-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b3753-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3753-135">Authorization</span></span> | <span data-ttu-id="b3753-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3753-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b3753-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3753-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b3753-139">CSV</span><span class="sxs-lookup"><span data-stu-id="b3753-139">CSV</span></span>

<span data-ttu-id="b3753-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="b3753-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b3753-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="b3753-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b3753-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b3753-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b3753-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="b3753-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b3753-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="b3753-144">Report Refresh Date</span></span>
- <span data-ttu-id="b3753-145">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="b3753-145">Site Type</span></span>
- <span data-ttu-id="b3753-146">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="b3753-146">Storage Used (Byte)</span></span>
- <span data-ttu-id="b3753-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="b3753-147">Report Date</span></span>
- <span data-ttu-id="b3753-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="b3753-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="b3753-149">JSON</span><span class="sxs-lookup"><span data-stu-id="b3753-149">JSON</span></span>

<span data-ttu-id="b3753-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[siteUsageStorage](../resources/siteusagestorage.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3753-150">If successful, this method returns a `200 OK` response code and a **[siteUsageStorage](../resources/siteusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3753-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3753-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b3753-152">CSV</span><span class="sxs-lookup"><span data-stu-id="b3753-152">CSV</span></span>

<span data-ttu-id="b3753-153">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="b3753-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b3753-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3753-154">Request</span></span>

<span data-ttu-id="b3753-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3753-155">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b3753-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3753-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagestorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageStorage(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b3753-157">C#</span><span class="sxs-lookup"><span data-stu-id="b3753-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusagestorage-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b3753-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="b3753-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusagestorage-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b3753-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b3753-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusagestorage-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b3753-160">Java</span><span class="sxs-lookup"><span data-stu-id="b3753-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveusagestorage-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b3753-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3753-161">Response</span></span>

<span data-ttu-id="b3753-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3753-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b3753-163">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="b3753-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="b3753-164">JSON</span><span class="sxs-lookup"><span data-stu-id="b3753-164">JSON</span></span>

<span data-ttu-id="b3753-165">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="b3753-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b3753-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3753-166">Request</span></span>

<span data-ttu-id="b3753-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3753-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b3753-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3753-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagestorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageStorage(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b3753-169">C#</span><span class="sxs-lookup"><span data-stu-id="b3753-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusagestorage-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b3753-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="b3753-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusagestorage-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b3753-171">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b3753-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusagestorage-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b3753-172">Java</span><span class="sxs-lookup"><span data-stu-id="b3753-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveusagestorage-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b3753-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3753-173">Response</span></span>

<span data-ttu-id="b3753-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3753-174">The following is an example of the response.</span></span>

> <span data-ttu-id="b3753-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3753-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteUsageStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "storageUsedInBytes": 132654293197, 
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
