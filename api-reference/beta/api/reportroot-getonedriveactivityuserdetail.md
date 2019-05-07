---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: Obtenha dados sobre as atividades do OneDrive por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 95c07673d5ee5cec26fbf1737baaf8207e2b2e9c
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639366"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="dcc14-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="dcc14-103">reportRoot: getOneDriveActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcc14-104">Obtenha dados sobre as atividades do OneDrive por usuário.</span><span class="sxs-lookup"><span data-stu-id="dcc14-104">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="dcc14-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="dcc14-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="dcc14-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dcc14-106">Permissions</span></span>

<span data-ttu-id="dcc14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcc14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dcc14-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dcc14-109">Permission type</span></span>                        | <span data-ttu-id="dcc14-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dcc14-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dcc14-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dcc14-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dcc14-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcc14-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="dcc14-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dcc14-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcc14-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcc14-114">Not supported.</span></span>                           |
| <span data-ttu-id="dcc14-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dcc14-115">Application</span></span>                            | <span data-ttu-id="dcc14-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcc14-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="dcc14-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcc14-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="dcc14-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="dcc14-118">Function parameters</span></span>

<span data-ttu-id="dcc14-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="dcc14-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="dcc14-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dcc14-120">Parameter</span></span> | <span data-ttu-id="dcc14-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="dcc14-121">Type</span></span>   | <span data-ttu-id="dcc14-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcc14-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="dcc14-123">ponto</span><span class="sxs-lookup"><span data-stu-id="dcc14-123">period</span></span>    | <span data-ttu-id="dcc14-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dcc14-124">string</span></span> | <span data-ttu-id="dcc14-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="dcc14-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="dcc14-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="dcc14-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="dcc14-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="dcc14-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="dcc14-128">data</span><span class="sxs-lookup"><span data-stu-id="dcc14-128">date</span></span>      | <span data-ttu-id="dcc14-129">Data</span><span class="sxs-lookup"><span data-stu-id="dcc14-129">Date</span></span>   | <span data-ttu-id="dcc14-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="dcc14-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="dcc14-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="dcc14-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="dcc14-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="dcc14-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="dcc14-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="dcc14-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="dcc14-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="dcc14-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="dcc14-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="dcc14-135">The default output type is text/csv.</span></span> <span data-ttu-id="dcc14-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="dcc14-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcc14-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcc14-137">Request headers</span></span>

| <span data-ttu-id="dcc14-138">Nome</span><span class="sxs-lookup"><span data-stu-id="dcc14-138">Name</span></span>          | <span data-ttu-id="dcc14-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcc14-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="dcc14-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcc14-140">Authorization</span></span> | <span data-ttu-id="dcc14-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcc14-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="dcc14-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcc14-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="dcc14-144">CSV</span><span class="sxs-lookup"><span data-stu-id="dcc14-144">CSV</span></span>

<span data-ttu-id="dcc14-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="dcc14-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dcc14-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="dcc14-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dcc14-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="dcc14-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="dcc14-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="dcc14-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="dcc14-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="dcc14-149">Report Refresh Date</span></span>
- <span data-ttu-id="dcc14-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="dcc14-150">User Principal Name</span></span>
- <span data-ttu-id="dcc14-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="dcc14-151">Is Deleted</span></span>
- <span data-ttu-id="dcc14-152">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="dcc14-152">Deleted Date</span></span>
- <span data-ttu-id="dcc14-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="dcc14-153">Last Activity Date</span></span>
- <span data-ttu-id="dcc14-154">Contagem de arquivos exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="dcc14-154">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="dcc14-155">Contagem de arquivos sincronizados</span><span class="sxs-lookup"><span data-stu-id="dcc14-155">Synced File Count</span></span>
- <span data-ttu-id="dcc14-156">Contagem de arquivos compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="dcc14-156">Shared Internally File Count</span></span>
- <span data-ttu-id="dcc14-157">Contagem de arquivos compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="dcc14-157">Shared Externally File Count</span></span>
- <span data-ttu-id="dcc14-158">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="dcc14-158">Assigned Products</span></span>
- <span data-ttu-id="dcc14-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="dcc14-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="dcc14-160">JSON</span><span class="sxs-lookup"><span data-stu-id="dcc14-160">JSON</span></span>

<span data-ttu-id="dcc14-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dcc14-161">If successful, this method returns a `200 OK` response code and a **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="dcc14-162">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="dcc14-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="dcc14-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dcc14-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="dcc14-164">CSV</span><span class="sxs-lookup"><span data-stu-id="dcc14-164">CSV</span></span>

<span data-ttu-id="dcc14-165">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="dcc14-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="dcc14-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcc14-166">Request</span></span>

<span data-ttu-id="dcc14-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcc14-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="dcc14-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcc14-168">Response</span></span>

<span data-ttu-id="dcc14-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dcc14-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dcc14-170">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="dcc14-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dcc14-171">Basic</span><span class="sxs-lookup"><span data-stu-id="dcc14-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityuserdetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dcc14-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcc14-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityuserdetail_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="dcc14-173">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="dcc14-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="dcc14-174">JSON</span><span class="sxs-lookup"><span data-stu-id="dcc14-174">JSON</span></span>

<span data-ttu-id="dcc14-175">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="dcc14-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="dcc14-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcc14-176">Request</span></span>

<span data-ttu-id="dcc14-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcc14-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="dcc14-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcc14-178">Response</span></span>

<span data-ttu-id="dcc14-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dcc14-179">The following is an example of the response.</span></span>

> <span data-ttu-id="dcc14-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dcc14-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "viewedOrEditedFileCount": 1, 
      "syncedFileCount": 0, 
      "sharedInternallyFileCount": 0, 
      "sharedExternallyFileCount": 0, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dcc14-182">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="dcc14-182">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dcc14-183">Basic</span><span class="sxs-lookup"><span data-stu-id="dcc14-183">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityuserdetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dcc14-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcc14-184">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityuserdetail_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
