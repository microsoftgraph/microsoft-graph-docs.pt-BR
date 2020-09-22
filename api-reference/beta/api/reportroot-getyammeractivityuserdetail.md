---
title: 'reportRoot: getYammerActivityUserDetail'
description: Obtenha dados sobre as atividades do Yammer por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 965c83f953ad60920b6cee39d284c0633a1a38c6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052971"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="01465-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="01465-103">reportRoot: getYammerActivityUserDetail</span></span>

<span data-ttu-id="01465-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01465-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01465-105">Obtenha dados sobre as atividades do Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="01465-105">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="01465-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="01465-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="01465-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="01465-107">Permissions</span></span>

<span data-ttu-id="01465-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01465-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01465-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01465-110">Permission type</span></span>                        | <span data-ttu-id="01465-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01465-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="01465-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01465-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="01465-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="01465-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="01465-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01465-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01465-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01465-115">Not supported.</span></span>                           |
| <span data-ttu-id="01465-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01465-116">Application</span></span>                            | <span data-ttu-id="01465-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="01465-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="01465-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="01465-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="01465-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="01465-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="01465-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01465-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="01465-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="01465-121">Function parameters</span></span>

<span data-ttu-id="01465-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="01465-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="01465-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="01465-123">Parameter</span></span> | <span data-ttu-id="01465-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="01465-124">Type</span></span>   | <span data-ttu-id="01465-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="01465-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="01465-126">ponto</span><span class="sxs-lookup"><span data-stu-id="01465-126">period</span></span>    | <span data-ttu-id="01465-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01465-127">string</span></span> | <span data-ttu-id="01465-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="01465-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="01465-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="01465-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="01465-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="01465-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="01465-131">data</span><span class="sxs-lookup"><span data-stu-id="01465-131">date</span></span>      | <span data-ttu-id="01465-132">Data</span><span class="sxs-lookup"><span data-stu-id="01465-132">Date</span></span>   | <span data-ttu-id="01465-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="01465-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="01465-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="01465-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="01465-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="01465-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="01465-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="01465-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="01465-137">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="01465-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="01465-138">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="01465-138">The default output type is text/csv.</span></span> <span data-ttu-id="01465-139">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="01465-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01465-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01465-140">Request headers</span></span>

| <span data-ttu-id="01465-141">Nome</span><span class="sxs-lookup"><span data-stu-id="01465-141">Name</span></span>          | <span data-ttu-id="01465-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="01465-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="01465-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="01465-143">Authorization</span></span> | <span data-ttu-id="01465-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01465-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="01465-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="01465-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="01465-147">CSV</span><span class="sxs-lookup"><span data-stu-id="01465-147">CSV</span></span>

<span data-ttu-id="01465-148">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="01465-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="01465-149">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="01465-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="01465-150">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="01465-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="01465-151">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="01465-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="01465-152">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="01465-152">Report Refresh Date</span></span>
- <span data-ttu-id="01465-153">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="01465-153">User Principal Name</span></span>
- <span data-ttu-id="01465-154">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="01465-154">Display Name</span></span>
- <span data-ttu-id="01465-155">Estado do usuário</span><span class="sxs-lookup"><span data-stu-id="01465-155">User State</span></span>
- <span data-ttu-id="01465-156">Data de alteração de estado</span><span class="sxs-lookup"><span data-stu-id="01465-156">State Change Date</span></span>
- <span data-ttu-id="01465-157">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="01465-157">Last Activity Date</span></span>
- <span data-ttu-id="01465-158">Contagem de Postagens</span><span class="sxs-lookup"><span data-stu-id="01465-158">Posted Count</span></span>
- <span data-ttu-id="01465-159">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="01465-159">Read Count</span></span>
- <span data-ttu-id="01465-160">Contagem de Curtidas</span><span class="sxs-lookup"><span data-stu-id="01465-160">Liked Count</span></span>
- <span data-ttu-id="01465-161">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="01465-161">Assigned Products</span></span>
- <span data-ttu-id="01465-162">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="01465-162">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="01465-163">JSON</span><span class="sxs-lookup"><span data-stu-id="01465-163">JSON</span></span>

<span data-ttu-id="01465-164">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01465-164">If successful, this method returns a `200 OK` response code and a **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="01465-165">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="01465-165">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="01465-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01465-166">Example</span></span>

### <a name="csv"></a><span data-ttu-id="01465-167">CSV</span><span class="sxs-lookup"><span data-stu-id="01465-167">CSV</span></span>

<span data-ttu-id="01465-168">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="01465-168">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="01465-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01465-169">Request</span></span>

<span data-ttu-id="01465-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01465-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammeractivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="01465-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="01465-171">Response</span></span>

<span data-ttu-id="01465-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01465-172">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="01465-173">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="01465-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Posted Count,Read Count,Liked Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="01465-174">JSON</span><span class="sxs-lookup"><span data-stu-id="01465-174">JSON</span></span>

<span data-ttu-id="01465-175">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="01465-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="01465-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01465-176">Request</span></span>

<span data-ttu-id="01465-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01465-177">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammeractivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="01465-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="01465-178">Response</span></span>

<span data-ttu-id="01465-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01465-179">The following is an example of the response.</span></span>

> <span data-ttu-id="01465-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01465-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 434

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "userState": "active", 
      "stateChangeDate": "2015-08-26", 
      "lastActivityDate": "2017-09-01", 
      "postedCount": 2, 
      "readCount": 5, 
      "likedCount": 0, 
      "assignedProducts": [
        "Microsoft 365 ENTERPRISE E5"
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


