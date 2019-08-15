---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 83d13672b1b69807e48aa426e02e74b740deba26
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411134"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="f3234-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="f3234-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3234-104">Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="f3234-104">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3234-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f3234-105">Permissions</span></span>

<span data-ttu-id="f3234-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3234-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f3234-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3234-108">Permission type</span></span>                        | <span data-ttu-id="f3234-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3234-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f3234-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3234-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f3234-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3234-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f3234-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3234-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3234-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3234-113">Not supported.</span></span>                           |
| <span data-ttu-id="f3234-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3234-114">Application</span></span>                            | <span data-ttu-id="f3234-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3234-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f3234-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3234-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="f3234-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="f3234-117">Function parameters</span></span>

<span data-ttu-id="f3234-118">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f3234-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="f3234-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f3234-119">Parameter</span></span> | <span data-ttu-id="f3234-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3234-120">Type</span></span>   | <span data-ttu-id="f3234-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3234-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f3234-122">ponto</span><span class="sxs-lookup"><span data-stu-id="f3234-122">period</span></span>    | <span data-ttu-id="f3234-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3234-123">string</span></span> | <span data-ttu-id="f3234-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f3234-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f3234-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="f3234-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f3234-126">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f3234-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="f3234-127">data</span><span class="sxs-lookup"><span data-stu-id="f3234-127">date</span></span>      | <span data-ttu-id="f3234-128">Data</span><span class="sxs-lookup"><span data-stu-id="f3234-128">Date</span></span>   | <span data-ttu-id="f3234-129">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="f3234-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="f3234-130">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="f3234-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="f3234-131">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="f3234-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="f3234-132">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="f3234-132">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="f3234-133">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="f3234-133">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f3234-134">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="f3234-134">The default output type is text/csv.</span></span> <span data-ttu-id="f3234-135">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="f3234-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3234-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3234-136">Request headers</span></span>

| <span data-ttu-id="f3234-137">Nome</span><span class="sxs-lookup"><span data-stu-id="f3234-137">Name</span></span>          | <span data-ttu-id="f3234-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3234-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f3234-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3234-139">Authorization</span></span> | <span data-ttu-id="f3234-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3234-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f3234-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3234-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f3234-143">CSV</span><span class="sxs-lookup"><span data-stu-id="f3234-143">CSV</span></span>

<span data-ttu-id="f3234-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="f3234-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f3234-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="f3234-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f3234-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f3234-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f3234-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="f3234-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f3234-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="f3234-148">Report Refresh Date</span></span>
- <span data-ttu-id="f3234-149">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="f3234-149">User Principal Name</span></span>
- <span data-ttu-id="f3234-150">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="f3234-150">Last Activity Date</span></span>
- <span data-ttu-id="f3234-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="f3234-151">Is Deleted</span></span>
- <span data-ttu-id="f3234-152">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="f3234-152">Deleted Date</span></span>
- <span data-ttu-id="f3234-153">Usou Web</span><span class="sxs-lookup"><span data-stu-id="f3234-153">Used Web</span></span>
- <span data-ttu-id="f3234-154">Usou Windows Phone</span><span class="sxs-lookup"><span data-stu-id="f3234-154">Used Windows Phone</span></span>
- <span data-ttu-id="f3234-155">Usou iOS</span><span class="sxs-lookup"><span data-stu-id="f3234-155">Used iOS</span></span>
- <span data-ttu-id="f3234-156">Usou Mac</span><span class="sxs-lookup"><span data-stu-id="f3234-156">Used Mac</span></span>
- <span data-ttu-id="f3234-157">Usou telefone Android</span><span class="sxs-lookup"><span data-stu-id="f3234-157">Used Android Phone</span></span>
- <span data-ttu-id="f3234-158">Usou Windows</span><span class="sxs-lookup"><span data-stu-id="f3234-158">Used Windows</span></span>
- <span data-ttu-id="f3234-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="f3234-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="f3234-160">JSON</span><span class="sxs-lookup"><span data-stu-id="f3234-160">JSON</span></span>

<span data-ttu-id="f3234-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3234-161">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="f3234-162">O tamanho de página padrão para essa solicitação é de 2000 itens.</span><span class="sxs-lookup"><span data-stu-id="f3234-162">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="f3234-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3234-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f3234-164">CSV</span><span class="sxs-lookup"><span data-stu-id="f3234-164">CSV</span></span>

<span data-ttu-id="f3234-165">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="f3234-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f3234-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3234-166">Request</span></span>

<span data-ttu-id="f3234-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3234-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f3234-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3234-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f3234-169">C#</span><span class="sxs-lookup"><span data-stu-id="f3234-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f3234-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f3234-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f3234-171">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f3234-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f3234-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3234-172">Response</span></span>

<span data-ttu-id="f3234-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f3234-173">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f3234-174">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="f3234-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="f3234-175">JSON</span><span class="sxs-lookup"><span data-stu-id="f3234-175">JSON</span></span>

<span data-ttu-id="f3234-176">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="f3234-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f3234-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3234-177">Request</span></span>

<span data-ttu-id="f3234-178">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3234-178">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f3234-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3234-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f3234-180">C#</span><span class="sxs-lookup"><span data-stu-id="f3234-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f3234-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f3234-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f3234-182">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f3234-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f3234-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3234-183">Response</span></span>

<span data-ttu-id="f3234-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f3234-184">The following is an example of the response.</span></span>

> <span data-ttu-id="f3234-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3234-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "usedWeb": false, 
      "usedWindowsPhone": false, 
      "usediOS": true, 
      "usedMac": false, 
      "usedAndroidPhone": false, 
      "usedWindows": true, 
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
