---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Obtenha dados sobre a atividade do Skype for Business por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 8ca56904638598085cb345acf5d93babc4226347
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865311"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="b06a6-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="b06a6-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="b06a6-104">Obtenha dados sobre a atividade do Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="b06a6-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="b06a6-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="b06a6-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="b06a6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b06a6-106">Permissions</span></span>

<span data-ttu-id="b06a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b06a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b06a6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b06a6-109">Permission type</span></span>                        | <span data-ttu-id="b06a6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b06a6-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b06a6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b06a6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b06a6-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b06a6-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b06a6-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b06a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b06a6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b06a6-114">Not supported.</span></span>                           |
| <span data-ttu-id="b06a6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b06a6-115">Application</span></span>                            | <span data-ttu-id="b06a6-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b06a6-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="b06a6-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="b06a6-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="b06a6-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="b06a6-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="b06a6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b06a6-119">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="b06a6-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b06a6-120">Function parameters</span></span>

<span data-ttu-id="b06a6-121">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b06a6-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b06a6-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b06a6-122">Parameter</span></span> | <span data-ttu-id="b06a6-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b06a6-123">Type</span></span>   | <span data-ttu-id="b06a6-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b06a6-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b06a6-125">ponto</span><span class="sxs-lookup"><span data-stu-id="b06a6-125">period</span></span>    | <span data-ttu-id="b06a6-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b06a6-126">string</span></span> | <span data-ttu-id="b06a6-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b06a6-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b06a6-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="b06a6-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b06a6-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b06a6-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b06a6-130">data</span><span class="sxs-lookup"><span data-stu-id="b06a6-130">date</span></span>      | <span data-ttu-id="b06a6-131">Data</span><span class="sxs-lookup"><span data-stu-id="b06a6-131">Date</span></span>   | <span data-ttu-id="b06a6-132">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="b06a6-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b06a6-133">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="b06a6-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b06a6-134">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="b06a6-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b06a6-135">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="b06a6-135">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b06a6-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b06a6-136">Request headers</span></span>

| <span data-ttu-id="b06a6-137">Nome</span><span class="sxs-lookup"><span data-stu-id="b06a6-137">Name</span></span>          | <span data-ttu-id="b06a6-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="b06a6-138">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b06a6-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="b06a6-139">Authorization</span></span> | <span data-ttu-id="b06a6-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b06a6-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b06a6-142">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b06a6-142">If-None-Match</span></span> | <span data-ttu-id="b06a6-143">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="b06a6-143">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b06a6-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b06a6-144">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b06a6-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b06a6-145">Response</span></span>

