---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Obtenha dados sobre a atividade do Skype for Business por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 93236b646f841f6e6a8d4f2a06e2780ac964460e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267232"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="bab84-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="bab84-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bab84-104">Obtenha dados sobre a atividade do Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="bab84-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="bab84-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="bab84-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="bab84-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bab84-106">Permissions</span></span>

<span data-ttu-id="bab84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bab84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bab84-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bab84-109">Permission type</span></span>                        | <span data-ttu-id="bab84-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bab84-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bab84-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bab84-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bab84-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bab84-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bab84-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bab84-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bab84-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bab84-114">Not supported.</span></span>                           |
| <span data-ttu-id="bab84-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bab84-115">Application</span></span>                            | <span data-ttu-id="bab84-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bab84-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bab84-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bab84-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="bab84-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="bab84-118">Function parameters</span></span>

<span data-ttu-id="bab84-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="bab84-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="bab84-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bab84-120">Parameter</span></span> | <span data-ttu-id="bab84-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="bab84-121">Type</span></span>   | <span data-ttu-id="bab84-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bab84-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bab84-123">ponto</span><span class="sxs-lookup"><span data-stu-id="bab84-123">period</span></span>    | <span data-ttu-id="bab84-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bab84-124">string</span></span> | <span data-ttu-id="bab84-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bab84-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bab84-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="bab84-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bab84-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bab84-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="bab84-128">data</span><span class="sxs-lookup"><span data-stu-id="bab84-128">date</span></span>      | <span data-ttu-id="bab84-129">Data</span><span class="sxs-lookup"><span data-stu-id="bab84-129">Date</span></span>   | <span data-ttu-id="bab84-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="bab84-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="bab84-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="bab84-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="bab84-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="bab84-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="bab84-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="bab84-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="bab84-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="bab84-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="bab84-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="bab84-135">The default output type is text/csv.</span></span> <span data-ttu-id="bab84-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="bab84-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bab84-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bab84-137">Request headers</span></span>

| <span data-ttu-id="bab84-138">Nome</span><span class="sxs-lookup"><span data-stu-id="bab84-138">Name</span></span>          | <span data-ttu-id="bab84-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="bab84-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="bab84-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="bab84-140">Authorization</span></span> | <span data-ttu-id="bab84-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bab84-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bab84-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="bab84-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="bab84-144">CSV</span><span class="sxs-lookup"><span data-stu-id="bab84-144">CSV</span></span>

<span data-ttu-id="bab84-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="bab84-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bab84-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="bab84-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bab84-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="bab84-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bab84-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="bab84-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bab84-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="bab84-149">Report Refresh Date</span></span>
- <span data-ttu-id="bab84-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="bab84-150">User Principal Name</span></span>
- <span data-ttu-id="bab84-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="bab84-151">Is Deleted</span></span>
- <span data-ttu-id="bab84-152">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="bab84-152">Deleted Date</span></span>
- <span data-ttu-id="bab84-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="bab84-153">Last Activity Date</span></span>
- <span data-ttu-id="bab84-154">Contagem total de sessão de ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="bab84-154">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="bab84-155">Contagem total de conferência organizada</span><span class="sxs-lookup"><span data-stu-id="bab84-155">Total Organized Conference Count</span></span>
- <span data-ttu-id="bab84-156">Contagem total de conferência participada</span><span class="sxs-lookup"><span data-stu-id="bab84-156">Total Participated Conference Count</span></span>
- <span data-ttu-id="bab84-157">Data da última atividade ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="bab84-157">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="bab84-158">Data da última atividade da conferência organizada</span><span class="sxs-lookup"><span data-stu-id="bab84-158">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="bab84-159">Data da última atividade da conferência participada</span><span class="sxs-lookup"><span data-stu-id="bab84-159">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="bab84-160">Contagem de mensagens instantâneas ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="bab84-160">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="bab84-161">Contagem de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="bab84-161">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="bab84-162">Minutos de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="bab84-162">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="bab84-163">Contagem de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="bab84-163">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="bab84-164">Minutos de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="bab84-164">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="bab84-165">Contagem de compartilhamentos de aplicativos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="bab84-165">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="bab84-166">Contagem de transferências de arquivos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="bab84-166">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="bab84-167">Contagem de mensagens instantâneas em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="bab84-167">Organized Conference IM Count</span></span>
- <span data-ttu-id="bab84-168">Contagem de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="bab84-168">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="bab84-169">Minutos de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="bab84-169">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="bab84-170">Contagem de compartilhamentos de aplicativos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="bab84-170">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="bab84-171">Contagem de Web em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="bab84-171">Organized Conference Web Count</span></span>
- <span data-ttu-id="bab84-172">Contagem de chamadas dial-in/out por terceiros em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="bab84-172">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="bab84-173">Contagem de chamadas dial-in/out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="bab84-173">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="bab84-174">Minutos de chamadas dial-in pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="bab84-174">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="bab84-175">Minutos de chamadas dial-out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="bab84-175">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="bab84-176">Contagem de IM de conferência participada</span><span class="sxs-lookup"><span data-stu-id="bab84-176">Participated Conference IM Count</span></span>
- <span data-ttu-id="bab84-177">Contagem de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="bab84-177">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="bab84-178">Minutos de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="bab84-178">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="bab84-179">Contagem de compartilhamentos de aplicativos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="bab84-179">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="bab84-180">Contagem de Web em conferência participada</span><span class="sxs-lookup"><span data-stu-id="bab84-180">Participated Conference Web Count</span></span>
- <span data-ttu-id="bab84-181">Contagem de chamadas dial-in/out por terceiros em conferência participada</span><span class="sxs-lookup"><span data-stu-id="bab84-181">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="bab84-182">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="bab84-182">Assigned Products</span></span>
- <span data-ttu-id="bab84-183">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="bab84-183">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="bab84-184">JSON</span><span class="sxs-lookup"><span data-stu-id="bab84-184">JSON</span></span>

