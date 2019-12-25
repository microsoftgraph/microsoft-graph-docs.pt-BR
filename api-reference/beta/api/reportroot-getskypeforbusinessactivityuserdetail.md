---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Obtenha dados sobre a atividade do Skype for Business por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 62593b6698ec71b447df839dc4213704af3b639d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869007"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="71ac9-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="71ac9-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71ac9-104">Obtenha dados sobre a atividade do Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="71ac9-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="71ac9-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="71ac9-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="71ac9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="71ac9-106">Permissions</span></span>

<span data-ttu-id="71ac9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71ac9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71ac9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71ac9-109">Permission type</span></span>                        | <span data-ttu-id="71ac9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71ac9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="71ac9-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71ac9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="71ac9-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="71ac9-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="71ac9-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71ac9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71ac9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71ac9-114">Not supported.</span></span>                           |
| <span data-ttu-id="71ac9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71ac9-115">Application</span></span>                            | <span data-ttu-id="71ac9-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="71ac9-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="71ac9-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="71ac9-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="71ac9-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="71ac9-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="71ac9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71ac9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="71ac9-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="71ac9-120">Function parameters</span></span>

<span data-ttu-id="71ac9-121">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="71ac9-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="71ac9-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="71ac9-122">Parameter</span></span> | <span data-ttu-id="71ac9-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="71ac9-123">Type</span></span>   | <span data-ttu-id="71ac9-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="71ac9-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="71ac9-125">ponto</span><span class="sxs-lookup"><span data-stu-id="71ac9-125">period</span></span>    | <span data-ttu-id="71ac9-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71ac9-126">string</span></span> | <span data-ttu-id="71ac9-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="71ac9-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="71ac9-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="71ac9-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="71ac9-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="71ac9-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="71ac9-130">data</span><span class="sxs-lookup"><span data-stu-id="71ac9-130">date</span></span>      | <span data-ttu-id="71ac9-131">Data</span><span class="sxs-lookup"><span data-stu-id="71ac9-131">Date</span></span>   | <span data-ttu-id="71ac9-132">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="71ac9-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="71ac9-133">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="71ac9-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="71ac9-134">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="71ac9-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="71ac9-135">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="71ac9-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="71ac9-136">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="71ac9-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="71ac9-137">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="71ac9-137">The default output type is text/csv.</span></span> <span data-ttu-id="71ac9-138">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="71ac9-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71ac9-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71ac9-139">Request headers</span></span>

| <span data-ttu-id="71ac9-140">Nome</span><span class="sxs-lookup"><span data-stu-id="71ac9-140">Name</span></span>          | <span data-ttu-id="71ac9-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="71ac9-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="71ac9-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="71ac9-142">Authorization</span></span> | <span data-ttu-id="71ac9-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71ac9-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="71ac9-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="71ac9-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="71ac9-146">CSV</span><span class="sxs-lookup"><span data-stu-id="71ac9-146">CSV</span></span>

