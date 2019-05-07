---
title: 'reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts'
description: Obtenha as tendências de uso da duração em minutos e o tipo de sessões de conferência das quais os usuários de sua organização participaram. Tipos de sessões de conferência incluem áudio/vídeo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5ec4819c2e7f937bed7e06946dda1a43ad2c3539
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639191"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="e0f05-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="e0f05-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0f05-105">Obtenha as tendências de uso da duração em minutos e o tipo de sessões de conferência das quais os usuários de sua organização participaram.</span><span class="sxs-lookup"><span data-stu-id="e0f05-105">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="e0f05-106">Tipos de sessões de conferência incluem áudio/vídeo.</span><span class="sxs-lookup"><span data-stu-id="e0f05-106">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="e0f05-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do participante da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="e0f05-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="e0f05-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0f05-108">Permissions</span></span>

<span data-ttu-id="e0f05-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0f05-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0f05-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0f05-111">Permission type</span></span>                        | <span data-ttu-id="e0f05-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0f05-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e0f05-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0f05-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0f05-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0f05-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e0f05-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0f05-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0f05-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0f05-116">Not supported.</span></span>                           |
| <span data-ttu-id="e0f05-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0f05-117">Application</span></span>                            | <span data-ttu-id="e0f05-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0f05-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e0f05-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0f05-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e0f05-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e0f05-120">Function parameters</span></span>

<span data-ttu-id="e0f05-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="e0f05-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e0f05-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e0f05-122">Parameter</span></span> | <span data-ttu-id="e0f05-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0f05-123">Type</span></span>   | <span data-ttu-id="e0f05-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0f05-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e0f05-125">ponto</span><span class="sxs-lookup"><span data-stu-id="e0f05-125">period</span></span>    | <span data-ttu-id="e0f05-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0f05-126">string</span></span> | <span data-ttu-id="e0f05-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e0f05-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e0f05-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="e0f05-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e0f05-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e0f05-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e0f05-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0f05-130">Required.</span></span> |

<span data-ttu-id="e0f05-131">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e0f05-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e0f05-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="e0f05-132">The default output type is text/csv.</span></span> <span data-ttu-id="e0f05-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="e0f05-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0f05-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0f05-134">Request headers</span></span>

| <span data-ttu-id="e0f05-135">Nome</span><span class="sxs-lookup"><span data-stu-id="e0f05-135">Name</span></span>          | <span data-ttu-id="e0f05-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0f05-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e0f05-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0f05-137">Authorization</span></span> | <span data-ttu-id="e0f05-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0f05-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e0f05-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0f05-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e0f05-141">CSV</span><span class="sxs-lookup"><span data-stu-id="e0f05-141">CSV</span></span>

<span data-ttu-id="e0f05-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="e0f05-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e0f05-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="e0f05-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e0f05-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e0f05-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e0f05-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="e0f05-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e0f05-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="e0f05-146">Report Refresh Date</span></span>
- <span data-ttu-id="e0f05-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="e0f05-147">Report Date</span></span>
- <span data-ttu-id="e0f05-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="e0f05-148">Report Period</span></span>
- <span data-ttu-id="e0f05-149">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="e0f05-149">Audio/Video</span></span>

### <a name="json"></a><span data-ttu-id="e0f05-150">JSON</span><span class="sxs-lookup"><span data-stu-id="e0f05-150">JSON</span></span>

<span data-ttu-id="e0f05-151">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0f05-151">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0f05-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0f05-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e0f05-153">CSV</span><span class="sxs-lookup"><span data-stu-id="e0f05-153">CSV</span></span>

<span data-ttu-id="e0f05-154">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="e0f05-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e0f05-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0f05-155">Request</span></span>

<span data-ttu-id="e0f05-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0f05-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e0f05-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0f05-157">Response</span></span>

<span data-ttu-id="e0f05-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e0f05-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e0f05-159">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="e0f05-159">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e0f05-160">Basic</span><span class="sxs-lookup"><span data-stu-id="e0f05-160">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityminutecounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0f05-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0f05-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityminutecounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="e0f05-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="e0f05-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="e0f05-163">JSON</span><span class="sxs-lookup"><span data-stu-id="e0f05-163">JSON</span></span>

<span data-ttu-id="e0f05-164">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="e0f05-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e0f05-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0f05-165">Request</span></span>

<span data-ttu-id="e0f05-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0f05-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e0f05-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0f05-167">Response</span></span>

<span data-ttu-id="e0f05-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e0f05-168">The following is an example of the response.</span></span>

> <span data-ttu-id="e0f05-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0f05-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e0f05-171">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="e0f05-171">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e0f05-172">Basic</span><span class="sxs-lookup"><span data-stu-id="e0f05-172">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityminutecounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0f05-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0f05-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityminutecounts_json-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