<span data-ttu-id="b06a6-146">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="b06a6-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b06a6-147">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="b06a6-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b06a6-148">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b06a6-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b06a6-149">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="b06a6-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b06a6-150">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="b06a6-150">Report Refresh Date</span></span>
- <span data-ttu-id="b06a6-151">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="b06a6-151">User Principal Name</span></span>
- <span data-ttu-id="b06a6-152">Excluído</span><span class="sxs-lookup"><span data-stu-id="b06a6-152">Is Deleted</span></span>
- <span data-ttu-id="b06a6-153">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="b06a6-153">Deleted Date</span></span>
- <span data-ttu-id="b06a6-154">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="b06a6-154">Last Activity Date</span></span>
- <span data-ttu-id="b06a6-155">Contagem total de sessão de ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="b06a6-155">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="b06a6-156">Contagem total de conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b06a6-156">Total Organized Conference Count</span></span>
- <span data-ttu-id="b06a6-157">Contagem total de conferência participada</span><span class="sxs-lookup"><span data-stu-id="b06a6-157">Total Participated Conference Count</span></span>
- <span data-ttu-id="b06a6-158">Data da última atividade ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="b06a6-158">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="b06a6-159">Data da última atividade da conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b06a6-159">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="b06a6-160">Data da última atividade da conferência participada</span><span class="sxs-lookup"><span data-stu-id="b06a6-160">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="b06a6-161">Contagem de mensagens instantâneas ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="b06a6-161">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="b06a6-162">Contagem de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="b06a6-162">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="b06a6-163">Minutos de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="b06a6-163">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="b06a6-164">Contagem de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="b06a6-164">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="b06a6-165">Minutos de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="b06a6-165">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="b06a6-166">Contagem de compartilhamentos de aplicativos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="b06a6-166">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="b06a6-167">Contagem de transferências de arquivos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="b06a6-167">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="b06a6-168">Contagem de mensagens instantâneas em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b06a6-168">Organized Conference IM Count</span></span>
- <span data-ttu-id="b06a6-169">Contagem de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b06a6-169">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="b06a6-170">Minutos de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b06a6-170">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="b06a6-171">Contagem de compartilhamentos de aplicativos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b06a6-171">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="b06a6-172">Contagem de Web em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b06a6-172">Organized Conference Web Count</span></span>
- <span data-ttu-id="b06a6-173">Contagem de chamadas dial-in/out por terceiros em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b06a6-173">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="b06a6-174">Contagem de chamadas dial-in/out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b06a6-174">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="b06a6-175">Minutos de chamadas dial-in pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b06a6-175">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="b06a6-176">Minutos de chamadas dial-out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b06a6-176">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="b06a6-177">Contagem de mensagens instantâneas em conferência participada</span><span class="sxs-lookup"><span data-stu-id="b06a6-177">Paricipated Conference IM Count</span></span>
- <span data-ttu-id="b06a6-178">Contagem de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="b06a6-178">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="b06a6-179">Minutos de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="b06a6-179">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="b06a6-180">Contagem de compartilhamentos de aplicativos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="b06a6-180">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="b06a6-181">Contagem de Web em conferência participada</span><span class="sxs-lookup"><span data-stu-id="b06a6-181">Participated Conference Web Count</span></span>
- <span data-ttu-id="b06a6-182">Contagem de chamadas dial-in/out por terceiros em conferência participada</span><span class="sxs-lookup"><span data-stu-id="b06a6-182">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="b06a6-183">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="b06a6-183">Assigned Products</span></span>
- <span data-ttu-id="b06a6-184">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="b06a6-184">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b06a6-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b06a6-185">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b06a6-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b06a6-186">Request</span></span>

<span data-ttu-id="b06a6-187">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b06a6-187">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b06a6-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="b06a6-188">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b06a6-189">C#</span><span class="sxs-lookup"><span data-stu-id="b06a6-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b06a6-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b06a6-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b06a6-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b06a6-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b06a6-192">Java</span><span class="sxs-lookup"><span data-stu-id="b06a6-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b06a6-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="b06a6-193">Response</span></span>

<span data-ttu-id="b06a6-194">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b06a6-194">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b06a6-195">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="b06a6-195">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Total Peer-to-peer Session Count,Total Organized Conference Count,Total Participated Conference Count,Peer-to-peer Last Activity Date,Organized Conference Last Activity Date,Participated Conference Last Activity Date,Peer-to-peer IM Count,Peer-to-peer Audio Count,Peer-to-peer Audio Minutes,Peer-to-peer Video Count,Peer-to-peer Video Minutes,Peer-to-peer App Sharing Count,Peer-to-peer File Transfer Count,Organized Conference IM Count,Organized Conference Audio/Video Count,Organized Conference Audio/Video Minutes,Organized Conference App Sharing Count,Organized Conference Web Count,Organized Conference Dial-in/out 3rd Party Count,Organized Conference Dial-in/out Microsoft Count,Organized Conference Dial-in Microsoft Minutes,Organized Conference Dial-out Microsoft Minutes,Paricipated Conference IM Count,Participated Conference Audio/Video Count,Participated Conference Audio/Video Minutes,Participated Conference App Sharing Count,Participated Conference Web Count,Participated Conference Dial-in/out 3rd Party Count,Assigned Products,Report Period
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
