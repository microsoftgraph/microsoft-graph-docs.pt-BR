---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Obtenha dados sobre as atividades de grupo do Yammer por grupo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0f24445dc38edbdab501ca0212fd1ee1c4575e0f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453951"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="67443-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="67443-103">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="67443-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="67443-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67443-105">Obtenha dados sobre as atividades de grupo do Yammer por grupo.</span><span class="sxs-lookup"><span data-stu-id="67443-105">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="67443-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade de grupos do Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="67443-106">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="67443-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="67443-107">Permissions</span></span>

<span data-ttu-id="67443-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67443-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="67443-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67443-110">Permission type</span></span>                        | <span data-ttu-id="67443-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67443-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="67443-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67443-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="67443-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="67443-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="67443-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67443-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67443-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67443-115">Not supported.</span></span>                           |
| <span data-ttu-id="67443-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67443-116">Application</span></span>                            | <span data-ttu-id="67443-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="67443-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="67443-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="67443-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="67443-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="67443-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="67443-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67443-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="67443-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="67443-121">Function parameters</span></span>

<span data-ttu-id="67443-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="67443-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="67443-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="67443-123">Parameter</span></span> | <span data-ttu-id="67443-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="67443-124">Type</span></span>   | <span data-ttu-id="67443-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="67443-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="67443-126">ponto</span><span class="sxs-lookup"><span data-stu-id="67443-126">period</span></span>    | <span data-ttu-id="67443-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67443-127">string</span></span> | <span data-ttu-id="67443-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="67443-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="67443-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="67443-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="67443-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="67443-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="67443-131">data</span><span class="sxs-lookup"><span data-stu-id="67443-131">date</span></span>      | <span data-ttu-id="67443-132">Data</span><span class="sxs-lookup"><span data-stu-id="67443-132">Date</span></span>   | <span data-ttu-id="67443-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="67443-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="67443-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="67443-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="67443-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="67443-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="67443-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="67443-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="67443-137">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="67443-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="67443-138">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="67443-138">The default output type is text/csv.</span></span> <span data-ttu-id="67443-139">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="67443-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67443-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67443-140">Request headers</span></span>

| <span data-ttu-id="67443-141">Nome</span><span class="sxs-lookup"><span data-stu-id="67443-141">Name</span></span>          | <span data-ttu-id="67443-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="67443-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="67443-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="67443-143">Authorization</span></span> | <span data-ttu-id="67443-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67443-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="67443-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="67443-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="67443-147">CSV</span><span class="sxs-lookup"><span data-stu-id="67443-147">CSV</span></span>

<span data-ttu-id="67443-148">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="67443-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="67443-149">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="67443-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="67443-150">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="67443-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="67443-151">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="67443-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="67443-152">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="67443-152">Report Refresh Date</span></span>
- <span data-ttu-id="67443-153">Nome de exibição do grupo</span><span class="sxs-lookup"><span data-stu-id="67443-153">Group Display Name</span></span>
- <span data-ttu-id="67443-154">Excluído</span><span class="sxs-lookup"><span data-stu-id="67443-154">Is Deleted</span></span>
- <span data-ttu-id="67443-155">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="67443-155">Owner Principal Name</span></span>
- <span data-ttu-id="67443-156">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="67443-156">Last Activity Date</span></span>
- <span data-ttu-id="67443-157">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="67443-157">Group Type</span></span>
- <span data-ttu-id="67443-158">Office 365 Connected</span><span class="sxs-lookup"><span data-stu-id="67443-158">Office 365 Connected</span></span>
- <span data-ttu-id="67443-159">Contagem de Membros</span><span class="sxs-lookup"><span data-stu-id="67443-159">Member Count</span></span>
- <span data-ttu-id="67443-160">Contagem de Postagens</span><span class="sxs-lookup"><span data-stu-id="67443-160">Posted Count</span></span>
- <span data-ttu-id="67443-161">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="67443-161">Read Count</span></span>
- <span data-ttu-id="67443-162">Contagem de Curtidas</span><span class="sxs-lookup"><span data-stu-id="67443-162">Liked Count</span></span>
- <span data-ttu-id="67443-163">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="67443-163">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="67443-164">JSON</span><span class="sxs-lookup"><span data-stu-id="67443-164">JSON</span></span>

<span data-ttu-id="67443-165">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67443-165">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="67443-166">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="67443-166">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="67443-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67443-167">Example</span></span>

### <a name="csv"></a><span data-ttu-id="67443-168">CSV</span><span class="sxs-lookup"><span data-stu-id="67443-168">CSV</span></span>

<span data-ttu-id="67443-169">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="67443-169">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="67443-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67443-170">Request</span></span>

<span data-ttu-id="67443-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="67443-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="67443-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="67443-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="67443-173">C#</span><span class="sxs-lookup"><span data-stu-id="67443-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitydetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67443-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67443-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitydetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67443-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67443-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitydetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="67443-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="67443-176">Response</span></span>

<span data-ttu-id="67443-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="67443-177">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="67443-178">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="67443-178">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```

### <a name="json"></a><span data-ttu-id="67443-179">JSON</span><span class="sxs-lookup"><span data-stu-id="67443-179">JSON</span></span>

<span data-ttu-id="67443-180">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="67443-180">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="67443-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67443-181">Request</span></span>

<span data-ttu-id="67443-182">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="67443-182">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="67443-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="67443-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="67443-184">C#</span><span class="sxs-lookup"><span data-stu-id="67443-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitydetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67443-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67443-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitydetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67443-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67443-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitydetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="67443-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="67443-187">Response</span></span>

<span data-ttu-id="67443-188">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="67443-188">The following is an example of the response.</span></span>

> <span data-ttu-id="67443-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67443-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "lastActivityDate": "2017-08-30", 
      "groupType": "private", 
      "office365Connected": true, 
      "memberCount": 176, 
      "postedCount": 15, 
      "readCount": 24, 
      "likedCount": 3, 
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
