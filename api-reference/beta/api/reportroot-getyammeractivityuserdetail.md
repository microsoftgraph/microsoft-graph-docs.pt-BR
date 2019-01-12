---
title: 'reportRoot: getYammerActivityUserDetail'
description: Obtenha dados sobre as atividades do Yammer por usuário.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 9e1efd17342dc7f6b4e1dca78afb76ca500f7b14
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913125"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="f5421-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="f5421-103">reportRoot: getYammerActivityUserDetail</span></span>

> <span data-ttu-id="f5421-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f5421-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5421-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f5421-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5421-106">Obtenha dados sobre as atividades do Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="f5421-106">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="f5421-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades do Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="f5421-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="f5421-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5421-108">Permissions</span></span>

<span data-ttu-id="f5421-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5421-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f5421-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5421-111">Permission type</span></span>                        | <span data-ttu-id="f5421-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5421-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f5421-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5421-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5421-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5421-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f5421-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5421-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5421-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5421-116">Not supported.</span></span>                           |
| <span data-ttu-id="f5421-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5421-117">Application</span></span>                            | <span data-ttu-id="f5421-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5421-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f5421-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5421-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="f5421-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="f5421-120">Function parameters</span></span>

<span data-ttu-id="f5421-121">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f5421-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="f5421-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f5421-122">Parameter</span></span> | <span data-ttu-id="f5421-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5421-123">Type</span></span>   | <span data-ttu-id="f5421-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5421-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f5421-125">ponto</span><span class="sxs-lookup"><span data-stu-id="f5421-125">period</span></span>    | <span data-ttu-id="f5421-126">string</span><span class="sxs-lookup"><span data-stu-id="f5421-126">string</span></span> | <span data-ttu-id="f5421-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f5421-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f5421-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="f5421-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f5421-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f5421-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="f5421-130">data</span><span class="sxs-lookup"><span data-stu-id="f5421-130">date</span></span>      | <span data-ttu-id="f5421-131">Data</span><span class="sxs-lookup"><span data-stu-id="f5421-131">Date</span></span>   | <span data-ttu-id="f5421-132">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="f5421-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="f5421-133">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="f5421-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="f5421-134">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="f5421-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="f5421-135">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="f5421-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="f5421-136">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="f5421-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f5421-137">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="f5421-137">The default output type is text/csv.</span></span> <span data-ttu-id="f5421-138">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="f5421-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5421-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5421-139">Request headers</span></span>

| <span data-ttu-id="f5421-140">Nome</span><span class="sxs-lookup"><span data-stu-id="f5421-140">Name</span></span>          | <span data-ttu-id="f5421-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5421-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f5421-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5421-142">Authorization</span></span> | <span data-ttu-id="f5421-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5421-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f5421-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5421-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f5421-146">CSV</span><span class="sxs-lookup"><span data-stu-id="f5421-146">CSV</span></span>

<span data-ttu-id="f5421-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="f5421-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f5421-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="f5421-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f5421-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f5421-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f5421-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="f5421-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f5421-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="f5421-151">Report Refresh Date</span></span>
- <span data-ttu-id="f5421-152">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="f5421-152">User Principal Name</span></span>
- <span data-ttu-id="f5421-153">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="f5421-153">Display Name</span></span>
- <span data-ttu-id="f5421-154">Estado do usuário</span><span class="sxs-lookup"><span data-stu-id="f5421-154">User State</span></span>
- <span data-ttu-id="f5421-155">Data de alteração de estado</span><span class="sxs-lookup"><span data-stu-id="f5421-155">State Change Date</span></span>
- <span data-ttu-id="f5421-156">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="f5421-156">Last Activity Date</span></span>
- <span data-ttu-id="f5421-157">Contagem de Postagens</span><span class="sxs-lookup"><span data-stu-id="f5421-157">Posted Count</span></span>
- <span data-ttu-id="f5421-158">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="f5421-158">Read Count</span></span>
- <span data-ttu-id="f5421-159">Contagem de Curtidas</span><span class="sxs-lookup"><span data-stu-id="f5421-159">Liked Count</span></span>
- <span data-ttu-id="f5421-160">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="f5421-160">Assigned Products</span></span>
- <span data-ttu-id="f5421-161">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="f5421-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="f5421-162">JSON</span><span class="sxs-lookup"><span data-stu-id="f5421-162">JSON</span></span>

<span data-ttu-id="f5421-163">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5421-163">If successful, this method returns a `200 OK` response code and a **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="f5421-164">O tamanho de página padrão para essa solicitação é 200 itens.</span><span class="sxs-lookup"><span data-stu-id="f5421-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="f5421-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5421-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f5421-166">CSV</span><span class="sxs-lookup"><span data-stu-id="f5421-166">CSV</span></span>

<span data-ttu-id="f5421-167">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="f5421-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f5421-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5421-168">Request</span></span>

<span data-ttu-id="f5421-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5421-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="f5421-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5421-170">Response</span></span>

<span data-ttu-id="f5421-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f5421-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f5421-172">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="f5421-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="f5421-173">JSON</span><span class="sxs-lookup"><span data-stu-id="f5421-173">JSON</span></span>

<span data-ttu-id="f5421-174">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="f5421-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f5421-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5421-175">Request</span></span>

<span data-ttu-id="f5421-176">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5421-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="f5421-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5421-177">Response</span></span>

<span data-ttu-id="f5421-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f5421-178">The following is an example of the response.</span></span>

> <span data-ttu-id="f5421-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5421-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
