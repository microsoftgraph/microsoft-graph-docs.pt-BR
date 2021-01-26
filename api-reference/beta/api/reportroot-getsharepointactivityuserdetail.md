---
title: 'reportRoot: getSharePointActivityUserDetail'
description: Obtenha dados sobre as atividades do SharePoint por usuário.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 73bdf1d978f3c589f678053895e788120aabca24
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981897"
---
# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="20167-103">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="20167-103">reportRoot: getSharePointActivityUserDetail</span></span>

<span data-ttu-id="20167-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20167-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20167-105">Obtenha dados sobre as atividades do SharePoint por usuário.</span><span class="sxs-lookup"><span data-stu-id="20167-105">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="20167-106">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte [relatórios do Microsoft 365 - atividade do SharePoint.](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)</span><span class="sxs-lookup"><span data-stu-id="20167-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="20167-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="20167-107">Permissions</span></span>

<span data-ttu-id="20167-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20167-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20167-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20167-110">Permission type</span></span>                        | <span data-ttu-id="20167-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20167-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="20167-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20167-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="20167-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="20167-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="20167-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20167-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20167-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20167-115">Not supported.</span></span>                           |
| <span data-ttu-id="20167-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20167-116">Application</span></span>                            | <span data-ttu-id="20167-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="20167-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="20167-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="20167-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="20167-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="20167-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="20167-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20167-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="20167-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="20167-121">Function parameters</span></span>

<span data-ttu-id="20167-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="20167-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="20167-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="20167-123">Parameter</span></span> | <span data-ttu-id="20167-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="20167-124">Type</span></span>   | <span data-ttu-id="20167-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="20167-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="20167-126">ponto</span><span class="sxs-lookup"><span data-stu-id="20167-126">period</span></span>    | <span data-ttu-id="20167-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20167-127">string</span></span> | <span data-ttu-id="20167-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="20167-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="20167-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="20167-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="20167-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="20167-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="20167-131">data</span><span class="sxs-lookup"><span data-stu-id="20167-131">date</span></span>      | <span data-ttu-id="20167-132">Data</span><span class="sxs-lookup"><span data-stu-id="20167-132">Date</span></span>   | <span data-ttu-id="20167-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="20167-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="20167-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="20167-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="20167-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="20167-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="20167-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="20167-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="20167-137">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="20167-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="20167-138">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="20167-138">The default output type is text/csv.</span></span> <span data-ttu-id="20167-139">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta $format OData definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="20167-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20167-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20167-140">Request headers</span></span>

| <span data-ttu-id="20167-141">Nome</span><span class="sxs-lookup"><span data-stu-id="20167-141">Name</span></span>          | <span data-ttu-id="20167-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="20167-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="20167-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="20167-143">Authorization</span></span> | <span data-ttu-id="20167-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20167-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="20167-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="20167-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="20167-147">CSV</span><span class="sxs-lookup"><span data-stu-id="20167-147">CSV</span></span>

<span data-ttu-id="20167-148">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="20167-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="20167-149">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="20167-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="20167-150">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="20167-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="20167-151">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="20167-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="20167-152">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="20167-152">Report Refresh Date</span></span>
- <span data-ttu-id="20167-153">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="20167-153">User Principal Name</span></span>
- <span data-ttu-id="20167-154">Excluído</span><span class="sxs-lookup"><span data-stu-id="20167-154">Is Deleted</span></span>
- <span data-ttu-id="20167-155">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="20167-155">Deleted Date</span></span>
- <span data-ttu-id="20167-156">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="20167-156">Last Activity Date</span></span>
- <span data-ttu-id="20167-157">Contagem de arquivos exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="20167-157">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="20167-158">Contagem de arquivos sincronizados</span><span class="sxs-lookup"><span data-stu-id="20167-158">Synced File Count</span></span>
- <span data-ttu-id="20167-159">Contagem de arquivos compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="20167-159">Shared Internally File Count</span></span>
- <span data-ttu-id="20167-160">Contagem de arquivos compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="20167-160">Shared Externally File Count</span></span>
- <span data-ttu-id="20167-161">Contagem de páginas visitadas</span><span class="sxs-lookup"><span data-stu-id="20167-161">Visited Page Count</span></span>
- <span data-ttu-id="20167-162">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="20167-162">Assigned Products</span></span>
- <span data-ttu-id="20167-163">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="20167-163">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="20167-164">JSON</span><span class="sxs-lookup"><span data-stu-id="20167-164">JSON</span></span>

<span data-ttu-id="20167-165">Se bem-sucedido, este método retorna um código de resposta e um `200 OK` **[objeto sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20167-165">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="20167-166">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="20167-166">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="20167-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20167-167">Example</span></span>

### <a name="csv"></a><span data-ttu-id="20167-168">CSV</span><span class="sxs-lookup"><span data-stu-id="20167-168">CSV</span></span>

<span data-ttu-id="20167-169">A seguir está um exemplo que saída CSV.</span><span class="sxs-lookup"><span data-stu-id="20167-169">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="20167-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20167-170">Request</span></span>

<span data-ttu-id="20167-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="20167-171">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointactivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="20167-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="20167-172">Response</span></span>

<span data-ttu-id="20167-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="20167-173">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="20167-174">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="20167-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="20167-175">JSON</span><span class="sxs-lookup"><span data-stu-id="20167-175">JSON</span></span>

<span data-ttu-id="20167-176">A seguir está um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="20167-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="20167-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20167-177">Request</span></span>

<span data-ttu-id="20167-178">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="20167-178">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointactivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="20167-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="20167-179">Response</span></span>

<span data-ttu-id="20167-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="20167-180">The following is an example of the response.</span></span>

> <span data-ttu-id="20167-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20167-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


