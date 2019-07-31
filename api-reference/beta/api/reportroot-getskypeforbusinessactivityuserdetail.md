---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Obtenha dados sobre a atividade do Skype for Business por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 4c3eebedc28c0866cedf40624bb137ac8f232a89
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35988066"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="19b64-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="19b64-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19b64-104">Obtenha dados sobre a atividade do Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="19b64-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="19b64-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="19b64-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="19b64-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="19b64-106">Permissions</span></span>

<span data-ttu-id="19b64-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19b64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19b64-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19b64-109">Permission type</span></span>                        | <span data-ttu-id="19b64-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19b64-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="19b64-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19b64-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="19b64-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="19b64-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="19b64-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19b64-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19b64-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19b64-114">Not supported.</span></span>                           |
| <span data-ttu-id="19b64-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19b64-115">Application</span></span>                            | <span data-ttu-id="19b64-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="19b64-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="19b64-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19b64-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="19b64-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="19b64-118">Function parameters</span></span>

<span data-ttu-id="19b64-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="19b64-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="19b64-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="19b64-120">Parameter</span></span> | <span data-ttu-id="19b64-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="19b64-121">Type</span></span>   | <span data-ttu-id="19b64-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="19b64-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="19b64-123">ponto</span><span class="sxs-lookup"><span data-stu-id="19b64-123">period</span></span>    | <span data-ttu-id="19b64-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19b64-124">string</span></span> | <span data-ttu-id="19b64-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="19b64-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="19b64-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="19b64-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="19b64-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="19b64-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="19b64-128">data</span><span class="sxs-lookup"><span data-stu-id="19b64-128">date</span></span>      | <span data-ttu-id="19b64-129">Data</span><span class="sxs-lookup"><span data-stu-id="19b64-129">Date</span></span>   | <span data-ttu-id="19b64-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="19b64-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="19b64-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="19b64-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="19b64-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="19b64-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="19b64-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="19b64-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="19b64-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="19b64-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="19b64-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="19b64-135">The default output type is text/csv.</span></span> <span data-ttu-id="19b64-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="19b64-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19b64-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19b64-137">Request headers</span></span>

| <span data-ttu-id="19b64-138">Nome</span><span class="sxs-lookup"><span data-stu-id="19b64-138">Name</span></span>          | <span data-ttu-id="19b64-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="19b64-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="19b64-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="19b64-140">Authorization</span></span> | <span data-ttu-id="19b64-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19b64-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="19b64-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="19b64-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="19b64-144">CSV</span><span class="sxs-lookup"><span data-stu-id="19b64-144">CSV</span></span>

