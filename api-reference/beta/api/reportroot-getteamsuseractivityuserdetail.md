---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: Obter detalhes sobre a atividade de usuário do Microsoft Teams por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a8ea4a5a8293df09abbb2eeafceb3b932730cfdc
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722703"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="bddd8-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="bddd8-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bddd8-104">Obtém detalhes sobre a atividade de usuários do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="bddd8-104">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="bddd8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bddd8-105">Permissions</span></span>

<span data-ttu-id="bddd8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bddd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bddd8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bddd8-108">Permission type</span></span>                        | <span data-ttu-id="bddd8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bddd8-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bddd8-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bddd8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bddd8-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bddd8-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bddd8-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bddd8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bddd8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bddd8-113">Not supported.</span></span>                           |
| <span data-ttu-id="bddd8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bddd8-114">Application</span></span>                            | <span data-ttu-id="bddd8-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bddd8-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bddd8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bddd8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='D7')
GET /reports/getTeamsUserActivityUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="bddd8-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="bddd8-117">Function parameters</span></span>

<span data-ttu-id="bddd8-118">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="bddd8-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="bddd8-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bddd8-119">Parameter</span></span> | <span data-ttu-id="bddd8-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="bddd8-120">Type</span></span>   | <span data-ttu-id="bddd8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bddd8-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bddd8-122">ponto</span><span class="sxs-lookup"><span data-stu-id="bddd8-122">period</span></span>    | <span data-ttu-id="bddd8-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bddd8-123">string</span></span> | <span data-ttu-id="bddd8-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bddd8-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bddd8-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="bddd8-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bddd8-126">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bddd8-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="bddd8-127">data</span><span class="sxs-lookup"><span data-stu-id="bddd8-127">date</span></span>      | <span data-ttu-id="bddd8-128">Data</span><span class="sxs-lookup"><span data-stu-id="bddd8-128">Date</span></span>   | <span data-ttu-id="bddd8-129">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="bddd8-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="bddd8-130">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="bddd8-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="bddd8-131">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="bddd8-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="bddd8-132">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="bddd8-132">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="bddd8-133">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="bddd8-133">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="bddd8-134">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="bddd8-134">The default output type is text/csv.</span></span> <span data-ttu-id="bddd8-135">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="bddd8-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bddd8-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bddd8-136">Request headers</span></span>

| <span data-ttu-id="bddd8-137">Nome</span><span class="sxs-lookup"><span data-stu-id="bddd8-137">Name</span></span>          | <span data-ttu-id="bddd8-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="bddd8-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="bddd8-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="bddd8-139">Authorization</span></span> | <span data-ttu-id="bddd8-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bddd8-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bddd8-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="bddd8-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="bddd8-143">CSV</span><span class="sxs-lookup"><span data-stu-id="bddd8-143">CSV</span></span>

<span data-ttu-id="bddd8-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="bddd8-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bddd8-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="bddd8-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bddd8-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="bddd8-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bddd8-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="bddd8-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bddd8-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="bddd8-148">Report Refresh Date</span></span>
- <span data-ttu-id="bddd8-149">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="bddd8-149">User Principal Name</span></span>
- <span data-ttu-id="bddd8-150">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="bddd8-150">Last Activity Date</span></span>
- <span data-ttu-id="bddd8-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="bddd8-151">Is Deleted</span></span>
- <span data-ttu-id="bddd8-152">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="bddd8-152">Deleted Date</span></span>
- <span data-ttu-id="bddd8-153">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="bddd8-153">Assigned Products</span></span>
- <span data-ttu-id="bddd8-154">Número de mensagens de chat de equipe</span><span class="sxs-lookup"><span data-stu-id="bddd8-154">Team Chat Message Count</span></span>
- <span data-ttu-id="bddd8-155">Contagem de mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="bddd8-155">Private Chat Message Count</span></span>
- <span data-ttu-id="bddd8-156">Contagem de chamadas</span><span class="sxs-lookup"><span data-stu-id="bddd8-156">Call Count</span></span>
- <span data-ttu-id="bddd8-157">Contagem de reuniões</span><span class="sxs-lookup"><span data-stu-id="bddd8-157">Meeting Count</span></span>
- <span data-ttu-id="bddd8-158">Tem outra ação</span><span class="sxs-lookup"><span data-stu-id="bddd8-158">Has Other Action</span></span>
- <span data-ttu-id="bddd8-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="bddd8-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="bddd8-160">JSON</span><span class="sxs-lookup"><span data-stu-id="bddd8-160">JSON</span></span>

<span data-ttu-id="bddd8-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bddd8-161">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="bddd8-162">O tamanho de página padrão para essa solicitação é de 2000 itens.</span><span class="sxs-lookup"><span data-stu-id="bddd8-162">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="bddd8-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bddd8-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="bddd8-164">CSV</span><span class="sxs-lookup"><span data-stu-id="bddd8-164">CSV</span></span>

<span data-ttu-id="bddd8-165">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="bddd8-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="bddd8-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bddd8-166">Request</span></span>

<span data-ttu-id="bddd8-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bddd8-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bddd8-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="bddd8-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bddd8-169">C#</span><span class="sxs-lookup"><span data-stu-id="bddd8-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bddd8-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bddd8-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bddd8-171">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bddd8-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bddd8-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="bddd8-172">Response</span></span>

<span data-ttu-id="bddd8-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bddd8-173">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="bddd8-174">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="bddd8-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
```

### <a name="json"></a><span data-ttu-id="bddd8-175">JSON</span><span class="sxs-lookup"><span data-stu-id="bddd8-175">JSON</span></span>

<span data-ttu-id="bddd8-176">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="bddd8-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="bddd8-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bddd8-177">Request</span></span>

<span data-ttu-id="bddd8-178">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bddd8-178">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bddd8-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="bddd8-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bddd8-180">C#</span><span class="sxs-lookup"><span data-stu-id="bddd8-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bddd8-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bddd8-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bddd8-182">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bddd8-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bddd8-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="bddd8-183">Response</span></span>

<span data-ttu-id="bddd8-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bddd8-184">The following is an example of the response.</span></span>

> <span data-ttu-id="bddd8-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bddd8-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 452

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "teamChatMessageCount": 0, 
      "privateChatMessageCount": 49, 
      "callCount": 2, 
      "meetingCount": 0, 
      "hasOtherAction": true, 
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
