---
title: 'reportRoot: getOneDriveActivityFileCounts'
description: Obtenha o número de usuários únicos licenciados que realizaram interações de arquivos contra qualquer conta do OneDrive.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: e3a5d9cd840d47fd950330758e64b33625052904
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518349"
---
# <a name="reportroot-getonedriveactivityfilecounts"></a><span data-ttu-id="f1b3d-103">reportRoot: getOneDriveActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="f1b3d-103">reportRoot: getOneDriveActivityFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1b3d-104">Obtenha o número de usuários únicos licenciados que realizaram interações de arquivos contra qualquer conta do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-104">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span>

> <span data-ttu-id="f1b3d-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="f1b3d-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="f1b3d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1b3d-106">Permissions</span></span>

<span data-ttu-id="f1b3d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1b3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f1b3d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1b3d-109">Permission type</span></span>                        | <span data-ttu-id="f1b3d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1b3d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f1b3d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1b3d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1b3d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1b3d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f1b3d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1b3d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1b3d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-114">Not supported.</span></span>                           |
| <span data-ttu-id="f1b3d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1b3d-115">Application</span></span>                            | <span data-ttu-id="f1b3d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1b3d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f1b3d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1b3d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f1b3d-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="f1b3d-118">Function parameters</span></span>

<span data-ttu-id="f1b3d-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f1b3d-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f1b3d-120">Parameter</span></span> | <span data-ttu-id="f1b3d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1b3d-121">Type</span></span>   | <span data-ttu-id="f1b3d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1b3d-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f1b3d-123">ponto</span><span class="sxs-lookup"><span data-stu-id="f1b3d-123">period</span></span>    | <span data-ttu-id="f1b3d-124">string</span><span class="sxs-lookup"><span data-stu-id="f1b3d-124">string</span></span> | <span data-ttu-id="f1b3d-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f1b3d-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f1b3d-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f1b3d-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-128">Required.</span></span> |

<span data-ttu-id="f1b3d-129">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f1b3d-130">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-130">The default output type is text/csv.</span></span> <span data-ttu-id="f1b3d-131">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1b3d-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1b3d-132">Request headers</span></span>

| <span data-ttu-id="f1b3d-133">Nome</span><span class="sxs-lookup"><span data-stu-id="f1b3d-133">Name</span></span>          | <span data-ttu-id="f1b3d-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1b3d-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f1b3d-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1b3d-135">Authorization</span></span> | <span data-ttu-id="f1b3d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f1b3d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1b3d-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f1b3d-139">CSV</span><span class="sxs-lookup"><span data-stu-id="f1b3d-139">CSV</span></span>

<span data-ttu-id="f1b3d-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f1b3d-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f1b3d-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f1b3d-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f1b3d-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="f1b3d-144">Report Refresh Date</span></span>
- <span data-ttu-id="f1b3d-145">Exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="f1b3d-145">Viewed Or Edited</span></span>
- <span data-ttu-id="f1b3d-146">Sincronizados</span><span class="sxs-lookup"><span data-stu-id="f1b3d-146">Synced</span></span>
- <span data-ttu-id="f1b3d-147">Compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="f1b3d-147">Shared Internally</span></span>
- <span data-ttu-id="f1b3d-148">Compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="f1b3d-148">Shared Externally</span></span>
- <span data-ttu-id="f1b3d-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="f1b3d-149">Report Date</span></span>
- <span data-ttu-id="f1b3d-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="f1b3d-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="f1b3d-151">JSON</span><span class="sxs-lookup"><span data-stu-id="f1b3d-151">JSON</span></span>

<span data-ttu-id="f1b3d-152">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[siteActivitySummary](../resources/siteactivitysummary.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-152">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1b3d-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1b3d-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f1b3d-154">CSV</span><span class="sxs-lookup"><span data-stu-id="f1b3d-154">CSV</span></span>

<span data-ttu-id="f1b3d-155">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f1b3d-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1b3d-156">Request</span></span>

<span data-ttu-id="f1b3d-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityfilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityFileCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="f1b3d-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1b3d-158">Response</span></span>

<span data-ttu-id="f1b3d-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f1b3d-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="f1b3d-161">JSON</span><span class="sxs-lookup"><span data-stu-id="f1b3d-161">JSON</span></span>

<span data-ttu-id="f1b3d-162">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f1b3d-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1b3d-163">Request</span></span>

<span data-ttu-id="f1b3d-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityfilecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityFileCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="f1b3d-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1b3d-165">Response</span></span>

<span data-ttu-id="f1b3d-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-166">The following is an example of the response.</span></span>

> <span data-ttu-id="f1b3d-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1b3d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 280

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 1997, 
      "synced": 24756, 
      "sharedInternally": 7, 
      "sharedExternally": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityfilecounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
