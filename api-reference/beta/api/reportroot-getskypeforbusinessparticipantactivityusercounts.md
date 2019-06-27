---
title: 'reportRoot: getSkypeForBusinessParticipantActivityUserCounts'
description: Obtenha tendências de uso do número de usuários únicos e o tipo de sessões de conferência das quais os usuários de sua organização participaram. Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: ebcc0285558099d46708c70feec1252b3f2e6494
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265174"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityusercounts"></a><span data-ttu-id="8f94a-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="8f94a-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f94a-105">Obtenha tendências de uso do número de usuários únicos e o tipo de sessões de conferência das quais os usuários de sua organização participaram.</span><span class="sxs-lookup"><span data-stu-id="8f94a-105">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="8f94a-106">Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros.</span><span class="sxs-lookup"><span data-stu-id="8f94a-106">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="8f94a-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do participante da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="8f94a-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="8f94a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f94a-108">Permissions</span></span>

<span data-ttu-id="8f94a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f94a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f94a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f94a-111">Permission type</span></span>                        | <span data-ttu-id="8f94a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f94a-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8f94a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f94a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f94a-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f94a-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8f94a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f94a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f94a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f94a-116">Not supported.</span></span>                           |
| <span data-ttu-id="8f94a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f94a-117">Application</span></span>                            | <span data-ttu-id="8f94a-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f94a-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8f94a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f94a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8f94a-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="8f94a-120">Function parameters</span></span>

<span data-ttu-id="8f94a-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="8f94a-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8f94a-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8f94a-122">Parameter</span></span> | <span data-ttu-id="8f94a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f94a-123">Type</span></span>   | <span data-ttu-id="8f94a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f94a-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8f94a-125">ponto</span><span class="sxs-lookup"><span data-stu-id="8f94a-125">period</span></span>    | <span data-ttu-id="8f94a-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f94a-126">string</span></span> | <span data-ttu-id="8f94a-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="8f94a-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8f94a-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="8f94a-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8f94a-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="8f94a-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8f94a-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f94a-130">Required.</span></span> |

<span data-ttu-id="8f94a-131">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8f94a-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8f94a-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="8f94a-132">The default output type is text/csv.</span></span> <span data-ttu-id="8f94a-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="8f94a-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f94a-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f94a-134">Request headers</span></span>

| <span data-ttu-id="8f94a-135">Nome</span><span class="sxs-lookup"><span data-stu-id="8f94a-135">Name</span></span>          | <span data-ttu-id="8f94a-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f94a-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8f94a-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f94a-137">Authorization</span></span> | <span data-ttu-id="8f94a-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8f94a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f94a-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8f94a-141">CSV</span><span class="sxs-lookup"><span data-stu-id="8f94a-141">CSV</span></span>

<span data-ttu-id="8f94a-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="8f94a-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8f94a-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="8f94a-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8f94a-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8f94a-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8f94a-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="8f94a-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8f94a-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="8f94a-146">Report Refresh Date</span></span>
- <span data-ttu-id="8f94a-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="8f94a-147">Report Date</span></span>
- <span data-ttu-id="8f94a-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="8f94a-148">Report Period</span></span>
- <span data-ttu-id="8f94a-149">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="8f94a-149">IM</span></span>
- <span data-ttu-id="8f94a-150">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="8f94a-150">Audio/Video</span></span>
- <span data-ttu-id="8f94a-151">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="8f94a-151">App Sharing</span></span>
- <span data-ttu-id="8f94a-152">Web</span><span class="sxs-lookup"><span data-stu-id="8f94a-152">Web</span></span>
- <span data-ttu-id="8f94a-153">Dial-in/out por terceiros</span><span class="sxs-lookup"><span data-stu-id="8f94a-153">Dial-in/out 3rd Party</span></span>

### <a name="json"></a><span data-ttu-id="8f94a-154">JSON</span><span class="sxs-lookup"><span data-stu-id="8f94a-154">JSON</span></span>

<span data-ttu-id="8f94a-155">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f94a-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f94a-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f94a-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8f94a-157">CSV</span><span class="sxs-lookup"><span data-stu-id="8f94a-157">CSV</span></span>

<span data-ttu-id="8f94a-158">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="8f94a-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8f94a-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f94a-159">Request</span></span>

<span data-ttu-id="8f94a-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f94a-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="8f94a-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f94a-161">Response</span></span>

<span data-ttu-id="8f94a-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8f94a-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8f94a-163">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="8f94a-163">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8f94a-164">C#</span><span class="sxs-lookup"><span data-stu-id="8f94a-164">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityusercounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f94a-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="8f94a-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityusercounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8f94a-166">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8f94a-166">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityusercounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="8f94a-167">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="8f94a-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
```

### <a name="json"></a><span data-ttu-id="8f94a-168">JSON</span><span class="sxs-lookup"><span data-stu-id="8f94a-168">JSON</span></span>

<span data-ttu-id="8f94a-169">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="8f94a-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8f94a-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f94a-170">Request</span></span>

<span data-ttu-id="8f94a-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f94a-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="8f94a-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f94a-172">Response</span></span>

<span data-ttu-id="8f94a-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8f94a-173">The following is an example of the response.</span></span>

> <span data-ttu-id="8f94a-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 301

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityUserCounts)", 
  "value": [
    {
      "im": 137, 
      "audioVideo": 196, 
      "appSharing": 214, 
      "web": 30, 
      "dialInOut3rdParty": 2, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8f94a-176">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="8f94a-176">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8f94a-177">C#</span><span class="sxs-lookup"><span data-stu-id="8f94a-177">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f94a-178">Javascript</span><span class="sxs-lookup"><span data-stu-id="8f94a-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityusercounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8f94a-179">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8f94a-179">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessparticipantactivityusercounts_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessparticipantactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
