---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: Obtenha dados sobre o uso do site do SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: bcb7dff705a3e78552cccde70d3916c32d8a0645
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896249"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="0c4b2-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="0c4b2-103">reportRoot: getSharePointSiteUsageDetail</span></span>

<span data-ttu-id="0c4b2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c4b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c4b2-105">Obtenha dados sobre o uso do site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-105">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="0c4b2-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição de relatórios e nomes, consulte [Microsoft 365 Reports-uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="0c4b2-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="0c4b2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0c4b2-107">Permissions</span></span>

<span data-ttu-id="0c4b2-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0c4b2-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c4b2-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0c4b2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c4b2-110">Permission type</span></span>                        | <span data-ttu-id="0c4b2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c4b2-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0c4b2-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c4b2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0c4b2-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c4b2-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0c4b2-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c4b2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c4b2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-115">Not supported.</span></span>                           |
| <span data-ttu-id="0c4b2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c4b2-116">Application</span></span>                            | <span data-ttu-id="0c4b2-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c4b2-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="0c4b2-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="0c4b2-119">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="0c4b2-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="0c4b2-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c4b2-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="0c4b2-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="0c4b2-121">Function parameters</span></span>

<span data-ttu-id="0c4b2-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="0c4b2-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0c4b2-123">Parameter</span></span> | <span data-ttu-id="0c4b2-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c4b2-124">Type</span></span>   | <span data-ttu-id="0c4b2-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c4b2-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0c4b2-126">ponto</span><span class="sxs-lookup"><span data-stu-id="0c4b2-126">period</span></span>    | <span data-ttu-id="0c4b2-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c4b2-127">string</span></span> | <span data-ttu-id="0c4b2-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0c4b2-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0c4b2-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="0c4b2-131">data</span><span class="sxs-lookup"><span data-stu-id="0c4b2-131">date</span></span>      | <span data-ttu-id="0c4b2-132">Data</span><span class="sxs-lookup"><span data-stu-id="0c4b2-132">Date</span></span>   | <span data-ttu-id="0c4b2-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="0c4b2-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="0c4b2-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="0c4b2-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="0c4b2-137">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0c4b2-138">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-138">The default output type is text/csv.</span></span> <span data-ttu-id="0c4b2-139">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c4b2-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c4b2-140">Request headers</span></span>

| <span data-ttu-id="0c4b2-141">Nome</span><span class="sxs-lookup"><span data-stu-id="0c4b2-141">Name</span></span>          | <span data-ttu-id="0c4b2-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c4b2-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0c4b2-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c4b2-143">Authorization</span></span> | <span data-ttu-id="0c4b2-144">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-144">Bearer {token}.</span></span> <span data-ttu-id="0c4b2-145">Required.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-145">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0c4b2-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c4b2-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0c4b2-147">CSV</span><span class="sxs-lookup"><span data-stu-id="0c4b2-147">CSV</span></span>

<span data-ttu-id="0c4b2-148">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0c4b2-149">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0c4b2-150">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0c4b2-151">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="0c4b2-151">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="0c4b2-152">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="0c4b2-152">Report Refresh Date</span></span>
- <span data-ttu-id="0c4b2-153">ID de site</span><span class="sxs-lookup"><span data-stu-id="0c4b2-153">Site Id</span></span>
- <span data-ttu-id="0c4b2-154">URL do site</span><span class="sxs-lookup"><span data-stu-id="0c4b2-154">Site URL</span></span>
- <span data-ttu-id="0c4b2-155">Nome de exibição do proprietário</span><span class="sxs-lookup"><span data-stu-id="0c4b2-155">Owner Display Name</span></span>
- <span data-ttu-id="0c4b2-156">Excluído</span><span class="sxs-lookup"><span data-stu-id="0c4b2-156">Is Deleted</span></span>
- <span data-ttu-id="0c4b2-157">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="0c4b2-157">Last Activity Date</span></span>
- <span data-ttu-id="0c4b2-158">Contagem de arquivos</span><span class="sxs-lookup"><span data-stu-id="0c4b2-158">File Count</span></span>
- <span data-ttu-id="0c4b2-159">Contagem de arquivos ativos</span><span class="sxs-lookup"><span data-stu-id="0c4b2-159">Active File Count</span></span>
- <span data-ttu-id="0c4b2-160">Contagem de visualização de página</span><span class="sxs-lookup"><span data-stu-id="0c4b2-160">Page View Count</span></span>
- <span data-ttu-id="0c4b2-161">Contagem de páginas visitadas</span><span class="sxs-lookup"><span data-stu-id="0c4b2-161">Visited Page Count</span></span>
- <span data-ttu-id="0c4b2-162">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="0c4b2-162">Storage Used (Byte)</span></span>
- <span data-ttu-id="0c4b2-163">Armazenamento alocado (bytes)</span><span class="sxs-lookup"><span data-stu-id="0c4b2-163">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="0c4b2-164">Modelo de Web raiz</span><span class="sxs-lookup"><span data-stu-id="0c4b2-164">Root Web Template</span></span>
- <span data-ttu-id="0c4b2-165">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="0c4b2-165">Owner Principal Name</span></span>
- <span data-ttu-id="0c4b2-166">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="0c4b2-166">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0c4b2-167">JSON</span><span class="sxs-lookup"><span data-stu-id="0c4b2-167">JSON</span></span>

<span data-ttu-id="0c4b2-168">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-168">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="0c4b2-169">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-169">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="0c4b2-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c4b2-170">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0c4b2-171">CSV</span><span class="sxs-lookup"><span data-stu-id="0c4b2-171">CSV</span></span>

<span data-ttu-id="0c4b2-172">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-172">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0c4b2-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c4b2-173">Request</span></span>

<span data-ttu-id="0c4b2-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-174">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointsiteusagedetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="0c4b2-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c4b2-175">Response</span></span>

<span data-ttu-id="0c4b2-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-176">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0c4b2-177">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-177">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Owner Principal Name,Report Period
```

### <a name="json"></a><span data-ttu-id="0c4b2-178">JSON</span><span class="sxs-lookup"><span data-stu-id="0c4b2-178">JSON</span></span>

<span data-ttu-id="0c4b2-179">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-179">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0c4b2-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c4b2-180">Request</span></span>

<span data-ttu-id="0c4b2-181">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-181">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointsiteusagedetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="0c4b2-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c4b2-182">Response</span></span>

<span data-ttu-id="0c4b2-183">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-183">The following is an example of the response.</span></span>

> <span data-ttu-id="0c4b2-184">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-184">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0c4b2-185">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="0c4b2-185">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteId": "siteId-value", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 170, 
      "activeFileCount": 25, 
      "pageViewCount": 7, 
      "visitedPageCount": 3, 
      "storageUsedInBytes": 63442116, 
      "storageAllocatedInBytes": 2748779094400, 
      "rootWebTemplate": "Publishing Site", 
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