<span data-ttu-id="19b64-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="19b64-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="19b64-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="19b64-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="19b64-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="19b64-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="19b64-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="19b64-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="19b64-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="19b64-149">Report Refresh Date</span></span>
- <span data-ttu-id="19b64-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="19b64-150">User Principal Name</span></span>
- <span data-ttu-id="19b64-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="19b64-151">Is Deleted</span></span>
- <span data-ttu-id="19b64-152">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="19b64-152">Deleted Date</span></span>
- <span data-ttu-id="19b64-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="19b64-153">Last Activity Date</span></span>
- <span data-ttu-id="19b64-154">Contagem total de sessão de ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="19b64-154">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="19b64-155">Contagem total de conferência organizada</span><span class="sxs-lookup"><span data-stu-id="19b64-155">Total Organized Conference Count</span></span>
- <span data-ttu-id="19b64-156">Contagem total de conferência participada</span><span class="sxs-lookup"><span data-stu-id="19b64-156">Total Participated Conference Count</span></span>
- <span data-ttu-id="19b64-157">Data da última atividade ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="19b64-157">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="19b64-158">Data da última atividade da conferência organizada</span><span class="sxs-lookup"><span data-stu-id="19b64-158">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="19b64-159">Data da última atividade da conferência participada</span><span class="sxs-lookup"><span data-stu-id="19b64-159">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="19b64-160">Contagem de mensagens instantâneas ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="19b64-160">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="19b64-161">Contagem de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="19b64-161">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="19b64-162">Minutos de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="19b64-162">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="19b64-163">Contagem de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="19b64-163">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="19b64-164">Minutos de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="19b64-164">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="19b64-165">Contagem de compartilhamentos de aplicativos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="19b64-165">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="19b64-166">Contagem de transferências de arquivos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="19b64-166">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="19b64-167">Contagem de mensagens instantâneas em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="19b64-167">Organized Conference IM Count</span></span>
- <span data-ttu-id="19b64-168">Contagem de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="19b64-168">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="19b64-169">Minutos de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="19b64-169">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="19b64-170">Contagem de compartilhamentos de aplicativos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="19b64-170">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="19b64-171">Contagem de Web em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="19b64-171">Organized Conference Web Count</span></span>
- <span data-ttu-id="19b64-172">Contagem de chamadas dial-in/out por terceiros em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="19b64-172">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="19b64-173">Contagem de chamadas dial-in/out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="19b64-173">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="19b64-174">Minutos de chamadas dial-in pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="19b64-174">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="19b64-175">Minutos de chamadas dial-out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="19b64-175">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="19b64-176">Contagem de IM de conferência participada</span><span class="sxs-lookup"><span data-stu-id="19b64-176">Participated Conference IM Count</span></span>
- <span data-ttu-id="19b64-177">Contagem de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="19b64-177">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="19b64-178">Minutos de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="19b64-178">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="19b64-179">Contagem de compartilhamentos de aplicativos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="19b64-179">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="19b64-180">Contagem de Web em conferência participada</span><span class="sxs-lookup"><span data-stu-id="19b64-180">Participated Conference Web Count</span></span>
- <span data-ttu-id="19b64-181">Contagem de chamadas dial-in/out por terceiros em conferência participada</span><span class="sxs-lookup"><span data-stu-id="19b64-181">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="19b64-182">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="19b64-182">Assigned Products</span></span>
- <span data-ttu-id="19b64-183">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="19b64-183">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="19b64-184">JSON</span><span class="sxs-lookup"><span data-stu-id="19b64-184">JSON</span></span>

<span data-ttu-id="19b64-185">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19b64-185">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="19b64-186">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="19b64-186">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="19b64-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19b64-187">Example</span></span>

### <a name="csv"></a><span data-ttu-id="19b64-188">CSV</span><span class="sxs-lookup"><span data-stu-id="19b64-188">CSV</span></span>

<span data-ttu-id="19b64-189">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="19b64-189">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="19b64-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19b64-190">Request</span></span>

<span data-ttu-id="19b64-191">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="19b64-191">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="19b64-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="19b64-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="19b64-193">C#</span><span class="sxs-lookup"><span data-stu-id="19b64-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19b64-194">Javascript</span><span class="sxs-lookup"><span data-stu-id="19b64-194">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19b64-195">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="19b64-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="19b64-196">Java</span><span class="sxs-lookup"><span data-stu-id="19b64-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessactivityuserdetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="19b64-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="19b64-197">Response</span></span>

<span data-ttu-id="19b64-198">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="19b64-198">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="19b64-199">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="19b64-199">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="19b64-200">JSON</span><span class="sxs-lookup"><span data-stu-id="19b64-200">JSON</span></span>

<span data-ttu-id="19b64-201">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="19b64-201">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="19b64-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19b64-202">Request</span></span>

<span data-ttu-id="19b64-203">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="19b64-203">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="19b64-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="19b64-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="19b64-205">C#</span><span class="sxs-lookup"><span data-stu-id="19b64-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19b64-206">Javascript</span><span class="sxs-lookup"><span data-stu-id="19b64-206">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19b64-207">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="19b64-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="19b64-208">Java</span><span class="sxs-lookup"><span data-stu-id="19b64-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessactivityuserdetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="19b64-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="19b64-209">Response</span></span>

<span data-ttu-id="19b64-210">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="19b64-210">The following is an example of the response.</span></span>

> <span data-ttu-id="19b64-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19b64-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
