---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Obtenha dados sobre as atividades de grupo do Yammer por grupo.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 15744a267736d0413d01a760cad459fd7c4aae46
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054942"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="9c3d9-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="9c3d9-103">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="9c3d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c3d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c3d9-105">Obtenha dados sobre as atividades de grupo do Yammer por grupo.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-105">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="9c3d9-106">**Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - atividade Yammer grupos](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="9c3d9-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="9c3d9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c3d9-107">Permissions</span></span>

<span data-ttu-id="9c3d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c3d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9c3d9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c3d9-110">Permission type</span></span>                        | <span data-ttu-id="9c3d9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c3d9-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9c3d9-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c3d9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9c3d9-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c3d9-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9c3d9-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c3d9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c3d9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-115">Not supported.</span></span>                           |
| <span data-ttu-id="9c3d9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c3d9-116">Application</span></span>                            | <span data-ttu-id="9c3d9-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c3d9-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="9c3d9-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="9c3d9-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="9c3d9-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="9c3d9-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c3d9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="9c3d9-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="9c3d9-121">Function parameters</span></span>

<span data-ttu-id="9c3d9-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="9c3d9-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9c3d9-123">Parameter</span></span> | <span data-ttu-id="9c3d9-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c3d9-124">Type</span></span>   | <span data-ttu-id="9c3d9-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c3d9-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9c3d9-126">ponto</span><span class="sxs-lookup"><span data-stu-id="9c3d9-126">period</span></span>    | <span data-ttu-id="9c3d9-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c3d9-127">string</span></span> | <span data-ttu-id="9c3d9-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9c3d9-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9c3d9-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="9c3d9-131">data</span><span class="sxs-lookup"><span data-stu-id="9c3d9-131">date</span></span>      | <span data-ttu-id="9c3d9-132">Data</span><span class="sxs-lookup"><span data-stu-id="9c3d9-132">Date</span></span>   | <span data-ttu-id="9c3d9-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="9c3d9-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="9c3d9-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="9c3d9-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="9c3d9-137">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="9c3d9-138">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-138">The default output type is text/csv.</span></span> <span data-ttu-id="9c3d9-139">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c3d9-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c3d9-140">Request headers</span></span>

| <span data-ttu-id="9c3d9-141">Nome</span><span class="sxs-lookup"><span data-stu-id="9c3d9-141">Name</span></span>          | <span data-ttu-id="9c3d9-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c3d9-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9c3d9-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c3d9-143">Authorization</span></span> | <span data-ttu-id="9c3d9-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9c3d9-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c3d9-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="9c3d9-147">CSV</span><span class="sxs-lookup"><span data-stu-id="9c3d9-147">CSV</span></span>

<span data-ttu-id="9c3d9-148">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9c3d9-149">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9c3d9-150">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9c3d9-151">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9c3d9-152">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="9c3d9-152">Report Refresh Date</span></span>
- <span data-ttu-id="9c3d9-153">Nome de exibição do grupo</span><span class="sxs-lookup"><span data-stu-id="9c3d9-153">Group Display Name</span></span>
- <span data-ttu-id="9c3d9-154">Excluído</span><span class="sxs-lookup"><span data-stu-id="9c3d9-154">Is Deleted</span></span>
- <span data-ttu-id="9c3d9-155">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="9c3d9-155">Owner Principal Name</span></span>
- <span data-ttu-id="9c3d9-156">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="9c3d9-156">Last Activity Date</span></span>
- <span data-ttu-id="9c3d9-157">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="9c3d9-157">Group Type</span></span>
- <span data-ttu-id="9c3d9-158">Office 365 Connected</span><span class="sxs-lookup"><span data-stu-id="9c3d9-158">Office 365 Connected</span></span>
- <span data-ttu-id="9c3d9-159">Contagem de Membros</span><span class="sxs-lookup"><span data-stu-id="9c3d9-159">Member Count</span></span>
- <span data-ttu-id="9c3d9-160">Contagem de Postagens</span><span class="sxs-lookup"><span data-stu-id="9c3d9-160">Posted Count</span></span>
- <span data-ttu-id="9c3d9-161">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="9c3d9-161">Read Count</span></span>
- <span data-ttu-id="9c3d9-162">Contagem de Curtidas</span><span class="sxs-lookup"><span data-stu-id="9c3d9-162">Liked Count</span></span>
- <span data-ttu-id="9c3d9-163">Nome de exibição de rede</span><span class="sxs-lookup"><span data-stu-id="9c3d9-163">Network Display Name</span></span>
- <span data-ttu-id="9c3d9-164">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="9c3d9-164">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="9c3d9-165">JSON</span><span class="sxs-lookup"><span data-stu-id="9c3d9-165">JSON</span></span>

<span data-ttu-id="9c3d9-166">Se tiver êxito, este método retornará um código de resposta e um `200 OK` **[objeto yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-166">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="9c3d9-167">O tamanho padrão da página para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-167">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="9c3d9-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c3d9-168">Example</span></span>

### <a name="csv"></a><span data-ttu-id="9c3d9-169">CSV</span><span class="sxs-lookup"><span data-stu-id="9c3d9-169">CSV</span></span>

<span data-ttu-id="9c3d9-170">A seguir, um exemplo que dá saída ao CSV.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-170">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="9c3d9-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c3d9-171">Request</span></span>

<span data-ttu-id="9c3d9-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-172">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="9c3d9-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c3d9-173">Response</span></span>

<span data-ttu-id="9c3d9-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9c3d9-175">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Network Display Name,Report Period
```

### <a name="json"></a><span data-ttu-id="9c3d9-176">JSON</span><span class="sxs-lookup"><span data-stu-id="9c3d9-176">JSON</span></span>

<span data-ttu-id="9c3d9-177">A seguir, um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="9c3d9-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c3d9-178">Request</span></span>

<span data-ttu-id="9c3d9-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-179">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="9c3d9-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c3d9-180">Response</span></span>

<span data-ttu-id="9c3d9-181">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-181">The following is an example of the response.</span></span>

> <span data-ttu-id="9c3d9-182">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9c3d9-182">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "networkDisplayName": "networkDisplayName-value",
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


