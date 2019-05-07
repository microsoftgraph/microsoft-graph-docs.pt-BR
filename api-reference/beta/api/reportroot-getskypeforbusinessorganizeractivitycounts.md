---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityCounts'
description: Obtenha tendências de uso do número e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização. Os tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, Web, dial-in/out por terceiros, dial-in/out pela Microsoft.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0194df11740111d93c27929ccaecc550bbbc47c8
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639205"
---
# <a name="reportroot-getskypeforbusinessorganizeractivitycounts"></a><span data-ttu-id="ba7fc-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="ba7fc-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba7fc-105">Obtenha tendências de uso do número e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-105">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="ba7fc-106">Os tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, Web, dial-in/out por terceiros, dial-in/out pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span>

> <span data-ttu-id="ba7fc-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do organizador da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="ba7fc-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="ba7fc-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba7fc-108">Permissions</span></span>

<span data-ttu-id="ba7fc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba7fc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba7fc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba7fc-111">Permission type</span></span>                        | <span data-ttu-id="ba7fc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba7fc-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ba7fc-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba7fc-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba7fc-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba7fc-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ba7fc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba7fc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba7fc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-116">Not supported.</span></span>                           |
| <span data-ttu-id="ba7fc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba7fc-117">Application</span></span>                            | <span data-ttu-id="ba7fc-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba7fc-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ba7fc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba7fc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ba7fc-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="ba7fc-120">Function parameters</span></span>

<span data-ttu-id="ba7fc-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ba7fc-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ba7fc-122">Parameter</span></span> | <span data-ttu-id="ba7fc-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba7fc-123">Type</span></span>   | <span data-ttu-id="ba7fc-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba7fc-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ba7fc-125">ponto</span><span class="sxs-lookup"><span data-stu-id="ba7fc-125">period</span></span>    | <span data-ttu-id="ba7fc-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba7fc-126">string</span></span> | <span data-ttu-id="ba7fc-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ba7fc-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ba7fc-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ba7fc-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-130">Required.</span></span> |

<span data-ttu-id="ba7fc-131">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ba7fc-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-132">The default output type is text/csv.</span></span> <span data-ttu-id="ba7fc-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba7fc-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba7fc-134">Request headers</span></span>

| <span data-ttu-id="ba7fc-135">Nome</span><span class="sxs-lookup"><span data-stu-id="ba7fc-135">Name</span></span>          | <span data-ttu-id="ba7fc-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba7fc-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ba7fc-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba7fc-137">Authorization</span></span> | <span data-ttu-id="ba7fc-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ba7fc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba7fc-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ba7fc-141">CSV</span><span class="sxs-lookup"><span data-stu-id="ba7fc-141">CSV</span></span>

<span data-ttu-id="ba7fc-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ba7fc-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ba7fc-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ba7fc-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ba7fc-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="ba7fc-146">Report Refresh Date</span></span>
- <span data-ttu-id="ba7fc-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="ba7fc-147">Report Date</span></span>
- <span data-ttu-id="ba7fc-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="ba7fc-148">Report Period</span></span>
- <span data-ttu-id="ba7fc-149">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="ba7fc-149">IM</span></span>
- <span data-ttu-id="ba7fc-150">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="ba7fc-150">Audio/Video</span></span>
- <span data-ttu-id="ba7fc-151">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="ba7fc-151">App Sharing</span></span>
- <span data-ttu-id="ba7fc-152">Web</span><span class="sxs-lookup"><span data-stu-id="ba7fc-152">Web</span></span>
- <span data-ttu-id="ba7fc-153">Dial-in/out por terceiros</span><span class="sxs-lookup"><span data-stu-id="ba7fc-153">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="ba7fc-154">Dial-in/out pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="ba7fc-154">Dial-in/out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="ba7fc-155">JSON</span><span class="sxs-lookup"><span data-stu-id="ba7fc-155">JSON</span></span>

<span data-ttu-id="ba7fc-156">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba7fc-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba7fc-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ba7fc-158">CSV</span><span class="sxs-lookup"><span data-stu-id="ba7fc-158">CSV</span></span>

<span data-ttu-id="ba7fc-159">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ba7fc-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba7fc-160">Request</span></span>

<span data-ttu-id="ba7fc-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="ba7fc-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba7fc-162">Response</span></span>

<span data-ttu-id="ba7fc-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ba7fc-164">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="ba7fc-164">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ba7fc-165">Basic</span><span class="sxs-lookup"><span data-stu-id="ba7fc-165">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivitycounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ba7fc-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba7fc-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivitycounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="ba7fc-167">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
```

### <a name="json"></a><span data-ttu-id="ba7fc-168">JSON</span><span class="sxs-lookup"><span data-stu-id="ba7fc-168">JSON</span></span>

<span data-ttu-id="ba7fc-169">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ba7fc-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba7fc-170">Request</span></span>

<span data-ttu-id="ba7fc-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="ba7fc-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba7fc-172">Response</span></span>

<span data-ttu-id="ba7fc-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-173">The following is an example of the response.</span></span>

> <span data-ttu-id="ba7fc-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba7fc-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 315

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessOrganizerActivityCounts)", 
  "value": [
    {
      "im": 20, 
      "audioVideo": 43, 
      "appSharing": 20, 
      "web": 6, 
      "dialInOut3rdParty": 0, 
      "dialInOutMicrosoft": 48, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ba7fc-176">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="ba7fc-176">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ba7fc-177">Basic</span><span class="sxs-lookup"><span data-stu-id="ba7fc-177">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivitycounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ba7fc-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba7fc-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivitycounts_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessorganizeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
