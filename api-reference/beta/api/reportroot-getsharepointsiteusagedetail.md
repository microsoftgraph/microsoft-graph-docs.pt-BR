---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: Obtenha dados sobre o uso do site do SharePoint.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: b58d90ef3be8a723190909ee960f659de6f6c58b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049062"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="543f0-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="543f0-103">reportRoot: getSharePointSiteUsageDetail</span></span>

<span data-ttu-id="543f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="543f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="543f0-105">Obtenha dados sobre o uso do site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="543f0-105">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="543f0-106">**Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - SharePoint uso do site](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="543f0-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="543f0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="543f0-107">Permissions</span></span>

<span data-ttu-id="543f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="543f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="543f0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="543f0-110">Permission type</span></span>                        | <span data-ttu-id="543f0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="543f0-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="543f0-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="543f0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="543f0-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="543f0-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="543f0-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="543f0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="543f0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="543f0-115">Not supported.</span></span>                           |
| <span data-ttu-id="543f0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="543f0-116">Application</span></span>                            | <span data-ttu-id="543f0-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="543f0-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="543f0-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="543f0-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="543f0-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="543f0-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="543f0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="543f0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="543f0-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="543f0-121">Function parameters</span></span>

<span data-ttu-id="543f0-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="543f0-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="543f0-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="543f0-123">Parameter</span></span> | <span data-ttu-id="543f0-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="543f0-124">Type</span></span>   | <span data-ttu-id="543f0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="543f0-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="543f0-126">ponto</span><span class="sxs-lookup"><span data-stu-id="543f0-126">period</span></span>    | <span data-ttu-id="543f0-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="543f0-127">string</span></span> | <span data-ttu-id="543f0-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="543f0-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="543f0-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="543f0-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="543f0-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="543f0-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="543f0-131">data</span><span class="sxs-lookup"><span data-stu-id="543f0-131">date</span></span>      | <span data-ttu-id="543f0-132">Data</span><span class="sxs-lookup"><span data-stu-id="543f0-132">Date</span></span>   | <span data-ttu-id="543f0-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="543f0-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="543f0-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="543f0-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="543f0-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="543f0-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="543f0-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="543f0-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="543f0-137">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="543f0-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="543f0-138">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="543f0-138">The default output type is text/csv.</span></span> <span data-ttu-id="543f0-139">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="543f0-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="543f0-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="543f0-140">Request headers</span></span>

| <span data-ttu-id="543f0-141">Nome</span><span class="sxs-lookup"><span data-stu-id="543f0-141">Name</span></span>          | <span data-ttu-id="543f0-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="543f0-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="543f0-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="543f0-143">Authorization</span></span> | <span data-ttu-id="543f0-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="543f0-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="543f0-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="543f0-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="543f0-147">CSV</span><span class="sxs-lookup"><span data-stu-id="543f0-147">CSV</span></span>

<span data-ttu-id="543f0-148">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="543f0-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="543f0-149">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="543f0-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="543f0-150">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="543f0-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="543f0-151">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="543f0-151">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="543f0-152">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="543f0-152">Report Refresh Date</span></span>
- <span data-ttu-id="543f0-153">Site Id</span><span class="sxs-lookup"><span data-stu-id="543f0-153">Site Id</span></span>
- <span data-ttu-id="543f0-154">URL do site</span><span class="sxs-lookup"><span data-stu-id="543f0-154">Site URL</span></span>
- <span data-ttu-id="543f0-155">Nome de exibição do proprietário</span><span class="sxs-lookup"><span data-stu-id="543f0-155">Owner Display Name</span></span>
- <span data-ttu-id="543f0-156">Excluído</span><span class="sxs-lookup"><span data-stu-id="543f0-156">Is Deleted</span></span>
- <span data-ttu-id="543f0-157">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="543f0-157">Last Activity Date</span></span>
- <span data-ttu-id="543f0-158">ID do rótulo de sensibilidade do site</span><span class="sxs-lookup"><span data-stu-id="543f0-158">Site Sensitivity Label Id</span></span>
- <span data-ttu-id="543f0-159">Compartilhamento Externo</span><span class="sxs-lookup"><span data-stu-id="543f0-159">External Sharing</span></span>
- <span data-ttu-id="543f0-160">Política de dispositivo sem gestão</span><span class="sxs-lookup"><span data-stu-id="543f0-160">Unmanaged Device Policy</span></span>
- <span data-ttu-id="543f0-161">Localização Geográfica</span><span class="sxs-lookup"><span data-stu-id="543f0-161">Geo Location</span></span>
- <span data-ttu-id="543f0-162">Contagem de arquivos</span><span class="sxs-lookup"><span data-stu-id="543f0-162">File Count</span></span>
- <span data-ttu-id="543f0-163">Contagem de arquivos ativos</span><span class="sxs-lookup"><span data-stu-id="543f0-163">Active File Count</span></span>
- <span data-ttu-id="543f0-164">Contagem de visualização de página</span><span class="sxs-lookup"><span data-stu-id="543f0-164">Page View Count</span></span>
- <span data-ttu-id="543f0-165">Contagem de páginas visitadas</span><span class="sxs-lookup"><span data-stu-id="543f0-165">Visited Page Count</span></span>
- <span data-ttu-id="543f0-166">Contagem de links anônimos</span><span class="sxs-lookup"><span data-stu-id="543f0-166">Anonymous Link Count</span></span>
- <span data-ttu-id="543f0-167">Contagem de vínculos da empresa</span><span class="sxs-lookup"><span data-stu-id="543f0-167">Company Link Count</span></span>
- <span data-ttu-id="543f0-168">Link seguro para contagem de convidados</span><span class="sxs-lookup"><span data-stu-id="543f0-168">Secure Link For Guest Count</span></span>
- <span data-ttu-id="543f0-169">Link Seguro para Contagem de Membros</span><span class="sxs-lookup"><span data-stu-id="543f0-169">Secure Link For Member Count</span></span>
- <span data-ttu-id="543f0-170">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="543f0-170">Storage Used (Byte)</span></span>
- <span data-ttu-id="543f0-171">Armazenamento alocado (bytes)</span><span class="sxs-lookup"><span data-stu-id="543f0-171">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="543f0-172">Modelo de Web raiz</span><span class="sxs-lookup"><span data-stu-id="543f0-172">Root Web Template</span></span>
- <span data-ttu-id="543f0-173">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="543f0-173">Owner Principal Name</span></span>
- <span data-ttu-id="543f0-174">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="543f0-174">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="543f0-175">JSON</span><span class="sxs-lookup"><span data-stu-id="543f0-175">JSON</span></span>

<span data-ttu-id="543f0-176">Se tiver êxito, este método retornará um código de resposta e um `200 OK` **[objeto sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="543f0-176">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="543f0-177">O tamanho padrão da página para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="543f0-177">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="543f0-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="543f0-178">Example</span></span>

### <a name="csv"></a><span data-ttu-id="543f0-179">CSV</span><span class="sxs-lookup"><span data-stu-id="543f0-179">CSV</span></span>

<span data-ttu-id="543f0-180">A seguir, um exemplo que dá saída ao CSV.</span><span class="sxs-lookup"><span data-stu-id="543f0-180">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="543f0-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="543f0-181">Request</span></span>

<span data-ttu-id="543f0-182">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="543f0-182">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointsiteusagedetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="543f0-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="543f0-183">Response</span></span>

<span data-ttu-id="543f0-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="543f0-184">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="543f0-185">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="543f0-185">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,Site Sensitivity Label Id,External Sharing,Unmanaged Device Policy,Geo Location,File Count,Active File Count,Page View Count,Visited Page Count,Anonymous Link Count,Company Link Count,Secure Link For Guest Count,Secure Link For Member Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Owner Principal Name,Report Period
```

### <a name="json"></a><span data-ttu-id="543f0-186">JSON</span><span class="sxs-lookup"><span data-stu-id="543f0-186">JSON</span></span>

<span data-ttu-id="543f0-187">A seguir, um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="543f0-187">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="543f0-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="543f0-188">Request</span></span>

<span data-ttu-id="543f0-189">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="543f0-189">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointsiteusagedetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="543f0-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="543f0-190">Response</span></span>

<span data-ttu-id="543f0-191">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="543f0-191">The following is an example of the response.</span></span>

> <span data-ttu-id="543f0-192">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="543f0-192">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "SiteSensitivityLabelId": "SiteSensitivityLabelId-value",
      "ExternalSharing": false,
      "UnmanagedDevicePolicy": "UnmanagedDevicePolicy-value",
      "GeoLocation": "GeoLocation-value",
      "fileCount": 170, 
      "activeFileCount": 25, 
      "pageViewCount": 7, 
      "visitedPageCount": 3, 
      "AnonymousLinkCount": 5,
      "CompanyLinkCount": 8,
      "SecureLinkForGuestCount": 13,
      "SecureLinkForMemberCount": 11,
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


