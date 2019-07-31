---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: Obter detalhes sobre a atividade de usuário do Microsoft Teams por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 15456b0f341ef16742764c0191a66fdf9c3c9bf1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983121"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="8f7b7-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="8f7b7-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f7b7-104">Obtém detalhes sobre a atividade de usuários do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-104">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f7b7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f7b7-105">Permissions</span></span>

<span data-ttu-id="8f7b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f7b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f7b7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f7b7-108">Permission type</span></span>                        | <span data-ttu-id="8f7b7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f7b7-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8f7b7-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f7b7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f7b7-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f7b7-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8f7b7-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f7b7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f7b7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-113">Not supported.</span></span>                           |
| <span data-ttu-id="8f7b7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f7b7-114">Application</span></span>                            | <span data-ttu-id="8f7b7-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f7b7-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8f7b7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f7b7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='D7')
GET /reports/getTeamsUserActivityUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="8f7b7-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="8f7b7-117">Function parameters</span></span>

<span data-ttu-id="8f7b7-118">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="8f7b7-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8f7b7-119">Parameter</span></span> | <span data-ttu-id="8f7b7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f7b7-120">Type</span></span>   | <span data-ttu-id="8f7b7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f7b7-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8f7b7-122">ponto</span><span class="sxs-lookup"><span data-stu-id="8f7b7-122">period</span></span>    | <span data-ttu-id="8f7b7-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f7b7-123">string</span></span> | <span data-ttu-id="8f7b7-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8f7b7-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8f7b7-126">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="8f7b7-127">data</span><span class="sxs-lookup"><span data-stu-id="8f7b7-127">date</span></span>      | <span data-ttu-id="8f7b7-128">Data</span><span class="sxs-lookup"><span data-stu-id="8f7b7-128">Date</span></span>   | <span data-ttu-id="8f7b7-129">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="8f7b7-130">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="8f7b7-131">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="8f7b7-132">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-132">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="8f7b7-133">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-133">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8f7b7-134">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-134">The default output type is text/csv.</span></span> <span data-ttu-id="8f7b7-135">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f7b7-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f7b7-136">Request headers</span></span>

| <span data-ttu-id="8f7b7-137">Nome</span><span class="sxs-lookup"><span data-stu-id="8f7b7-137">Name</span></span>          | <span data-ttu-id="8f7b7-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f7b7-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8f7b7-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f7b7-139">Authorization</span></span> | <span data-ttu-id="8f7b7-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8f7b7-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f7b7-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8f7b7-143">CSV</span><span class="sxs-lookup"><span data-stu-id="8f7b7-143">CSV</span></span>

<span data-ttu-id="8f7b7-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8f7b7-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8f7b7-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8f7b7-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8f7b7-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="8f7b7-148">Report Refresh Date</span></span>
- <span data-ttu-id="8f7b7-149">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="8f7b7-149">User Principal Name</span></span>
- <span data-ttu-id="8f7b7-150">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="8f7b7-150">Last Activity Date</span></span>
- <span data-ttu-id="8f7b7-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="8f7b7-151">Is Deleted</span></span>
- <span data-ttu-id="8f7b7-152">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="8f7b7-152">Deleted Date</span></span>
- <span data-ttu-id="8f7b7-153">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="8f7b7-153">Assigned Products</span></span>
- <span data-ttu-id="8f7b7-154">Número de mensagens de chat de equipe</span><span class="sxs-lookup"><span data-stu-id="8f7b7-154">Team Chat Message Count</span></span>
- <span data-ttu-id="8f7b7-155">Contagem de mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="8f7b7-155">Private Chat Message Count</span></span>
- <span data-ttu-id="8f7b7-156">Contagem de chamadas</span><span class="sxs-lookup"><span data-stu-id="8f7b7-156">Call Count</span></span>
- <span data-ttu-id="8f7b7-157">Contagem de reuniões</span><span class="sxs-lookup"><span data-stu-id="8f7b7-157">Meeting Count</span></span>
- <span data-ttu-id="8f7b7-158">Tem outra ação</span><span class="sxs-lookup"><span data-stu-id="8f7b7-158">Has Other Action</span></span>
- <span data-ttu-id="8f7b7-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="8f7b7-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="8f7b7-160">JSON</span><span class="sxs-lookup"><span data-stu-id="8f7b7-160">JSON</span></span>

<span data-ttu-id="8f7b7-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-161">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="8f7b7-162">O tamanho de página padrão para essa solicitação é de 2000 itens.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-162">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="8f7b7-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f7b7-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8f7b7-164">CSV</span><span class="sxs-lookup"><span data-stu-id="8f7b7-164">CSV</span></span>

<span data-ttu-id="8f7b7-165">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8f7b7-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f7b7-166">Request</span></span>

<span data-ttu-id="8f7b7-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8f7b7-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f7b7-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f7b7-169">C#</span><span class="sxs-lookup"><span data-stu-id="8f7b7-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f7b7-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="8f7b7-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f7b7-171">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8f7b7-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8f7b7-172">Java</span><span class="sxs-lookup"><span data-stu-id="8f7b7-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivityuserdetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8f7b7-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f7b7-173">Response</span></span>

<span data-ttu-id="8f7b7-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8f7b7-175">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="8f7b7-176">JSON</span><span class="sxs-lookup"><span data-stu-id="8f7b7-176">JSON</span></span>

<span data-ttu-id="8f7b7-177">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8f7b7-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f7b7-178">Request</span></span>

<span data-ttu-id="8f7b7-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-179">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8f7b7-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f7b7-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f7b7-181">C#</span><span class="sxs-lookup"><span data-stu-id="8f7b7-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f7b7-182">Javascript</span><span class="sxs-lookup"><span data-stu-id="8f7b7-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f7b7-183">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8f7b7-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8f7b7-184">Java</span><span class="sxs-lookup"><span data-stu-id="8f7b7-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivityuserdetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8f7b7-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f7b7-185">Response</span></span>

<span data-ttu-id="8f7b7-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-186">The following is an example of the response.</span></span>

> <span data-ttu-id="8f7b7-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f7b7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