<span data-ttu-id="71ac9-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="71ac9-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="71ac9-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="71ac9-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="71ac9-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="71ac9-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="71ac9-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="71ac9-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="71ac9-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="71ac9-151">Report Refresh Date</span></span>
- <span data-ttu-id="71ac9-152">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="71ac9-152">User Principal Name</span></span>
- <span data-ttu-id="71ac9-153">Excluído</span><span class="sxs-lookup"><span data-stu-id="71ac9-153">Is Deleted</span></span>
- <span data-ttu-id="71ac9-154">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="71ac9-154">Deleted Date</span></span>
- <span data-ttu-id="71ac9-155">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="71ac9-155">Last Activity Date</span></span>
- <span data-ttu-id="71ac9-156">Contagem total de sessão de ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="71ac9-156">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="71ac9-157">Contagem total de conferência organizada</span><span class="sxs-lookup"><span data-stu-id="71ac9-157">Total Organized Conference Count</span></span>
- <span data-ttu-id="71ac9-158">Contagem total de conferência participada</span><span class="sxs-lookup"><span data-stu-id="71ac9-158">Total Participated Conference Count</span></span>
- <span data-ttu-id="71ac9-159">Data da última atividade ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="71ac9-159">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="71ac9-160">Data da última atividade da conferência organizada</span><span class="sxs-lookup"><span data-stu-id="71ac9-160">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="71ac9-161">Data da última atividade da conferência participada</span><span class="sxs-lookup"><span data-stu-id="71ac9-161">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="71ac9-162">Contagem de mensagens instantâneas ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="71ac9-162">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="71ac9-163">Contagem de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="71ac9-163">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="71ac9-164">Minutos de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="71ac9-164">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="71ac9-165">Contagem de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="71ac9-165">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="71ac9-166">Minutos de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="71ac9-166">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="71ac9-167">Contagem de compartilhamentos de aplicativos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="71ac9-167">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="71ac9-168">Contagem de transferências de arquivos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="71ac9-168">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="71ac9-169">Contagem de mensagens instantâneas em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="71ac9-169">Organized Conference IM Count</span></span>
- <span data-ttu-id="71ac9-170">Contagem de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="71ac9-170">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="71ac9-171">Minutos de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="71ac9-171">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="71ac9-172">Contagem de compartilhamentos de aplicativos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="71ac9-172">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="71ac9-173">Contagem de Web em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="71ac9-173">Organized Conference Web Count</span></span>
- <span data-ttu-id="71ac9-174">Contagem de chamadas dial-in/out por terceiros em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="71ac9-174">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="71ac9-175">Contagem de chamadas dial-in/out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="71ac9-175">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="71ac9-176">Minutos de chamadas dial-in pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="71ac9-176">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="71ac9-177">Minutos de chamadas dial-out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="71ac9-177">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="71ac9-178">Contagem de IM de conferência participada</span><span class="sxs-lookup"><span data-stu-id="71ac9-178">Participated Conference IM Count</span></span>
- <span data-ttu-id="71ac9-179">Contagem de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="71ac9-179">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="71ac9-180">Minutos de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="71ac9-180">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="71ac9-181">Contagem de compartilhamentos de aplicativos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="71ac9-181">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="71ac9-182">Contagem de Web em conferência participada</span><span class="sxs-lookup"><span data-stu-id="71ac9-182">Participated Conference Web Count</span></span>
- <span data-ttu-id="71ac9-183">Contagem de chamadas dial-in/out por terceiros em conferência participada</span><span class="sxs-lookup"><span data-stu-id="71ac9-183">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="71ac9-184">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="71ac9-184">Assigned Products</span></span>
- <span data-ttu-id="71ac9-185">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="71ac9-185">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="71ac9-186">JSON</span><span class="sxs-lookup"><span data-stu-id="71ac9-186">JSON</span></span>

<span data-ttu-id="71ac9-187">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71ac9-187">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="71ac9-188">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="71ac9-188">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="71ac9-189">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71ac9-189">Example</span></span>

### <a name="csv"></a><span data-ttu-id="71ac9-190">CSV</span><span class="sxs-lookup"><span data-stu-id="71ac9-190">CSV</span></span>

<span data-ttu-id="71ac9-191">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="71ac9-191">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="71ac9-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71ac9-192">Request</span></span>

<span data-ttu-id="71ac9-193">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="71ac9-193">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="71ac9-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="71ac9-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="71ac9-195">C#</span><span class="sxs-lookup"><span data-stu-id="71ac9-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71ac9-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71ac9-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="71ac9-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71ac9-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="71ac9-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="71ac9-198">Response</span></span>

<span data-ttu-id="71ac9-199">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="71ac9-199">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="71ac9-200">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="71ac9-200">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="71ac9-201">JSON</span><span class="sxs-lookup"><span data-stu-id="71ac9-201">JSON</span></span>

<span data-ttu-id="71ac9-202">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="71ac9-202">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="71ac9-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71ac9-203">Request</span></span>

<span data-ttu-id="71ac9-204">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="71ac9-204">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="71ac9-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="71ac9-205">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="71ac9-206">C#</span><span class="sxs-lookup"><span data-stu-id="71ac9-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71ac9-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71ac9-207">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="71ac9-208">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71ac9-208">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="71ac9-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="71ac9-209">Response</span></span>

<span data-ttu-id="71ac9-210">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="71ac9-210">The following is an example of the response.</span></span>

> <span data-ttu-id="71ac9-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71ac9-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
