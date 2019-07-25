---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: Obtenha dados sobre as atividades do OneDrive por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e5b91ea48c79ee7ea9a53bb5337a65d01703e8ed
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873057"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="9cc8d-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="9cc8d-103">reportRoot: getOneDriveActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cc8d-104">Obtenha dados sobre as atividades do OneDrive por usuário.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-104">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="9cc8d-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="9cc8d-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="9cc8d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9cc8d-106">Permissions</span></span>

<span data-ttu-id="9cc8d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cc8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9cc8d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cc8d-109">Permission type</span></span>                        | <span data-ttu-id="9cc8d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9cc8d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9cc8d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cc8d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9cc8d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9cc8d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9cc8d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cc8d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cc8d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-114">Not supported.</span></span>                           |
| <span data-ttu-id="9cc8d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cc8d-115">Application</span></span>                            | <span data-ttu-id="9cc8d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9cc8d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9cc8d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc8d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="9cc8d-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="9cc8d-118">Function parameters</span></span>

<span data-ttu-id="9cc8d-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="9cc8d-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9cc8d-120">Parameter</span></span> | <span data-ttu-id="9cc8d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cc8d-121">Type</span></span>   | <span data-ttu-id="9cc8d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cc8d-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9cc8d-123">ponto</span><span class="sxs-lookup"><span data-stu-id="9cc8d-123">period</span></span>    | <span data-ttu-id="9cc8d-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9cc8d-124">string</span></span> | <span data-ttu-id="9cc8d-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9cc8d-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9cc8d-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="9cc8d-128">data</span><span class="sxs-lookup"><span data-stu-id="9cc8d-128">date</span></span>      | <span data-ttu-id="9cc8d-129">Data</span><span class="sxs-lookup"><span data-stu-id="9cc8d-129">Date</span></span>   | <span data-ttu-id="9cc8d-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="9cc8d-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="9cc8d-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="9cc8d-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="9cc8d-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="9cc8d-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-135">The default output type is text/csv.</span></span> <span data-ttu-id="9cc8d-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9cc8d-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc8d-137">Request headers</span></span>

| <span data-ttu-id="9cc8d-138">Nome</span><span class="sxs-lookup"><span data-stu-id="9cc8d-138">Name</span></span>          | <span data-ttu-id="9cc8d-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cc8d-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9cc8d-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cc8d-140">Authorization</span></span> | <span data-ttu-id="9cc8d-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9cc8d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cc8d-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="9cc8d-144">CSV</span><span class="sxs-lookup"><span data-stu-id="9cc8d-144">CSV</span></span>

<span data-ttu-id="9cc8d-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9cc8d-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9cc8d-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9cc8d-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9cc8d-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="9cc8d-149">Report Refresh Date</span></span>
- <span data-ttu-id="9cc8d-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="9cc8d-150">User Principal Name</span></span>
- <span data-ttu-id="9cc8d-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="9cc8d-151">Is Deleted</span></span>
- <span data-ttu-id="9cc8d-152">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="9cc8d-152">Deleted Date</span></span>
- <span data-ttu-id="9cc8d-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="9cc8d-153">Last Activity Date</span></span>
- <span data-ttu-id="9cc8d-154">Contagem de arquivos exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="9cc8d-154">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="9cc8d-155">Contagem de arquivos sincronizados</span><span class="sxs-lookup"><span data-stu-id="9cc8d-155">Synced File Count</span></span>
- <span data-ttu-id="9cc8d-156">Contagem de arquivos compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="9cc8d-156">Shared Internally File Count</span></span>
- <span data-ttu-id="9cc8d-157">Contagem de arquivos compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="9cc8d-157">Shared Externally File Count</span></span>
- <span data-ttu-id="9cc8d-158">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="9cc8d-158">Assigned Products</span></span>
- <span data-ttu-id="9cc8d-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="9cc8d-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="9cc8d-160">JSON</span><span class="sxs-lookup"><span data-stu-id="9cc8d-160">JSON</span></span>

<span data-ttu-id="9cc8d-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-161">If successful, this method returns a `200 OK` response code and a **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="9cc8d-162">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="9cc8d-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9cc8d-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="9cc8d-164">CSV</span><span class="sxs-lookup"><span data-stu-id="9cc8d-164">CSV</span></span>

<span data-ttu-id="9cc8d-165">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="9cc8d-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc8d-166">Request</span></span>

<span data-ttu-id="9cc8d-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9cc8d-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc8d-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9cc8d-169">C#</span><span class="sxs-lookup"><span data-stu-id="9cc8d-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveactivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9cc8d-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="9cc8d-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveactivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9cc8d-171">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9cc8d-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveactivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9cc8d-172">Java</span><span class="sxs-lookup"><span data-stu-id="9cc8d-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveactivityuserdetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9cc8d-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cc8d-173">Response</span></span>

<span data-ttu-id="9cc8d-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9cc8d-175">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="9cc8d-176">JSON</span><span class="sxs-lookup"><span data-stu-id="9cc8d-176">JSON</span></span>

<span data-ttu-id="9cc8d-177">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="9cc8d-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc8d-178">Request</span></span>

<span data-ttu-id="9cc8d-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-179">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9cc8d-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc8d-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9cc8d-181">C#</span><span class="sxs-lookup"><span data-stu-id="9cc8d-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveactivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9cc8d-182">Javascript</span><span class="sxs-lookup"><span data-stu-id="9cc8d-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveactivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9cc8d-183">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9cc8d-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveactivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9cc8d-184">Java</span><span class="sxs-lookup"><span data-stu-id="9cc8d-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveactivityuserdetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9cc8d-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cc8d-185">Response</span></span>

<span data-ttu-id="9cc8d-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-186">The following is an example of the response.</span></span>

> <span data-ttu-id="9cc8d-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9cc8d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
