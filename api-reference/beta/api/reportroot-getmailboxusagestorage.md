---
title: 'reportRoot: getMailboxUsageStorage'
description: Obtenha a quantidade de armazenamento usada em sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 8978424f583990ff0d4bb497c836d85e7a983e65
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411771"
---
# <a name="reportroot-getmailboxusagestorage"></a><span data-ttu-id="4fe60-103">reportRoot: getMailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="4fe60-103">reportRoot: getMailboxUsageStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fe60-104">Obtenha a quantidade de armazenamento usada em sua organização.</span><span class="sxs-lookup"><span data-stu-id="4fe60-104">Get the amount of storage used in your organization.</span></span>

> <span data-ttu-id="4fe60-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="4fe60-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="4fe60-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4fe60-106">Permissions</span></span>

<span data-ttu-id="4fe60-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fe60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4fe60-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4fe60-109">Permission type</span></span>                        | <span data-ttu-id="4fe60-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4fe60-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4fe60-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4fe60-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4fe60-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fe60-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4fe60-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4fe60-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fe60-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4fe60-114">Not supported.</span></span>                           |
| <span data-ttu-id="4fe60-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4fe60-115">Application</span></span>                            | <span data-ttu-id="4fe60-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fe60-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4fe60-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4fe60-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4fe60-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="4fe60-118">Function parameters</span></span>

<span data-ttu-id="4fe60-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="4fe60-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4fe60-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4fe60-120">Parameter</span></span> | <span data-ttu-id="4fe60-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4fe60-121">Type</span></span>   | <span data-ttu-id="4fe60-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fe60-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4fe60-123">ponto</span><span class="sxs-lookup"><span data-stu-id="4fe60-123">period</span></span>    | <span data-ttu-id="4fe60-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4fe60-124">string</span></span> | <span data-ttu-id="4fe60-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4fe60-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4fe60-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="4fe60-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4fe60-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4fe60-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4fe60-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4fe60-128">Required.</span></span> |

<span data-ttu-id="4fe60-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4fe60-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4fe60-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="4fe60-130">The default output type is text/csv.</span></span> <span data-ttu-id="4fe60-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="4fe60-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4fe60-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4fe60-132">Request headers</span></span>

| <span data-ttu-id="4fe60-133">Nome</span><span class="sxs-lookup"><span data-stu-id="4fe60-133">Name</span></span>          | <span data-ttu-id="4fe60-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fe60-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4fe60-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="4fe60-135">Authorization</span></span> | <span data-ttu-id="4fe60-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4fe60-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4fe60-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fe60-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4fe60-139">CSV</span><span class="sxs-lookup"><span data-stu-id="4fe60-139">CSV</span></span>

<span data-ttu-id="4fe60-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="4fe60-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4fe60-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="4fe60-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4fe60-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4fe60-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4fe60-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="4fe60-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4fe60-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="4fe60-144">Report Refresh Date</span></span>
- <span data-ttu-id="4fe60-145">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="4fe60-145">Storage Used (Byte)</span></span>
- <span data-ttu-id="4fe60-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="4fe60-146">Report Date</span></span>
- <span data-ttu-id="4fe60-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="4fe60-147">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4fe60-148">JSON</span><span class="sxs-lookup"><span data-stu-id="4fe60-148">JSON</span></span>

<span data-ttu-id="4fe60-149">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[mailboxUsageStorage](../resources/mailboxusagestorage.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4fe60-149">If successful, this method returns a `200 OK` response code and a **[mailboxUsageStorage](../resources/mailboxusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fe60-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4fe60-150">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4fe60-151">CSV</span><span class="sxs-lookup"><span data-stu-id="4fe60-151">CSV</span></span>

<span data-ttu-id="4fe60-152">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="4fe60-152">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4fe60-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4fe60-153">Request</span></span>

<span data-ttu-id="4fe60-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4fe60-154">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4fe60-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="4fe60-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagestorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageStorage(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4fe60-156">C#</span><span class="sxs-lookup"><span data-stu-id="4fe60-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagestorage-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4fe60-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4fe60-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagestorage-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4fe60-158">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4fe60-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagestorage-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4fe60-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fe60-159">Response</span></span>

<span data-ttu-id="4fe60-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4fe60-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4fe60-161">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="4fe60-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="4fe60-162">JSON</span><span class="sxs-lookup"><span data-stu-id="4fe60-162">JSON</span></span>

<span data-ttu-id="4fe60-163">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="4fe60-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4fe60-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4fe60-164">Request</span></span>

<span data-ttu-id="4fe60-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4fe60-165">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4fe60-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="4fe60-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagestorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageStorage(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4fe60-167">C#</span><span class="sxs-lookup"><span data-stu-id="4fe60-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagestorage-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4fe60-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4fe60-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagestorage-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4fe60-169">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4fe60-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagestorage-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4fe60-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fe60-170">Response</span></span>

<span data-ttu-id="4fe60-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4fe60-171">The following is an example of the response.</span></span>

> <span data-ttu-id="4fe60-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4fe60-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 235

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "storageUsedInBytes": 5159432679270, 
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