<span data-ttu-id="bab84-185">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bab84-185">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="bab84-186">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="bab84-186">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="bab84-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bab84-187">Example</span></span>

### <a name="csv"></a><span data-ttu-id="bab84-188">CSV</span><span class="sxs-lookup"><span data-stu-id="bab84-188">CSV</span></span>

<span data-ttu-id="bab84-189">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="bab84-189">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="bab84-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bab84-190">Request</span></span>

<span data-ttu-id="bab84-191">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bab84-191">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="bab84-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="bab84-192">Response</span></span>

<span data-ttu-id="bab84-193">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bab84-193">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bab84-194">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="bab84-194">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bab84-195">C#</span><span class="sxs-lookup"><span data-stu-id="bab84-195">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessactivityuserdetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bab84-196">Javascript</span><span class="sxs-lookup"><span data-stu-id="bab84-196">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessactivityuserdetail_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bab84-197">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bab84-197">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessactivityuserdetail_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="bab84-198">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="bab84-198">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Total Peer-to-peer Session Count,Total Organized Conference Count,Total Participated Conference Count,Peer-to-peer Last Activity Date,Organized Conference Last Activity Date,Participated Conference Last Activity Date,Peer-to-peer IM Count,Peer-to-peer Audio Count,Peer-to-peer Audio Minutes,Peer-to-peer Video Count,Peer-to-peer Video Minutes,Peer-to-peer App Sharing Count,Peer-to-peer File Transfer Count,Organized Conference IM Count,Organized Conference Audio/Video Count,Organized Conference Audio/Video Minutes,Organized Conference App Sharing Count,Organized Conference Web Count,Organized Conference Dial-in/out 3rd Party Count,Organized Conference Dial-in/out Microsoft Count,Organized Conference Dial-in Microsoft Minutes,Organized Conference Dial-out Microsoft Minutes,Participated Conference IM Count,Participated Conference Audio/Video Count,Participated Conference Audio/Video Minutes,Participated Conference App Sharing Count,Participated Conference Web Count,Participated Conference Dial-in/out 3rd Party Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="bab84-199">JSON</span><span class="sxs-lookup"><span data-stu-id="bab84-199">JSON</span></span>

<span data-ttu-id="bab84-200">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="bab84-200">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="bab84-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bab84-201">Request</span></span>

<span data-ttu-id="bab84-202">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bab84-202">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="bab84-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="bab84-203">Response</span></span>

<span data-ttu-id="bab84-204">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bab84-204">The following is an example of the response.</span></span>

> <span data-ttu-id="bab84-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bab84-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1419

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessActivityUserDetail)", 
  "value": [
    {
      "totalPeerToPeerSessionCount": 12, 
      "totalOrganizedConferenceCount": 0, 
      "totalParticipatedConferenceCount": 1, 
      "peerToPeerLastActivityDate": "2017-09-01", 
      "organizedConferenceLastActivityDate": null, 
      "participatedConferenceLastActivityDate": "2017-08-31", 
      "peerToPeerIMCount": 12, 
      "peerToPeerAudioCount": 0, 
      "peerToPeerAudioMinutes": 0, 
      "peerToPeerVideoCount": 0, 
      "peerToPeerVideoMinutes": 0, 
      "peerToPeerAppSharingCount": 0, 
      "peerToPeerFileTransferCount": 0, 
      "organizedConferenceIMCount": 0, 
      "organizedConferenceAudioVideoCount": 0, 
      "organizedConferenceAudioVideoMinutes": 0, 
      "organizedConferenceAppSharingCount": 0, 
      "organizedConferenceWebCount": 0, 
      "organizedConferenceDialInOut3rdPartyCount": 0, 
      "organizedConferenceCloudDialInOutMicrosoftCount": 0, 
      "organizedConferenceCloudDialInMicrosoftMinutes": 0, 
      "organizedConferenceCloudDialOutMicrosoftMinutes": 0, 
      "participatedConferenceIMCount": 0, 
      "participatedConferenceAudioVideoCount": 1, 
      "participatedConferenceAudioVideoMinutes": 69, 
      "participatedConferenceAppSharingCount": 0, 
      "participatedConferenceWebCount": 0, 
      "participatedConferenceDialInOut3rdPartyCount": 0, 
      "reportRefreshDate": "2017-09-06", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5", 
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bab84-207">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="bab84-207">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bab84-208">C#</span><span class="sxs-lookup"><span data-stu-id="bab84-208">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessactivityuserdetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bab84-209">Javascript</span><span class="sxs-lookup"><span data-stu-id="bab84-209">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessactivityuserdetail_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bab84-210">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bab84-210">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessactivityuserdetail_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
