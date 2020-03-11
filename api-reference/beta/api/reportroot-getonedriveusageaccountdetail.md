---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: Obtenha dados sobre o uso do OneDrive por conta.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 58049605f2968d40b7dd4e63ade8a75b64421b30
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588967"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="c7bf5-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="c7bf5-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

<span data-ttu-id="c7bf5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7bf5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7bf5-105">Obtenha dados sobre o uso do OneDrive por conta.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-105">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="c7bf5-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="c7bf5-106">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="c7bf5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7bf5-107">Permissions</span></span>

<span data-ttu-id="c7bf5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7bf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7bf5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7bf5-110">Permission type</span></span>                        | <span data-ttu-id="c7bf5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7bf5-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c7bf5-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7bf5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7bf5-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7bf5-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c7bf5-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7bf5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7bf5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-115">Not supported.</span></span>                           |
| <span data-ttu-id="c7bf5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7bf5-116">Application</span></span>                            | <span data-ttu-id="c7bf5-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7bf5-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="c7bf5-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="c7bf5-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="c7bf5-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="c7bf5-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7bf5-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="c7bf5-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="c7bf5-121">Function parameters</span></span>

<span data-ttu-id="c7bf5-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="c7bf5-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c7bf5-123">Parameter</span></span> | <span data-ttu-id="c7bf5-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7bf5-124">Type</span></span>   | <span data-ttu-id="c7bf5-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7bf5-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c7bf5-126">ponto</span><span class="sxs-lookup"><span data-stu-id="c7bf5-126">period</span></span>    | <span data-ttu-id="c7bf5-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7bf5-127">string</span></span> | <span data-ttu-id="c7bf5-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c7bf5-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c7bf5-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="c7bf5-131">data</span><span class="sxs-lookup"><span data-stu-id="c7bf5-131">date</span></span>      | <span data-ttu-id="c7bf5-132">Data</span><span class="sxs-lookup"><span data-stu-id="c7bf5-132">Date</span></span>   | <span data-ttu-id="c7bf5-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="c7bf5-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="c7bf5-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="c7bf5-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="c7bf5-137">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c7bf5-138">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-138">The default output type is text/csv.</span></span> <span data-ttu-id="c7bf5-139">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7bf5-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7bf5-140">Request headers</span></span>

| <span data-ttu-id="c7bf5-141">Nome</span><span class="sxs-lookup"><span data-stu-id="c7bf5-141">Name</span></span>          | <span data-ttu-id="c7bf5-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7bf5-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c7bf5-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7bf5-143">Authorization</span></span> | <span data-ttu-id="c7bf5-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c7bf5-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7bf5-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c7bf5-147">CSV</span><span class="sxs-lookup"><span data-stu-id="c7bf5-147">CSV</span></span>

<span data-ttu-id="c7bf5-148">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c7bf5-149">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c7bf5-150">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c7bf5-151">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c7bf5-152">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="c7bf5-152">Report Refresh Date</span></span>
- <span data-ttu-id="c7bf5-153">URL do site</span><span class="sxs-lookup"><span data-stu-id="c7bf5-153">Site URL</span></span>
- <span data-ttu-id="c7bf5-154">Nome de exibição do proprietário</span><span class="sxs-lookup"><span data-stu-id="c7bf5-154">Owner Display Name</span></span>
- <span data-ttu-id="c7bf5-155">Excluído</span><span class="sxs-lookup"><span data-stu-id="c7bf5-155">Is Deleted</span></span>
- <span data-ttu-id="c7bf5-156">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="c7bf5-156">Last Activity Date</span></span>
- <span data-ttu-id="c7bf5-157">Contagem de arquivos</span><span class="sxs-lookup"><span data-stu-id="c7bf5-157">File Count</span></span>
- <span data-ttu-id="c7bf5-158">Contagem de arquivos ativos</span><span class="sxs-lookup"><span data-stu-id="c7bf5-158">Active File Count</span></span>
- <span data-ttu-id="c7bf5-159">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="c7bf5-159">Storage Used (Byte)</span></span>
- <span data-ttu-id="c7bf5-160">Armazenamento alocado (bytes)</span><span class="sxs-lookup"><span data-stu-id="c7bf5-160">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="c7bf5-161">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="c7bf5-161">Owner Principal Name</span></span>
- <span data-ttu-id="c7bf5-162">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="c7bf5-162">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="c7bf5-163">JSON</span><span class="sxs-lookup"><span data-stu-id="c7bf5-163">JSON</span></span>

<span data-ttu-id="c7bf5-164">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-164">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** object in the response body.</span></span>

<span data-ttu-id="c7bf5-165">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-165">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="c7bf5-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7bf5-166">Example</span></span>

<span data-ttu-id="c7bf5-167">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-167">The following is an example that outputs CSV.</span></span>

### <a name="csv"></a><span data-ttu-id="c7bf5-168">CSV</span><span class="sxs-lookup"><span data-stu-id="c7bf5-168">CSV</span></span>

#### <a name="request"></a><span data-ttu-id="c7bf5-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7bf5-169">Request</span></span>

<span data-ttu-id="c7bf5-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveusageaccountdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="c7bf5-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7bf5-171">Response</span></span>

<span data-ttu-id="c7bf5-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-172">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c7bf5-173">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Owner Principal Name,Report Period
```

### <a name="json"></a><span data-ttu-id="c7bf5-174">JSON</span><span class="sxs-lookup"><span data-stu-id="c7bf5-174">JSON</span></span>

<span data-ttu-id="c7bf5-175">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c7bf5-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7bf5-176">Request</span></span>

<span data-ttu-id="c7bf5-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-177">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveusageaccountdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="c7bf5-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7bf5-178">Response</span></span>

<span data-ttu-id="c7bf5-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-179">The following is an example of the response.</span></span>

> <span data-ttu-id="c7bf5-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7bf5-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 9, 
      "activeFileCount": 5, 
      "storageUsedInBytes": 12190375, 
      "storageAllocatedInBytes": 549755813880, 
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
