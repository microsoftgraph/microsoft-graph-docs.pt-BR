---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Obtenha a tendência no número de usuários ativos. Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 120ca2f005c61fec03fe8667729e9eda52790502
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411470"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="d5c87-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="d5c87-104">reportRoot: getSharePointActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5c87-105">Obtenha a tendência no número de usuários ativos.</span><span class="sxs-lookup"><span data-stu-id="d5c87-105">Get the trend in the number of active users.</span></span> <span data-ttu-id="d5c87-106">Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="d5c87-106">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="d5c87-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="d5c87-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="d5c87-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5c87-108">Permissions</span></span>

<span data-ttu-id="d5c87-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5c87-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5c87-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5c87-111">Permission type</span></span>                        | <span data-ttu-id="d5c87-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5c87-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d5c87-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5c87-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5c87-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c87-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d5c87-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5c87-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5c87-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5c87-116">Not supported.</span></span>                           |
| <span data-ttu-id="d5c87-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5c87-117">Application</span></span>                            | <span data-ttu-id="d5c87-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c87-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d5c87-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5c87-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d5c87-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d5c87-120">Function parameters</span></span>

<span data-ttu-id="d5c87-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d5c87-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d5c87-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d5c87-122">Parameter</span></span> | <span data-ttu-id="d5c87-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5c87-123">Type</span></span>   | <span data-ttu-id="d5c87-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5c87-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d5c87-125">ponto</span><span class="sxs-lookup"><span data-stu-id="d5c87-125">period</span></span>    | <span data-ttu-id="d5c87-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5c87-126">string</span></span> | <span data-ttu-id="d5c87-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d5c87-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d5c87-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="d5c87-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d5c87-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d5c87-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d5c87-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5c87-130">Required.</span></span> |

<span data-ttu-id="d5c87-131">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d5c87-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d5c87-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="d5c87-132">The default output type is text/csv.</span></span> <span data-ttu-id="d5c87-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="d5c87-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5c87-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5c87-134">Request headers</span></span>

| <span data-ttu-id="d5c87-135">Nome</span><span class="sxs-lookup"><span data-stu-id="d5c87-135">Name</span></span>          | <span data-ttu-id="d5c87-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5c87-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d5c87-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5c87-137">Authorization</span></span> | <span data-ttu-id="d5c87-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5c87-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d5c87-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5c87-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d5c87-141">CSV</span><span class="sxs-lookup"><span data-stu-id="d5c87-141">CSV</span></span>

<span data-ttu-id="d5c87-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d5c87-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d5c87-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d5c87-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d5c87-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d5c87-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d5c87-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d5c87-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d5c87-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d5c87-146">Report Refresh Date</span></span>
- <span data-ttu-id="d5c87-147">Página visitada</span><span class="sxs-lookup"><span data-stu-id="d5c87-147">Visited Page</span></span>
- <span data-ttu-id="d5c87-148">Exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="d5c87-148">Viewed Or Edited</span></span>
- <span data-ttu-id="d5c87-149">Sincronizados</span><span class="sxs-lookup"><span data-stu-id="d5c87-149">Synced</span></span>
- <span data-ttu-id="d5c87-150">Compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="d5c87-150">Shared Internally</span></span>
- <span data-ttu-id="d5c87-151">Compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="d5c87-151">Shared Externally</span></span>
- <span data-ttu-id="d5c87-152">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="d5c87-152">Report Date</span></span>
- <span data-ttu-id="d5c87-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="d5c87-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d5c87-154">JSON</span><span class="sxs-lookup"><span data-stu-id="d5c87-154">JSON</span></span>

<span data-ttu-id="d5c87-155">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5c87-155">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5c87-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5c87-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d5c87-157">CSV</span><span class="sxs-lookup"><span data-stu-id="d5c87-157">CSV</span></span>

<span data-ttu-id="d5c87-158">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="d5c87-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d5c87-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5c87-159">Request</span></span>

<span data-ttu-id="d5c87-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5c87-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d5c87-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5c87-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d5c87-162">C#</span><span class="sxs-lookup"><span data-stu-id="d5c87-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5c87-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5c87-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d5c87-164">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d5c87-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d5c87-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5c87-165">Response</span></span>

<span data-ttu-id="d5c87-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d5c87-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d5c87-167">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d5c87-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="d5c87-168">JSON</span><span class="sxs-lookup"><span data-stu-id="d5c87-168">JSON</span></span>

<span data-ttu-id="d5c87-169">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="d5c87-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d5c87-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5c87-170">Request</span></span>

<span data-ttu-id="d5c87-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5c87-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d5c87-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5c87-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d5c87-173">C#</span><span class="sxs-lookup"><span data-stu-id="d5c87-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5c87-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5c87-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d5c87-175">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d5c87-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d5c87-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5c87-176">Response</span></span>

<span data-ttu-id="d5c87-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d5c87-177">The following is an example of the response.</span></span>

> <span data-ttu-id="d5c87-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5c87-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPage": 56, 
      "viewedOrEdited": 163, 
      "synced": 7, 
      "sharedInternally": 10, 
      "sharedExternally": 1, 
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
