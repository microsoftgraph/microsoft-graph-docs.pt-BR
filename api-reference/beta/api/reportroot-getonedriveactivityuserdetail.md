---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: Obtenha dados sobre as atividades do OneDrive por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 40b4d5485998ebc39d541977c56c2afaef203819
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538141"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="e4426-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="e4426-103">reportRoot: getOneDriveActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4426-104">Obtenha dados sobre as atividades do OneDrive por usuário.</span><span class="sxs-lookup"><span data-stu-id="e4426-104">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="e4426-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="e4426-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="e4426-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4426-106">Permissions</span></span>

<span data-ttu-id="e4426-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4426-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e4426-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4426-109">Permission type</span></span>                        | <span data-ttu-id="e4426-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4426-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e4426-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4426-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e4426-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4426-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e4426-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4426-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4426-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4426-114">Not supported.</span></span>                           |
| <span data-ttu-id="e4426-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4426-115">Application</span></span>                            | <span data-ttu-id="e4426-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4426-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e4426-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4426-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="e4426-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e4426-118">Function parameters</span></span>

<span data-ttu-id="e4426-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="e4426-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="e4426-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e4426-120">Parameter</span></span> | <span data-ttu-id="e4426-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4426-121">Type</span></span>   | <span data-ttu-id="e4426-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4426-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e4426-123">ponto</span><span class="sxs-lookup"><span data-stu-id="e4426-123">period</span></span>    | <span data-ttu-id="e4426-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4426-124">string</span></span> | <span data-ttu-id="e4426-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e4426-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e4426-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="e4426-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e4426-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e4426-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="e4426-128">data</span><span class="sxs-lookup"><span data-stu-id="e4426-128">date</span></span>      | <span data-ttu-id="e4426-129">Data</span><span class="sxs-lookup"><span data-stu-id="e4426-129">Date</span></span>   | <span data-ttu-id="e4426-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="e4426-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="e4426-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="e4426-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="e4426-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="e4426-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="e4426-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="e4426-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="e4426-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="e4426-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e4426-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="e4426-135">The default output type is text/csv.</span></span> <span data-ttu-id="e4426-136">No enTanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="e4426-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4426-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4426-137">Request headers</span></span>

| <span data-ttu-id="e4426-138">Nome</span><span class="sxs-lookup"><span data-stu-id="e4426-138">Name</span></span>          | <span data-ttu-id="e4426-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4426-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e4426-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4426-140">Authorization</span></span> | <span data-ttu-id="e4426-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4426-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e4426-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4426-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e4426-144">CSV</span><span class="sxs-lookup"><span data-stu-id="e4426-144">CSV</span></span>

<span data-ttu-id="e4426-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="e4426-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e4426-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="e4426-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e4426-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e4426-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e4426-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="e4426-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e4426-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="e4426-149">Report Refresh Date</span></span>
- <span data-ttu-id="e4426-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="e4426-150">User Principal Name</span></span>
- <span data-ttu-id="e4426-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="e4426-151">Is Deleted</span></span>
- <span data-ttu-id="e4426-152">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="e4426-152">Deleted Date</span></span>
- <span data-ttu-id="e4426-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="e4426-153">Last Activity Date</span></span>
- <span data-ttu-id="e4426-154">Contagem de arquivos exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="e4426-154">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="e4426-155">Contagem de arquivos sincronizados</span><span class="sxs-lookup"><span data-stu-id="e4426-155">Synced File Count</span></span>
- <span data-ttu-id="e4426-156">Contagem de arquivos compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="e4426-156">Shared Internally File Count</span></span>
- <span data-ttu-id="e4426-157">Contagem de arquivos compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="e4426-157">Shared Externally File Count</span></span>
- <span data-ttu-id="e4426-158">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="e4426-158">Assigned Products</span></span>
- <span data-ttu-id="e4426-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="e4426-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e4426-160">JSON</span><span class="sxs-lookup"><span data-stu-id="e4426-160">JSON</span></span>

<span data-ttu-id="e4426-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4426-161">If successful, this method returns a `200 OK` response code and a **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="e4426-162">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="e4426-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="e4426-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4426-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e4426-164">CSV</span><span class="sxs-lookup"><span data-stu-id="e4426-164">CSV</span></span>

<span data-ttu-id="e4426-165">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="e4426-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e4426-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4426-166">Request</span></span>

<span data-ttu-id="e4426-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4426-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e4426-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4426-168">Response</span></span>

<span data-ttu-id="e4426-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4426-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e4426-170">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="e4426-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="e4426-171">JSON</span><span class="sxs-lookup"><span data-stu-id="e4426-171">JSON</span></span>

<span data-ttu-id="e4426-172">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="e4426-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e4426-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4426-173">Request</span></span>

<span data-ttu-id="e4426-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4426-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e4426-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4426-175">Response</span></span>

<span data-ttu-id="e4426-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4426-176">The following is an example of the response.</span></span>

> <span data-ttu-id="e4426-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4426-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "viewedOrEditedFileCount": 1, 
      "syncedFileCount": 0, 
      "sharedInternallyFileCount": 0, 
      "sharedExternallyFileCount": 0, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
