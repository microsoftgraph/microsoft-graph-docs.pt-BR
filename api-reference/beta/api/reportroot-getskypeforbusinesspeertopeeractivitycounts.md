---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityCounts'
description: Obtenha tendências de uso no número e tipo de sessões realizadas em sua organização. Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7a208e909e3f155c7a5e35cccac2fc4aad914959
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358993"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivitycounts"></a><span data-ttu-id="4a31f-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="4a31f-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a31f-105">Obtenha tendências de uso no número e tipo de sessões realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="4a31f-105">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="4a31f-106">Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos.</span><span class="sxs-lookup"><span data-stu-id="4a31f-106">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span>

> <span data-ttu-id="4a31f-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade ponto a ponto do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="4a31f-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a31f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4a31f-108">Permissions</span></span>

<span data-ttu-id="4a31f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a31f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a31f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a31f-111">Permission type</span></span>                        | <span data-ttu-id="4a31f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a31f-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4a31f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a31f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a31f-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a31f-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4a31f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a31f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a31f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a31f-116">Not supported.</span></span>                           |
| <span data-ttu-id="4a31f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a31f-117">Application</span></span>                            | <span data-ttu-id="4a31f-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a31f-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4a31f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a31f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4a31f-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="4a31f-120">Function parameters</span></span>

<span data-ttu-id="4a31f-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="4a31f-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4a31f-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4a31f-122">Parameter</span></span> | <span data-ttu-id="4a31f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a31f-123">Type</span></span>   | <span data-ttu-id="4a31f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a31f-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4a31f-125">ponto</span><span class="sxs-lookup"><span data-stu-id="4a31f-125">period</span></span>    | <span data-ttu-id="4a31f-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a31f-126">string</span></span> | <span data-ttu-id="4a31f-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4a31f-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4a31f-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="4a31f-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4a31f-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4a31f-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4a31f-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a31f-130">Required.</span></span> |

<span data-ttu-id="4a31f-131">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4a31f-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4a31f-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="4a31f-132">The default output type is text/csv.</span></span> <span data-ttu-id="4a31f-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="4a31f-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a31f-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a31f-134">Request headers</span></span>

| <span data-ttu-id="4a31f-135">Nome</span><span class="sxs-lookup"><span data-stu-id="4a31f-135">Name</span></span>          | <span data-ttu-id="4a31f-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a31f-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4a31f-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a31f-137">Authorization</span></span> | <span data-ttu-id="4a31f-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a31f-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4a31f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a31f-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4a31f-141">CSV</span><span class="sxs-lookup"><span data-stu-id="4a31f-141">CSV</span></span>

<span data-ttu-id="4a31f-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="4a31f-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4a31f-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="4a31f-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4a31f-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4a31f-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4a31f-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="4a31f-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4a31f-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="4a31f-146">Report Refresh Date</span></span>
- <span data-ttu-id="4a31f-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="4a31f-147">Report Date</span></span>
- <span data-ttu-id="4a31f-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="4a31f-148">Report Period</span></span>
- <span data-ttu-id="4a31f-149">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="4a31f-149">IM</span></span>
- <span data-ttu-id="4a31f-150">Áudio</span><span class="sxs-lookup"><span data-stu-id="4a31f-150">Audio</span></span>
- <span data-ttu-id="4a31f-151">Vídeo</span><span class="sxs-lookup"><span data-stu-id="4a31f-151">Video</span></span>
- <span data-ttu-id="4a31f-152">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="4a31f-152">App Sharing</span></span>
- <span data-ttu-id="4a31f-153">Transferência de arquivos</span><span class="sxs-lookup"><span data-stu-id="4a31f-153">File Transfer</span></span>

### <a name="json"></a><span data-ttu-id="4a31f-154">JSON</span><span class="sxs-lookup"><span data-stu-id="4a31f-154">JSON</span></span>

<span data-ttu-id="4a31f-155">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a31f-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a31f-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a31f-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4a31f-157">CSV</span><span class="sxs-lookup"><span data-stu-id="4a31f-157">CSV</span></span>

<span data-ttu-id="4a31f-158">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="4a31f-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4a31f-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a31f-159">Request</span></span>

<span data-ttu-id="4a31f-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a31f-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4a31f-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a31f-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4a31f-162">C#</span><span class="sxs-lookup"><span data-stu-id="4a31f-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a31f-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a31f-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4a31f-164">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4a31f-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4a31f-165">Java</span><span class="sxs-lookup"><span data-stu-id="4a31f-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinesspeertopeeractivitycounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4a31f-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a31f-166">Response</span></span>

<span data-ttu-id="4a31f-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4a31f-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4a31f-168">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="4a31f-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
```

### <a name="json"></a><span data-ttu-id="4a31f-169">JSON</span><span class="sxs-lookup"><span data-stu-id="4a31f-169">JSON</span></span>

<span data-ttu-id="4a31f-170">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="4a31f-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4a31f-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a31f-171">Request</span></span>

<span data-ttu-id="4a31f-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a31f-172">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4a31f-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a31f-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4a31f-174">C#</span><span class="sxs-lookup"><span data-stu-id="4a31f-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a31f-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a31f-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4a31f-176">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4a31f-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4a31f-177">Java</span><span class="sxs-lookup"><span data-stu-id="4a31f-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinesspeertopeeractivitycounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4a31f-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a31f-178">Response</span></span>

<span data-ttu-id="4a31f-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4a31f-179">The following is an example of the response.</span></span>

> <span data-ttu-id="4a31f-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a31f-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityCounts)", 
  "value": [
    {
      "im": 1177, 
      "audio": 107, 
      "video": 7, 
      "appSharing": 74, 
      "fileTransfer": 24, 
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
