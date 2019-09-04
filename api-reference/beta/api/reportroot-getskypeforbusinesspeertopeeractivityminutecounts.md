---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: Obtenha tendências de uso da duração em minutos e tipo de sessões ponto a ponto realizadas em sua organização. Tipos de sessões incluem áudio e vídeo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 2bef6670f12126261fe5a6246244bcaf3847cf6a
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722766"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="45dd4-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="45dd4-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45dd4-105">Obtenha tendências de uso da duração em minutos e tipo de sessões ponto a ponto realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="45dd4-105">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="45dd4-106">Tipos de sessões incluem áudio e vídeo.</span><span class="sxs-lookup"><span data-stu-id="45dd4-106">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="45dd4-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade ponto a ponto do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="45dd4-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="45dd4-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="45dd4-108">Permissions</span></span>

<span data-ttu-id="45dd4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45dd4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="45dd4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45dd4-111">Permission type</span></span>                        | <span data-ttu-id="45dd4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45dd4-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="45dd4-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45dd4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="45dd4-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="45dd4-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="45dd4-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45dd4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45dd4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45dd4-116">Not supported.</span></span>                           |
| <span data-ttu-id="45dd4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45dd4-117">Application</span></span>                            | <span data-ttu-id="45dd4-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="45dd4-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="45dd4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45dd4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="45dd4-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="45dd4-120">Function parameters</span></span>

<span data-ttu-id="45dd4-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="45dd4-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="45dd4-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="45dd4-122">Parameter</span></span> | <span data-ttu-id="45dd4-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="45dd4-123">Type</span></span>   | <span data-ttu-id="45dd4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="45dd4-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="45dd4-125">ponto</span><span class="sxs-lookup"><span data-stu-id="45dd4-125">period</span></span>    | <span data-ttu-id="45dd4-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45dd4-126">string</span></span> | <span data-ttu-id="45dd4-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="45dd4-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="45dd4-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="45dd4-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="45dd4-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="45dd4-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="45dd4-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45dd4-130">Required.</span></span> |

<span data-ttu-id="45dd4-131">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="45dd4-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="45dd4-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="45dd4-132">The default output type is text/csv.</span></span> <span data-ttu-id="45dd4-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="45dd4-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45dd4-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45dd4-134">Request headers</span></span>

| <span data-ttu-id="45dd4-135">Nome</span><span class="sxs-lookup"><span data-stu-id="45dd4-135">Name</span></span>          | <span data-ttu-id="45dd4-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="45dd4-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="45dd4-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="45dd4-137">Authorization</span></span> | <span data-ttu-id="45dd4-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45dd4-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="45dd4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="45dd4-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="45dd4-141">CSV</span><span class="sxs-lookup"><span data-stu-id="45dd4-141">CSV</span></span>

<span data-ttu-id="45dd4-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="45dd4-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="45dd4-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="45dd4-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="45dd4-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="45dd4-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="45dd4-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="45dd4-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="45dd4-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="45dd4-146">Report Refresh Date</span></span>
- <span data-ttu-id="45dd4-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="45dd4-147">Report Date</span></span>
- <span data-ttu-id="45dd4-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="45dd4-148">Report Period</span></span>
- <span data-ttu-id="45dd4-149">Áudio</span><span class="sxs-lookup"><span data-stu-id="45dd4-149">Audio</span></span>
- <span data-ttu-id="45dd4-150">Vídeo</span><span class="sxs-lookup"><span data-stu-id="45dd4-150">Video</span></span>

### <a name="json"></a><span data-ttu-id="45dd4-151">JSON</span><span class="sxs-lookup"><span data-stu-id="45dd4-151">JSON</span></span>

<span data-ttu-id="45dd4-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45dd4-152">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45dd4-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45dd4-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="45dd4-154">CSV</span><span class="sxs-lookup"><span data-stu-id="45dd4-154">CSV</span></span>

<span data-ttu-id="45dd4-155">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="45dd4-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="45dd4-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45dd4-156">Request</span></span>

<span data-ttu-id="45dd4-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="45dd4-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="45dd4-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="45dd4-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="45dd4-159">C#</span><span class="sxs-lookup"><span data-stu-id="45dd4-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="45dd4-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45dd4-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="45dd4-161">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="45dd4-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="45dd4-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="45dd4-162">Response</span></span>

<span data-ttu-id="45dd4-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="45dd4-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="45dd4-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="45dd4-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio,Video
```

### <a name="json"></a><span data-ttu-id="45dd4-165">JSON</span><span class="sxs-lookup"><span data-stu-id="45dd4-165">JSON</span></span>

<span data-ttu-id="45dd4-166">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="45dd4-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="45dd4-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45dd4-167">Request</span></span>

<span data-ttu-id="45dd4-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="45dd4-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="45dd4-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="45dd4-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="45dd4-170">C#</span><span class="sxs-lookup"><span data-stu-id="45dd4-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="45dd4-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45dd4-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="45dd4-172">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="45dd4-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="45dd4-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="45dd4-173">Response</span></span>

<span data-ttu-id="45dd4-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="45dd4-174">The following is an example of the response.</span></span>

> <span data-ttu-id="45dd4-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45dd4-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts)", 
  "value": [
    {
      "audio": 836, 
      "video": 35, 
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
