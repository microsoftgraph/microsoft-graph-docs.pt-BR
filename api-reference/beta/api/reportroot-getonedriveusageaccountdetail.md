---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: Obtenha dados sobre o uso do OneDrive por conta.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 1aa7de008f1791908786111a87c1ab046df7f42e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960298"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="b6523-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="b6523-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

> <span data-ttu-id="b6523-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b6523-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6523-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b6523-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b6523-106">Obtenha dados sobre o uso do OneDrive por conta.</span><span class="sxs-lookup"><span data-stu-id="b6523-106">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="b6523-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="b6523-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="b6523-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6523-108">Permissions</span></span>

<span data-ttu-id="b6523-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6523-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b6523-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6523-111">Permission type</span></span>                        | <span data-ttu-id="b6523-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6523-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b6523-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6523-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b6523-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6523-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b6523-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6523-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6523-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6523-116">Not supported.</span></span>                           |
| <span data-ttu-id="b6523-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6523-117">Application</span></span>                            | <span data-ttu-id="b6523-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6523-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b6523-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6523-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="b6523-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b6523-120">Function parameters</span></span>

<span data-ttu-id="b6523-121">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b6523-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b6523-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b6523-122">Parameter</span></span> | <span data-ttu-id="b6523-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6523-123">Type</span></span>   | <span data-ttu-id="b6523-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6523-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b6523-125">ponto</span><span class="sxs-lookup"><span data-stu-id="b6523-125">period</span></span>    | <span data-ttu-id="b6523-126">string</span><span class="sxs-lookup"><span data-stu-id="b6523-126">string</span></span> | <span data-ttu-id="b6523-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b6523-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b6523-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="b6523-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b6523-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b6523-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b6523-130">data</span><span class="sxs-lookup"><span data-stu-id="b6523-130">date</span></span>      | <span data-ttu-id="b6523-131">Data</span><span class="sxs-lookup"><span data-stu-id="b6523-131">Date</span></span>   | <span data-ttu-id="b6523-132">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="b6523-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b6523-133">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="b6523-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b6523-134">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="b6523-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b6523-135">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="b6523-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="b6523-136">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="b6523-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b6523-137">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="b6523-137">The default output type is text/csv.</span></span> <span data-ttu-id="b6523-138">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="b6523-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6523-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6523-139">Request headers</span></span>

| <span data-ttu-id="b6523-140">Nome</span><span class="sxs-lookup"><span data-stu-id="b6523-140">Name</span></span>          | <span data-ttu-id="b6523-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6523-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b6523-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6523-142">Authorization</span></span> | <span data-ttu-id="b6523-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6523-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b6523-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6523-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b6523-146">CSV</span><span class="sxs-lookup"><span data-stu-id="b6523-146">CSV</span></span>

<span data-ttu-id="b6523-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="b6523-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b6523-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="b6523-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b6523-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b6523-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b6523-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="b6523-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b6523-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="b6523-151">Report Refresh Date</span></span>
- <span data-ttu-id="b6523-152">URL do site</span><span class="sxs-lookup"><span data-stu-id="b6523-152">Site URL</span></span>
- <span data-ttu-id="b6523-153">Nome de exibição do proprietário</span><span class="sxs-lookup"><span data-stu-id="b6523-153">Owner Display Name</span></span>
- <span data-ttu-id="b6523-154">Excluído</span><span class="sxs-lookup"><span data-stu-id="b6523-154">Is Deleted</span></span>
- <span data-ttu-id="b6523-155">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="b6523-155">Last Activity Date</span></span>
- <span data-ttu-id="b6523-156">Contagem de arquivos</span><span class="sxs-lookup"><span data-stu-id="b6523-156">File Count</span></span>
- <span data-ttu-id="b6523-157">Contagem de arquivos ativos</span><span class="sxs-lookup"><span data-stu-id="b6523-157">Active File Count</span></span>
- <span data-ttu-id="b6523-158">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="b6523-158">Storage Used (Byte)</span></span>
- <span data-ttu-id="b6523-159">Armazenamento alocado (bytes)</span><span class="sxs-lookup"><span data-stu-id="b6523-159">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="b6523-160">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="b6523-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="b6523-161">JSON</span><span class="sxs-lookup"><span data-stu-id="b6523-161">JSON</span></span>

<span data-ttu-id="b6523-162">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6523-162">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** object in the response body.</span></span>

<span data-ttu-id="b6523-163">O tamanho de página padrão para essa solicitação é 200 itens.</span><span class="sxs-lookup"><span data-stu-id="b6523-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="b6523-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6523-164">Example</span></span>

<span data-ttu-id="b6523-165">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="b6523-165">The following is an example that outputs CSV.</span></span>

### <a name="csv"></a><span data-ttu-id="b6523-166">CSV</span><span class="sxs-lookup"><span data-stu-id="b6523-166">CSV</span></span>

#### <a name="request"></a><span data-ttu-id="b6523-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6523-167">Request</span></span>

<span data-ttu-id="b6523-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6523-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="b6523-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6523-169">Response</span></span>

<span data-ttu-id="b6523-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b6523-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b6523-171">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="b6523-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="b6523-172">JSON</span><span class="sxs-lookup"><span data-stu-id="b6523-172">JSON</span></span>

<span data-ttu-id="b6523-173">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="b6523-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b6523-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6523-174">Request</span></span>

<span data-ttu-id="b6523-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6523-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="b6523-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6523-176">Response</span></span>

<span data-ttu-id="b6523-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b6523-177">The following is an example of the response.</span></span>

> <span data-ttu-id="b6523-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6523-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
