---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: Obtenha dados sobre as atividades do OneDrive por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 4575847ccd0a1a607f74b7b7dad1cc0b7334b14a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869091"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="7b448-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="7b448-103">reportRoot: getOneDriveActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b448-104">Obtenha dados sobre as atividades do OneDrive por usuário.</span><span class="sxs-lookup"><span data-stu-id="7b448-104">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="7b448-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="7b448-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="7b448-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b448-106">Permissions</span></span>

<span data-ttu-id="7b448-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b448-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b448-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b448-109">Permission type</span></span>                        | <span data-ttu-id="7b448-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b448-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7b448-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b448-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b448-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b448-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7b448-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b448-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b448-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b448-114">Not supported.</span></span>                           |
| <span data-ttu-id="7b448-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b448-115">Application</span></span>                            | <span data-ttu-id="7b448-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b448-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="7b448-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="7b448-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="7b448-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="7b448-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="7b448-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b448-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="7b448-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="7b448-120">Function parameters</span></span>

<span data-ttu-id="7b448-121">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7b448-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="7b448-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7b448-122">Parameter</span></span> | <span data-ttu-id="7b448-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b448-123">Type</span></span>   | <span data-ttu-id="7b448-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b448-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7b448-125">ponto</span><span class="sxs-lookup"><span data-stu-id="7b448-125">period</span></span>    | <span data-ttu-id="7b448-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7b448-126">string</span></span> | <span data-ttu-id="7b448-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7b448-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7b448-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="7b448-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7b448-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7b448-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7b448-130">data</span><span class="sxs-lookup"><span data-stu-id="7b448-130">date</span></span>      | <span data-ttu-id="7b448-131">Data</span><span class="sxs-lookup"><span data-stu-id="7b448-131">Date</span></span>   | <span data-ttu-id="7b448-132">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="7b448-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7b448-133">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="7b448-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7b448-134">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="7b448-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7b448-135">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="7b448-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="7b448-136">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="7b448-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7b448-137">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="7b448-137">The default output type is text/csv.</span></span> <span data-ttu-id="7b448-138">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="7b448-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b448-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b448-139">Request headers</span></span>

| <span data-ttu-id="7b448-140">Nome</span><span class="sxs-lookup"><span data-stu-id="7b448-140">Name</span></span>          | <span data-ttu-id="7b448-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b448-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7b448-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b448-142">Authorization</span></span> | <span data-ttu-id="7b448-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b448-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7b448-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b448-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7b448-146">CSV</span><span class="sxs-lookup"><span data-stu-id="7b448-146">CSV</span></span>

<span data-ttu-id="7b448-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="7b448-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7b448-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="7b448-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7b448-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7b448-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7b448-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="7b448-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7b448-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="7b448-151">Report Refresh Date</span></span>
- <span data-ttu-id="7b448-152">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="7b448-152">User Principal Name</span></span>
- <span data-ttu-id="7b448-153">Excluído</span><span class="sxs-lookup"><span data-stu-id="7b448-153">Is Deleted</span></span>
- <span data-ttu-id="7b448-154">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="7b448-154">Deleted Date</span></span>
- <span data-ttu-id="7b448-155">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="7b448-155">Last Activity Date</span></span>
- <span data-ttu-id="7b448-156">Contagem de arquivos exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="7b448-156">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="7b448-157">Contagem de arquivos sincronizados</span><span class="sxs-lookup"><span data-stu-id="7b448-157">Synced File Count</span></span>
- <span data-ttu-id="7b448-158">Contagem de arquivos compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="7b448-158">Shared Internally File Count</span></span>
- <span data-ttu-id="7b448-159">Contagem de arquivos compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="7b448-159">Shared Externally File Count</span></span>
- <span data-ttu-id="7b448-160">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="7b448-160">Assigned Products</span></span>
- <span data-ttu-id="7b448-161">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="7b448-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7b448-162">JSON</span><span class="sxs-lookup"><span data-stu-id="7b448-162">JSON</span></span>

<span data-ttu-id="7b448-163">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b448-163">If successful, this method returns a `200 OK` response code and a **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="7b448-164">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="7b448-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="7b448-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b448-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7b448-166">CSV</span><span class="sxs-lookup"><span data-stu-id="7b448-166">CSV</span></span>

<span data-ttu-id="7b448-167">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="7b448-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7b448-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b448-168">Request</span></span>

<span data-ttu-id="7b448-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b448-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7b448-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b448-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7b448-171">C#</span><span class="sxs-lookup"><span data-stu-id="7b448-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveactivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7b448-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b448-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveactivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7b448-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b448-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveactivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7b448-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b448-174">Response</span></span>

<span data-ttu-id="7b448-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7b448-175">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7b448-176">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="7b448-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="7b448-177">JSON</span><span class="sxs-lookup"><span data-stu-id="7b448-177">JSON</span></span>

<span data-ttu-id="7b448-178">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="7b448-178">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7b448-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b448-179">Request</span></span>

<span data-ttu-id="7b448-180">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b448-180">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7b448-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b448-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7b448-182">C#</span><span class="sxs-lookup"><span data-stu-id="7b448-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveactivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7b448-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b448-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveactivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7b448-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b448-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveactivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7b448-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b448-185">Response</span></span>

<span data-ttu-id="7b448-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7b448-186">The following is an example of the response.</span></span>

> <span data-ttu-id="7b448-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7b448-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
