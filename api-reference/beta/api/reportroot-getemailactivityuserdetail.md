---
title: 'reportRoot: getEmailActivityUserDetail'
description: Obtenha dados sobre as atividades de email que os usuários realizaram.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 33bb217732da48c598e5e5d7b774f0f80726ab97
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869259"
---
# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="db551-103">reportRoot: getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="db551-103">reportRoot: getEmailActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db551-104">Obtenha dados sobre as atividades de email que os usuários realizaram.</span><span class="sxs-lookup"><span data-stu-id="db551-104">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="db551-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="db551-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="db551-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="db551-106">Permissions</span></span>

<span data-ttu-id="db551-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db551-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db551-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db551-109">Permission type</span></span>                        | <span data-ttu-id="db551-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db551-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="db551-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db551-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="db551-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="db551-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="db551-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db551-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db551-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db551-114">Not supported.</span></span>                           |
| <span data-ttu-id="db551-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db551-115">Application</span></span>                            | <span data-ttu-id="db551-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="db551-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="db551-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="db551-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="db551-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="db551-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="db551-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db551-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="db551-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="db551-120">Function parameters</span></span>

<span data-ttu-id="db551-121">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="db551-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="db551-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="db551-122">Parameter</span></span> | <span data-ttu-id="db551-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="db551-123">Type</span></span>   | <span data-ttu-id="db551-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="db551-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="db551-125">ponto</span><span class="sxs-lookup"><span data-stu-id="db551-125">period</span></span>    | <span data-ttu-id="db551-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db551-126">string</span></span> | <span data-ttu-id="db551-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="db551-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="db551-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="db551-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="db551-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="db551-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="db551-130">data</span><span class="sxs-lookup"><span data-stu-id="db551-130">date</span></span>      | <span data-ttu-id="db551-131">Data</span><span class="sxs-lookup"><span data-stu-id="db551-131">Date</span></span>   | <span data-ttu-id="db551-132">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="db551-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="db551-133">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="db551-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="db551-134">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="db551-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="db551-135">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="db551-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="db551-136">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="db551-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="db551-137">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="db551-137">The default output type is text/csv.</span></span> <span data-ttu-id="db551-138">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="db551-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="db551-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db551-139">Request headers</span></span>

| <span data-ttu-id="db551-140">Nome</span><span class="sxs-lookup"><span data-stu-id="db551-140">Name</span></span>          | <span data-ttu-id="db551-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="db551-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="db551-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="db551-142">Authorization</span></span> | <span data-ttu-id="db551-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db551-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="db551-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="db551-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="db551-146">CSV</span><span class="sxs-lookup"><span data-stu-id="db551-146">CSV</span></span>

<span data-ttu-id="db551-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="db551-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="db551-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="db551-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="db551-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="db551-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="db551-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="db551-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="db551-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="db551-151">Report Refresh Date</span></span>
- <span data-ttu-id="db551-152">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="db551-152">User Principal Name</span></span>
- <span data-ttu-id="db551-153">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="db551-153">Display Name</span></span>
- <span data-ttu-id="db551-154">Excluído</span><span class="sxs-lookup"><span data-stu-id="db551-154">Is Deleted</span></span>
- <span data-ttu-id="db551-155">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="db551-155">Deleted Date</span></span>
- <span data-ttu-id="db551-156">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="db551-156">Last Activity Date</span></span>
- <span data-ttu-id="db551-157">Contagem de Envios</span><span class="sxs-lookup"><span data-stu-id="db551-157">Send Count</span></span>
- <span data-ttu-id="db551-158">Contagem de Recebimentos</span><span class="sxs-lookup"><span data-stu-id="db551-158">Receive Count</span></span>
- <span data-ttu-id="db551-159">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="db551-159">Read Count</span></span>
- <span data-ttu-id="db551-160">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="db551-160">Assigned Products</span></span>
- <span data-ttu-id="db551-161">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="db551-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="db551-162">JSON</span><span class="sxs-lookup"><span data-stu-id="db551-162">JSON</span></span>

<span data-ttu-id="db551-163">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[emailActivityUserDetail](../resources/emailactivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db551-163">If successful, this method returns a `200 OK` response code and an **[emailActivityUserDetail](../resources/emailactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="db551-164">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="db551-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="db551-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db551-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="db551-166">CSV</span><span class="sxs-lookup"><span data-stu-id="db551-166">CSV</span></span>

<span data-ttu-id="db551-167">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="db551-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="db551-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db551-168">Request</span></span>

<span data-ttu-id="db551-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="db551-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="db551-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="db551-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db551-171">C#</span><span class="sxs-lookup"><span data-stu-id="db551-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db551-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db551-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db551-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db551-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="db551-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="db551-174">Response</span></span>

<span data-ttu-id="db551-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db551-175">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="db551-176">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="db551-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Send Count,Receive Count,Read Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="db551-177">JSON</span><span class="sxs-lookup"><span data-stu-id="db551-177">JSON</span></span>

<span data-ttu-id="db551-178">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="db551-178">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="db551-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db551-179">Request</span></span>

<span data-ttu-id="db551-180">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="db551-180">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="db551-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="db551-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db551-182">C#</span><span class="sxs-lookup"><span data-stu-id="db551-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db551-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db551-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db551-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db551-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="db551-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="db551-185">Response</span></span>

<span data-ttu-id="db551-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="db551-186">The following is an example of the response.</span></span>

> <span data-ttu-id="db551-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db551-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 424

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "sendCount": 86, 
      "receiveCount": 3198, 
      "readCount": 388, 
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
