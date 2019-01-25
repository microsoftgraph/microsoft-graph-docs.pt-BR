---
title: 'reportRoot: getOffice365GroupsActivityFileCounts'
description: Obtenha o número total de arquivos e quantos deles estavam ativos em todos os sites do grupo associados a um Grupo do Office 365.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: ef1b8fc83b6d94f0be9b3842917c3fe446e0e2d9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528106"
---
# <a name="reportroot-getoffice365groupsactivityfilecounts"></a><span data-ttu-id="cbead-103">reportRoot: getOffice365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="cbead-103">reportRoot: getOffice365GroupsActivityFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbead-104">Obtenha o número total de arquivos e quantos deles estavam ativos em todos os sites do grupo associados a um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="cbead-104">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span>

> <span data-ttu-id="cbead-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="cbead-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="cbead-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cbead-106">Permissions</span></span>

<span data-ttu-id="cbead-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbead-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cbead-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbead-109">Permission type</span></span>                        | <span data-ttu-id="cbead-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cbead-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cbead-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbead-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cbead-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbead-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cbead-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbead-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbead-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbead-114">Not supported.</span></span>                           |
| <span data-ttu-id="cbead-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbead-115">Application</span></span>                            | <span data-ttu-id="cbead-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbead-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cbead-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbead-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="cbead-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="cbead-118">Function parameters</span></span>

<span data-ttu-id="cbead-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="cbead-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="cbead-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cbead-120">Parameter</span></span> | <span data-ttu-id="cbead-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbead-121">Type</span></span>   | <span data-ttu-id="cbead-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbead-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cbead-123">ponto</span><span class="sxs-lookup"><span data-stu-id="cbead-123">period</span></span>    | <span data-ttu-id="cbead-124">string</span><span class="sxs-lookup"><span data-stu-id="cbead-124">string</span></span> | <span data-ttu-id="cbead-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="cbead-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cbead-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="cbead-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cbead-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="cbead-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="cbead-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbead-128">Required.</span></span> |

<span data-ttu-id="cbead-129">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cbead-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="cbead-130">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="cbead-130">The default output type is text/csv.</span></span> <span data-ttu-id="cbead-131">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="cbead-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cbead-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbead-132">Request headers</span></span>

| <span data-ttu-id="cbead-133">Nome</span><span class="sxs-lookup"><span data-stu-id="cbead-133">Name</span></span>          | <span data-ttu-id="cbead-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbead-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cbead-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbead-135">Authorization</span></span> | <span data-ttu-id="cbead-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbead-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cbead-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbead-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="cbead-139">CSV</span><span class="sxs-lookup"><span data-stu-id="cbead-139">CSV</span></span>

<span data-ttu-id="cbead-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="cbead-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cbead-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="cbead-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cbead-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="cbead-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cbead-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="cbead-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cbead-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="cbead-144">Report Refresh Date</span></span>
- <span data-ttu-id="cbead-145">Total</span><span class="sxs-lookup"><span data-stu-id="cbead-145">Total</span></span>
- <span data-ttu-id="cbead-146">Ativo</span><span class="sxs-lookup"><span data-stu-id="cbead-146">Active</span></span>
- <span data-ttu-id="cbead-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="cbead-147">Report Date</span></span>
- <span data-ttu-id="cbead-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="cbead-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="cbead-149">JSON</span><span class="sxs-lookup"><span data-stu-id="cbead-149">JSON</span></span>

<span data-ttu-id="cbead-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbead-150">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbead-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbead-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="cbead-152">CSV</span><span class="sxs-lookup"><span data-stu-id="cbead-152">CSV</span></span>

<span data-ttu-id="cbead-153">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="cbead-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="cbead-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbead-154">Request</span></span>

<span data-ttu-id="cbead-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbead-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivityfilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityFileCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="cbead-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbead-156">Response</span></span>

<span data-ttu-id="cbead-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cbead-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="cbead-158">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="cbead-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="cbead-159">JSON</span><span class="sxs-lookup"><span data-stu-id="cbead-159">JSON</span></span>

<span data-ttu-id="cbead-160">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="cbead-160">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="cbead-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbead-161">Request</span></span>

<span data-ttu-id="cbead-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbead-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivityfilecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityFileCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="cbead-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbead-163">Response</span></span>

<span data-ttu-id="cbead-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cbead-164">The following is an example of the response.</span></span>

> <span data-ttu-id="cbead-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbead-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityFileCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 229

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityFileCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "total": 26, 
      "active": 5, 
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
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivityfilecounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
