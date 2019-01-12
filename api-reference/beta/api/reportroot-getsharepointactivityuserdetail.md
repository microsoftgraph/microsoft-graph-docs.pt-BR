---
title: 'reportRoot: getSharePointActivityUserDetail'
description: Obtenha dados sobre as atividades do SharePoint por usuário.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 737e653d9f407e3eeaa7400b89c05a639a72f1c2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963189"
---
# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="9513e-103">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="9513e-103">reportRoot: getSharePointActivityUserDetail</span></span>

> <span data-ttu-id="9513e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9513e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9513e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9513e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9513e-106">Obtenha dados sobre as atividades do SharePoint por usuário.</span><span class="sxs-lookup"><span data-stu-id="9513e-106">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="9513e-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="9513e-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="9513e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="9513e-108">Permissions</span></span>

<span data-ttu-id="9513e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9513e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9513e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9513e-111">Permission type</span></span>                        | <span data-ttu-id="9513e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9513e-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9513e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9513e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="9513e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9513e-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9513e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9513e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9513e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9513e-116">Not supported.</span></span>                           |
| <span data-ttu-id="9513e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9513e-117">Application</span></span>                            | <span data-ttu-id="9513e-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9513e-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9513e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9513e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="9513e-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="9513e-120">Function parameters</span></span>

<span data-ttu-id="9513e-121">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="9513e-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="9513e-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9513e-122">Parameter</span></span> | <span data-ttu-id="9513e-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="9513e-123">Type</span></span>   | <span data-ttu-id="9513e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9513e-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9513e-125">ponto</span><span class="sxs-lookup"><span data-stu-id="9513e-125">period</span></span>    | <span data-ttu-id="9513e-126">string</span><span class="sxs-lookup"><span data-stu-id="9513e-126">string</span></span> | <span data-ttu-id="9513e-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9513e-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9513e-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="9513e-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9513e-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9513e-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="9513e-130">data</span><span class="sxs-lookup"><span data-stu-id="9513e-130">date</span></span>      | <span data-ttu-id="9513e-131">Data</span><span class="sxs-lookup"><span data-stu-id="9513e-131">Date</span></span>   | <span data-ttu-id="9513e-132">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="9513e-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="9513e-133">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="9513e-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="9513e-134">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="9513e-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="9513e-135">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="9513e-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="9513e-136">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="9513e-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="9513e-137">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="9513e-137">The default output type is text/csv.</span></span> <span data-ttu-id="9513e-138">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="9513e-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9513e-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9513e-139">Request headers</span></span>

| <span data-ttu-id="9513e-140">Nome</span><span class="sxs-lookup"><span data-stu-id="9513e-140">Name</span></span>          | <span data-ttu-id="9513e-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="9513e-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9513e-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="9513e-142">Authorization</span></span> | <span data-ttu-id="9513e-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9513e-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9513e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="9513e-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="9513e-146">CSV</span><span class="sxs-lookup"><span data-stu-id="9513e-146">CSV</span></span>

<span data-ttu-id="9513e-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="9513e-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9513e-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="9513e-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9513e-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9513e-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9513e-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="9513e-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9513e-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="9513e-151">Report Refresh Date</span></span>
- <span data-ttu-id="9513e-152">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="9513e-152">User Principal Name</span></span>
- <span data-ttu-id="9513e-153">Excluído</span><span class="sxs-lookup"><span data-stu-id="9513e-153">Is Deleted</span></span>
- <span data-ttu-id="9513e-154">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="9513e-154">Deleted Date</span></span>
- <span data-ttu-id="9513e-155">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="9513e-155">Last Activity Date</span></span>
- <span data-ttu-id="9513e-156">Contagem de arquivos exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="9513e-156">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="9513e-157">Contagem de arquivos sincronizados</span><span class="sxs-lookup"><span data-stu-id="9513e-157">Synced File Count</span></span>
- <span data-ttu-id="9513e-158">Contagem de arquivos compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="9513e-158">Shared Internally File Count</span></span>
- <span data-ttu-id="9513e-159">Contagem de arquivos compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="9513e-159">Shared Externally File Count</span></span>
- <span data-ttu-id="9513e-160">Contagem de páginas visitadas</span><span class="sxs-lookup"><span data-stu-id="9513e-160">Visited Page Count</span></span>
- <span data-ttu-id="9513e-161">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="9513e-161">Assigned Products</span></span>
- <span data-ttu-id="9513e-162">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="9513e-162">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="9513e-163">JSON</span><span class="sxs-lookup"><span data-stu-id="9513e-163">JSON</span></span>

<span data-ttu-id="9513e-164">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9513e-164">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="9513e-165">O tamanho de página padrão para essa solicitação é 200 itens.</span><span class="sxs-lookup"><span data-stu-id="9513e-165">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="9513e-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9513e-166">Example</span></span>

### <a name="csv"></a><span data-ttu-id="9513e-167">CSV</span><span class="sxs-lookup"><span data-stu-id="9513e-167">CSV</span></span>

<span data-ttu-id="9513e-168">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="9513e-168">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="9513e-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9513e-169">Request</span></span>

<span data-ttu-id="9513e-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9513e-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="9513e-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="9513e-171">Response</span></span>

<span data-ttu-id="9513e-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9513e-172">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9513e-173">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="9513e-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Visited Page Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="9513e-174">JSON</span><span class="sxs-lookup"><span data-stu-id="9513e-174">JSON</span></span>

<span data-ttu-id="9513e-175">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="9513e-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="9513e-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9513e-176">Request</span></span>

<span data-ttu-id="9513e-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9513e-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="9513e-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="9513e-178">Response</span></span>

<span data-ttu-id="9513e-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9513e-179">The following is an example of the response.</span></span>

> <span data-ttu-id="9513e-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9513e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 473

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "viewedOrEditedFileCount": 4, 
      "syncedFileCount": 0, 
      "sharedInternallyFileCount": 0, 
      "sharedExternallyFileCount": 0, 
      "visitedPageCount": 1, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
