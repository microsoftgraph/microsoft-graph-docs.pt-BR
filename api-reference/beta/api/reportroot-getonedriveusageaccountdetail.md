---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: Obtenha dados sobre o uso do OneDrive por conta.
ms.openlocfilehash: 8fc91c65a7a790cec6d13169ab10a13b02b7951a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034153"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="4bc1f-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="4bc1f-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

> <span data-ttu-id="4bc1f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4bc1f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4bc1f-106">Obtenha dados sobre o uso do OneDrive por conta.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-106">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="4bc1f-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="4bc1f-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="4bc1f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4bc1f-108">Permissions</span></span>

<span data-ttu-id="4bc1f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bc1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4bc1f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bc1f-111">Permission type</span></span>                        | <span data-ttu-id="4bc1f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4bc1f-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4bc1f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bc1f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4bc1f-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bc1f-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4bc1f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bc1f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bc1f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-116">Not supported.</span></span>                           |
| <span data-ttu-id="4bc1f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bc1f-117">Application</span></span>                            | <span data-ttu-id="4bc1f-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bc1f-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4bc1f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bc1f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="4bc1f-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="4bc1f-120">Function parameters</span></span>

<span data-ttu-id="4bc1f-121">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="4bc1f-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4bc1f-122">Parameter</span></span> | <span data-ttu-id="4bc1f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bc1f-123">Type</span></span>   | <span data-ttu-id="4bc1f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bc1f-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4bc1f-125">ponto</span><span class="sxs-lookup"><span data-stu-id="4bc1f-125">period</span></span>    | <span data-ttu-id="4bc1f-126">string</span><span class="sxs-lookup"><span data-stu-id="4bc1f-126">string</span></span> | <span data-ttu-id="4bc1f-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4bc1f-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4bc1f-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="4bc1f-130">data</span><span class="sxs-lookup"><span data-stu-id="4bc1f-130">date</span></span>      | <span data-ttu-id="4bc1f-131">Data</span><span class="sxs-lookup"><span data-stu-id="4bc1f-131">Date</span></span>   | <span data-ttu-id="4bc1f-132">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="4bc1f-133">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="4bc1f-134">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="4bc1f-135">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="4bc1f-136">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4bc1f-137">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-137">The default output type is text/csv.</span></span> <span data-ttu-id="4bc1f-138">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4bc1f-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bc1f-139">Request headers</span></span>

| <span data-ttu-id="4bc1f-140">Nome</span><span class="sxs-lookup"><span data-stu-id="4bc1f-140">Name</span></span>          | <span data-ttu-id="4bc1f-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bc1f-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4bc1f-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="4bc1f-142">Authorization</span></span> | <span data-ttu-id="4bc1f-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4bc1f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bc1f-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4bc1f-146">CSV</span><span class="sxs-lookup"><span data-stu-id="4bc1f-146">CSV</span></span>

<span data-ttu-id="4bc1f-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4bc1f-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4bc1f-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4bc1f-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4bc1f-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="4bc1f-151">Report Refresh Date</span></span>
- <span data-ttu-id="4bc1f-152">URL do site</span><span class="sxs-lookup"><span data-stu-id="4bc1f-152">Site URL</span></span>
- <span data-ttu-id="4bc1f-153">Nome de exibição do proprietário</span><span class="sxs-lookup"><span data-stu-id="4bc1f-153">Owner Display Name</span></span>
- <span data-ttu-id="4bc1f-154">Excluído</span><span class="sxs-lookup"><span data-stu-id="4bc1f-154">Is Deleted</span></span>
- <span data-ttu-id="4bc1f-155">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="4bc1f-155">Last Activity Date</span></span>
- <span data-ttu-id="4bc1f-156">Contagem de arquivos</span><span class="sxs-lookup"><span data-stu-id="4bc1f-156">File Count</span></span>
- <span data-ttu-id="4bc1f-157">Contagem de arquivos ativos</span><span class="sxs-lookup"><span data-stu-id="4bc1f-157">Active File Count</span></span>
- <span data-ttu-id="4bc1f-158">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="4bc1f-158">Storage Used (Byte)</span></span>
- <span data-ttu-id="4bc1f-159">Armazenamento alocado (bytes)</span><span class="sxs-lookup"><span data-stu-id="4bc1f-159">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="4bc1f-160">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="4bc1f-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4bc1f-161">JSON</span><span class="sxs-lookup"><span data-stu-id="4bc1f-161">JSON</span></span>

<span data-ttu-id="4bc1f-162">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-162">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** object in the response body.</span></span>

<span data-ttu-id="4bc1f-163">O tamanho de página padrão para essa solicitação é 200 itens.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="4bc1f-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bc1f-164">Example</span></span>

<span data-ttu-id="4bc1f-165">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-165">The following is an example that outputs CSV.</span></span>

### <a name="csv"></a><span data-ttu-id="4bc1f-166">CSV</span><span class="sxs-lookup"><span data-stu-id="4bc1f-166">CSV</span></span>

#### <a name="request"></a><span data-ttu-id="4bc1f-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bc1f-167">Request</span></span>

<span data-ttu-id="4bc1f-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="4bc1f-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bc1f-169">Response</span></span>

<span data-ttu-id="4bc1f-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4bc1f-171">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="4bc1f-172">JSON</span><span class="sxs-lookup"><span data-stu-id="4bc1f-172">JSON</span></span>

<span data-ttu-id="4bc1f-173">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4bc1f-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bc1f-174">Request</span></span>

<span data-ttu-id="4bc1f-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="4bc1f-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bc1f-176">Response</span></span>

<span data-ttu-id="4bc1f-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-177">The following is an example of the response.</span></span>

> <span data-ttu-id="4bc1f-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4bc1f-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
