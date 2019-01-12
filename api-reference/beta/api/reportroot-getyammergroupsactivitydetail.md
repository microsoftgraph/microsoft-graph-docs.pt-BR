---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Obtenha dados sobre as atividades de grupo do Yammer por grupo.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d589f6b8d9a5e51fe77c7da13ce3c5c0f662acce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942875"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="3365b-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="3365b-103">reportRoot: getYammerGroupsActivityDetail</span></span>

> <span data-ttu-id="3365b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3365b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3365b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3365b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3365b-106">Obtenha dados sobre as atividades de grupo do Yammer por grupo.</span><span class="sxs-lookup"><span data-stu-id="3365b-106">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="3365b-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade de grupos do Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="3365b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="3365b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3365b-108">Permissions</span></span>

<span data-ttu-id="3365b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3365b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3365b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3365b-111">Permission type</span></span>                        | <span data-ttu-id="3365b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3365b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3365b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3365b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="3365b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3365b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3365b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3365b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3365b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3365b-116">Not supported.</span></span>                           |
| <span data-ttu-id="3365b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3365b-117">Application</span></span>                            | <span data-ttu-id="3365b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3365b-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3365b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3365b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="3365b-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3365b-120">Function parameters</span></span>

<span data-ttu-id="3365b-121">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3365b-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="3365b-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3365b-122">Parameter</span></span> | <span data-ttu-id="3365b-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="3365b-123">Type</span></span>   | <span data-ttu-id="3365b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="3365b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3365b-125">ponto</span><span class="sxs-lookup"><span data-stu-id="3365b-125">period</span></span>    | <span data-ttu-id="3365b-126">string</span><span class="sxs-lookup"><span data-stu-id="3365b-126">string</span></span> | <span data-ttu-id="3365b-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3365b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3365b-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="3365b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3365b-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3365b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="3365b-130">data</span><span class="sxs-lookup"><span data-stu-id="3365b-130">date</span></span>      | <span data-ttu-id="3365b-131">Data</span><span class="sxs-lookup"><span data-stu-id="3365b-131">Date</span></span>   | <span data-ttu-id="3365b-132">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="3365b-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="3365b-133">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="3365b-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="3365b-134">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="3365b-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="3365b-135">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="3365b-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="3365b-136">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="3365b-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3365b-137">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="3365b-137">The default output type is text/csv.</span></span> <span data-ttu-id="3365b-138">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="3365b-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3365b-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3365b-139">Request headers</span></span>

| <span data-ttu-id="3365b-140">Nome</span><span class="sxs-lookup"><span data-stu-id="3365b-140">Name</span></span>          | <span data-ttu-id="3365b-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="3365b-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3365b-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="3365b-142">Authorization</span></span> | <span data-ttu-id="3365b-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3365b-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3365b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="3365b-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3365b-146">CSV</span><span class="sxs-lookup"><span data-stu-id="3365b-146">CSV</span></span>

<span data-ttu-id="3365b-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="3365b-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3365b-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="3365b-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3365b-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3365b-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3365b-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="3365b-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3365b-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="3365b-151">Report Refresh Date</span></span>
- <span data-ttu-id="3365b-152">Nome de exibição do grupo</span><span class="sxs-lookup"><span data-stu-id="3365b-152">Group Display Name</span></span>
- <span data-ttu-id="3365b-153">Excluído</span><span class="sxs-lookup"><span data-stu-id="3365b-153">Is Deleted</span></span>
- <span data-ttu-id="3365b-154">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="3365b-154">Owner Principal Name</span></span>
- <span data-ttu-id="3365b-155">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="3365b-155">Last Activity Date</span></span>
- <span data-ttu-id="3365b-156">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="3365b-156">Group Type</span></span>
- <span data-ttu-id="3365b-157">Office 365 Connected</span><span class="sxs-lookup"><span data-stu-id="3365b-157">Office 365 Connected</span></span>
- <span data-ttu-id="3365b-158">Contagem de Membros</span><span class="sxs-lookup"><span data-stu-id="3365b-158">Member Count</span></span>
- <span data-ttu-id="3365b-159">Contagem de Postagens</span><span class="sxs-lookup"><span data-stu-id="3365b-159">Posted Count</span></span>
- <span data-ttu-id="3365b-160">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="3365b-160">Read Count</span></span>
- <span data-ttu-id="3365b-161">Contagem de Curtidas</span><span class="sxs-lookup"><span data-stu-id="3365b-161">Liked Count</span></span>
- <span data-ttu-id="3365b-162">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="3365b-162">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3365b-163">JSON</span><span class="sxs-lookup"><span data-stu-id="3365b-163">JSON</span></span>

<span data-ttu-id="3365b-164">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3365b-164">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="3365b-165">O tamanho de página padrão para essa solicitação é 200 itens.</span><span class="sxs-lookup"><span data-stu-id="3365b-165">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="3365b-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3365b-166">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3365b-167">CSV</span><span class="sxs-lookup"><span data-stu-id="3365b-167">CSV</span></span>

<span data-ttu-id="3365b-168">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="3365b-168">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3365b-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3365b-169">Request</span></span>

<span data-ttu-id="3365b-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3365b-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="3365b-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="3365b-171">Response</span></span>

<span data-ttu-id="3365b-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3365b-172">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3365b-173">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="3365b-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="3365b-174">JSON</span><span class="sxs-lookup"><span data-stu-id="3365b-174">JSON</span></span>

<span data-ttu-id="3365b-175">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="3365b-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3365b-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3365b-176">Request</span></span>

<span data-ttu-id="3365b-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3365b-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="3365b-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="3365b-178">Response</span></span>

<span data-ttu-id="3365b-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3365b-179">The following is an example of the response.</span></span>

> <span data-ttu-id="3365b-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3365b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
