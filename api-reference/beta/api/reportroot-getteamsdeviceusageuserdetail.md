---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: f9a312cf29dc131c3b29d2f236ea32216a1dd268
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639135"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="397e0-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="397e0-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="397e0-104">Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="397e0-104">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="397e0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="397e0-105">Permissions</span></span>

<span data-ttu-id="397e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="397e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="397e0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="397e0-108">Permission type</span></span>                        | <span data-ttu-id="397e0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="397e0-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="397e0-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="397e0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="397e0-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="397e0-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="397e0-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="397e0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="397e0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="397e0-113">Not supported.</span></span>                           |
| <span data-ttu-id="397e0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="397e0-114">Application</span></span>                            | <span data-ttu-id="397e0-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="397e0-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="397e0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="397e0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="397e0-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="397e0-117">Function parameters</span></span>

<span data-ttu-id="397e0-118">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="397e0-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="397e0-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="397e0-119">Parameter</span></span> | <span data-ttu-id="397e0-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="397e0-120">Type</span></span>   | <span data-ttu-id="397e0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="397e0-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="397e0-122">ponto</span><span class="sxs-lookup"><span data-stu-id="397e0-122">period</span></span>    | <span data-ttu-id="397e0-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="397e0-123">string</span></span> | <span data-ttu-id="397e0-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="397e0-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="397e0-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="397e0-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="397e0-126">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="397e0-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="397e0-127">data</span><span class="sxs-lookup"><span data-stu-id="397e0-127">date</span></span>      | <span data-ttu-id="397e0-128">Data</span><span class="sxs-lookup"><span data-stu-id="397e0-128">Date</span></span>   | <span data-ttu-id="397e0-129">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="397e0-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="397e0-130">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="397e0-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="397e0-131">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="397e0-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="397e0-132">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="397e0-132">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="397e0-133">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="397e0-133">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="397e0-134">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="397e0-134">The default output type is text/csv.</span></span> <span data-ttu-id="397e0-135">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="397e0-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="397e0-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="397e0-136">Request headers</span></span>

| <span data-ttu-id="397e0-137">Nome</span><span class="sxs-lookup"><span data-stu-id="397e0-137">Name</span></span>          | <span data-ttu-id="397e0-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="397e0-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="397e0-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="397e0-139">Authorization</span></span> | <span data-ttu-id="397e0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="397e0-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="397e0-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="397e0-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="397e0-143">CSV</span><span class="sxs-lookup"><span data-stu-id="397e0-143">CSV</span></span>

<span data-ttu-id="397e0-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="397e0-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="397e0-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="397e0-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="397e0-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="397e0-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="397e0-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="397e0-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="397e0-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="397e0-148">Report Refresh Date</span></span>
- <span data-ttu-id="397e0-149">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="397e0-149">User Principal Name</span></span>
- <span data-ttu-id="397e0-150">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="397e0-150">Last Activity Date</span></span>
- <span data-ttu-id="397e0-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="397e0-151">Is Deleted</span></span>
- <span data-ttu-id="397e0-152">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="397e0-152">Deleted Date</span></span>
- <span data-ttu-id="397e0-153">Usou Web</span><span class="sxs-lookup"><span data-stu-id="397e0-153">Used Web</span></span>
- <span data-ttu-id="397e0-154">Usou Windows Phone</span><span class="sxs-lookup"><span data-stu-id="397e0-154">Used Windows Phone</span></span>
- <span data-ttu-id="397e0-155">Usou iOS</span><span class="sxs-lookup"><span data-stu-id="397e0-155">Used iOS</span></span>
- <span data-ttu-id="397e0-156">Usou Mac</span><span class="sxs-lookup"><span data-stu-id="397e0-156">Used Mac</span></span>
- <span data-ttu-id="397e0-157">Usou telefone Android</span><span class="sxs-lookup"><span data-stu-id="397e0-157">Used Android Phone</span></span>
- <span data-ttu-id="397e0-158">Usou Windows</span><span class="sxs-lookup"><span data-stu-id="397e0-158">Used Windows</span></span>
- <span data-ttu-id="397e0-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="397e0-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="397e0-160">JSON</span><span class="sxs-lookup"><span data-stu-id="397e0-160">JSON</span></span>

<span data-ttu-id="397e0-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="397e0-161">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="397e0-162">O tamanho de página padrão para essa solicitação é de 2000 itens.</span><span class="sxs-lookup"><span data-stu-id="397e0-162">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="397e0-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="397e0-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="397e0-164">CSV</span><span class="sxs-lookup"><span data-stu-id="397e0-164">CSV</span></span>

<span data-ttu-id="397e0-165">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="397e0-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="397e0-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="397e0-166">Request</span></span>

<span data-ttu-id="397e0-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="397e0-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="397e0-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="397e0-168">Response</span></span>

<span data-ttu-id="397e0-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="397e0-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="397e0-170">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="397e0-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="397e0-171">Basic</span><span class="sxs-lookup"><span data-stu-id="397e0-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusageuserdetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="397e0-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="397e0-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusageuserdetail_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="397e0-173">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="397e0-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="397e0-174">JSON</span><span class="sxs-lookup"><span data-stu-id="397e0-174">JSON</span></span>

<span data-ttu-id="397e0-175">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="397e0-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="397e0-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="397e0-176">Request</span></span>

<span data-ttu-id="397e0-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="397e0-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="397e0-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="397e0-178">Response</span></span>

<span data-ttu-id="397e0-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="397e0-179">The following is an example of the response.</span></span>

> <span data-ttu-id="397e0-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="397e0-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="397e0-182">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="397e0-182">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="397e0-183">Basic</span><span class="sxs-lookup"><span data-stu-id="397e0-183">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusageuserdetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="397e0-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="397e0-184">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusageuserdetail_json-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
