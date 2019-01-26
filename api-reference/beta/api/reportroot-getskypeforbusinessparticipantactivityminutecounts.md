---
title: 'reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts'
description: Obtenha as tendências de uso da duração em minutos e o tipo de sessões de conferência das quais os usuários de sua organização participaram. Tipos de sessões de conferência incluem áudio/vídeo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 6677ac111a1cad24e44e4c0e77892d55069ee825
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574345"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="b0641-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="b0641-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0641-105">Obtenha as tendências de uso da duração em minutos e o tipo de sessões de conferência das quais os usuários de sua organização participaram.</span><span class="sxs-lookup"><span data-stu-id="b0641-105">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="b0641-106">Tipos de sessões de conferência incluem áudio/vídeo.</span><span class="sxs-lookup"><span data-stu-id="b0641-106">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="b0641-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do participante da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="b0641-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="b0641-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0641-108">Permissions</span></span>

<span data-ttu-id="b0641-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0641-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0641-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0641-111">Permission type</span></span>                        | <span data-ttu-id="b0641-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0641-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b0641-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0641-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0641-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0641-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b0641-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0641-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0641-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0641-116">Not supported.</span></span>                           |
| <span data-ttu-id="b0641-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0641-117">Application</span></span>                            | <span data-ttu-id="b0641-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0641-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b0641-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0641-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b0641-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b0641-120">Function parameters</span></span>

<span data-ttu-id="b0641-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="b0641-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b0641-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b0641-122">Parameter</span></span> | <span data-ttu-id="b0641-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0641-123">Type</span></span>   | <span data-ttu-id="b0641-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0641-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b0641-125">ponto</span><span class="sxs-lookup"><span data-stu-id="b0641-125">period</span></span>    | <span data-ttu-id="b0641-126">string</span><span class="sxs-lookup"><span data-stu-id="b0641-126">string</span></span> | <span data-ttu-id="b0641-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b0641-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b0641-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="b0641-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b0641-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b0641-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b0641-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0641-130">Required.</span></span> |

<span data-ttu-id="b0641-131">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b0641-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b0641-132">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="b0641-132">The default output type is text/csv.</span></span> <span data-ttu-id="b0641-133">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="b0641-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0641-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0641-134">Request headers</span></span>

| <span data-ttu-id="b0641-135">Nome</span><span class="sxs-lookup"><span data-stu-id="b0641-135">Name</span></span>          | <span data-ttu-id="b0641-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0641-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b0641-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0641-137">Authorization</span></span> | <span data-ttu-id="b0641-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0641-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b0641-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0641-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b0641-141">CSV</span><span class="sxs-lookup"><span data-stu-id="b0641-141">CSV</span></span>

<span data-ttu-id="b0641-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="b0641-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b0641-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="b0641-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b0641-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b0641-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b0641-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="b0641-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b0641-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="b0641-146">Report Refresh Date</span></span>
- <span data-ttu-id="b0641-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="b0641-147">Report Date</span></span>
- <span data-ttu-id="b0641-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="b0641-148">Report Period</span></span>
- <span data-ttu-id="b0641-149">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="b0641-149">Audio/Video</span></span>

### <a name="json"></a><span data-ttu-id="b0641-150">JSON</span><span class="sxs-lookup"><span data-stu-id="b0641-150">JSON</span></span>

<span data-ttu-id="b0641-151">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0641-151">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0641-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0641-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b0641-153">CSV</span><span class="sxs-lookup"><span data-stu-id="b0641-153">CSV</span></span>

<span data-ttu-id="b0641-154">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="b0641-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b0641-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0641-155">Request</span></span>

<span data-ttu-id="b0641-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0641-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="b0641-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0641-157">Response</span></span>

<span data-ttu-id="b0641-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b0641-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b0641-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="b0641-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video
```

### <a name="json"></a><span data-ttu-id="b0641-160">JSON</span><span class="sxs-lookup"><span data-stu-id="b0641-160">JSON</span></span>

<span data-ttu-id="b0641-161">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="b0641-161">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b0641-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0641-162">Request</span></span>

<span data-ttu-id="b0641-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0641-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="b0641-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0641-164">Response</span></span>

<span data-ttu-id="b0641-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b0641-165">The following is an example of the response.</span></span>

> <span data-ttu-id="b0641-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0641-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityMinuteCounts)", 
  "value": [
    {
      "audiovideo": 6267, 
      "reportRefreshDate": "2017-09-01", 
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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
