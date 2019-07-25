---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Obtenha dados sobre a atividade do Skype for Business por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 42bdb7f5e486c1f252d52f7af3034b8fa3c89820
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892484"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="219c0-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="219c0-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="219c0-104">Obtenha dados sobre a atividade do Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="219c0-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="219c0-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="219c0-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="219c0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="219c0-106">Permissions</span></span>

<span data-ttu-id="219c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="219c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="219c0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="219c0-109">Permission type</span></span>                        | <span data-ttu-id="219c0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="219c0-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="219c0-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="219c0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="219c0-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="219c0-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="219c0-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="219c0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="219c0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="219c0-114">Not supported.</span></span>                           |
| <span data-ttu-id="219c0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="219c0-115">Application</span></span>                            | <span data-ttu-id="219c0-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="219c0-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="219c0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="219c0-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="219c0-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="219c0-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="219c0-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="219c0-119">Function parameters</span></span>

<span data-ttu-id="219c0-120">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="219c0-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="219c0-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="219c0-121">Parameter</span></span> | <span data-ttu-id="219c0-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="219c0-122">Type</span></span>   | <span data-ttu-id="219c0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="219c0-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="219c0-124">ponto</span><span class="sxs-lookup"><span data-stu-id="219c0-124">period</span></span>    | <span data-ttu-id="219c0-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="219c0-125">string</span></span> | <span data-ttu-id="219c0-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="219c0-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="219c0-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="219c0-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="219c0-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="219c0-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="219c0-129">data</span><span class="sxs-lookup"><span data-stu-id="219c0-129">date</span></span>      | <span data-ttu-id="219c0-130">Data</span><span class="sxs-lookup"><span data-stu-id="219c0-130">Date</span></span>   | <span data-ttu-id="219c0-131">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="219c0-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="219c0-132">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="219c0-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="219c0-133">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="219c0-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="219c0-134">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="219c0-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="219c0-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="219c0-135">Request headers</span></span>

| <span data-ttu-id="219c0-136">Nome</span><span class="sxs-lookup"><span data-stu-id="219c0-136">Name</span></span>          | <span data-ttu-id="219c0-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="219c0-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="219c0-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="219c0-138">Authorization</span></span> | <span data-ttu-id="219c0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="219c0-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="219c0-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="219c0-141">If-None-Match</span></span> | <span data-ttu-id="219c0-142">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="219c0-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="219c0-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="219c0-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="219c0-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="219c0-144">Response</span></span>

<span data-ttu-id="219c0-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="219c0-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="219c0-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="219c0-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="219c0-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="219c0-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="219c0-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="219c0-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="219c0-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="219c0-149">Report Refresh Date</span></span>
- <span data-ttu-id="219c0-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="219c0-150">User Principal Name</span></span>
- <span data-ttu-id="219c0-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="219c0-151">Is Deleted</span></span>
- <span data-ttu-id="219c0-152">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="219c0-152">Deleted Date</span></span>
- <span data-ttu-id="219c0-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="219c0-153">Last Activity Date</span></span>
- <span data-ttu-id="219c0-154">Contagem total de sessão de ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="219c0-154">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="219c0-155">Contagem total de conferência organizada</span><span class="sxs-lookup"><span data-stu-id="219c0-155">Total Organized Conference Count</span></span>
- <span data-ttu-id="219c0-156">Contagem total de conferência participada</span><span class="sxs-lookup"><span data-stu-id="219c0-156">Total Participated Conference Count</span></span>
- <span data-ttu-id="219c0-157">Data da última atividade ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="219c0-157">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="219c0-158">Data da última atividade da conferência organizada</span><span class="sxs-lookup"><span data-stu-id="219c0-158">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="219c0-159">Data da última atividade da conferência participada</span><span class="sxs-lookup"><span data-stu-id="219c0-159">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="219c0-160">Contagem de mensagens instantâneas ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="219c0-160">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="219c0-161">Contagem de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="219c0-161">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="219c0-162">Minutos de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="219c0-162">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="219c0-163">Contagem de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="219c0-163">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="219c0-164">Minutos de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="219c0-164">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="219c0-165">Contagem de compartilhamentos de aplicativos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="219c0-165">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="219c0-166">Contagem de transferências de arquivos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="219c0-166">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="219c0-167">Contagem de mensagens instantâneas em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="219c0-167">Organized Conference IM Count</span></span>
- <span data-ttu-id="219c0-168">Contagem de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="219c0-168">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="219c0-169">Minutos de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="219c0-169">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="219c0-170">Contagem de compartilhamentos de aplicativos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="219c0-170">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="219c0-171">Contagem de Web em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="219c0-171">Organized Conference Web Count</span></span>
- <span data-ttu-id="219c0-172">Contagem de chamadas dial-in/out por terceiros em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="219c0-172">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="219c0-173">Contagem de chamadas dial-in/out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="219c0-173">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="219c0-174">Minutos de chamadas dial-in pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="219c0-174">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="219c0-175">Minutos de chamadas dial-out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="219c0-175">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="219c0-176">Contagem de mensagens instantâneas em conferência participada</span><span class="sxs-lookup"><span data-stu-id="219c0-176">Paricipated Conference IM Count</span></span>
- <span data-ttu-id="219c0-177">Contagem de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="219c0-177">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="219c0-178">Minutos de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="219c0-178">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="219c0-179">Contagem de compartilhamentos de aplicativos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="219c0-179">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="219c0-180">Contagem de Web em conferência participada</span><span class="sxs-lookup"><span data-stu-id="219c0-180">Participated Conference Web Count</span></span>
- <span data-ttu-id="219c0-181">Contagem de chamadas dial-in/out por terceiros em conferência participada</span><span class="sxs-lookup"><span data-stu-id="219c0-181">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="219c0-182">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="219c0-182">Assigned Products</span></span>
- <span data-ttu-id="219c0-183">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="219c0-183">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="219c0-184">Exemplo</span><span class="sxs-lookup"><span data-stu-id="219c0-184">Example</span></span>

#### <a name="request"></a><span data-ttu-id="219c0-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="219c0-185">Request</span></span>

<span data-ttu-id="219c0-186">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="219c0-186">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="219c0-187">C#</span><span class="sxs-lookup"><span data-stu-id="219c0-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="219c0-188">Javascript</span><span class="sxs-lookup"><span data-stu-id="219c0-188">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="219c0-189">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="219c0-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="219c0-190">Java</span><span class="sxs-lookup"><span data-stu-id="219c0-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="219c0-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="219c0-191">Response</span></span>

<span data-ttu-id="219c0-192">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="219c0-192">The following is an example of the response.</span></span>

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

<span data-ttu-id="219c0-193">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="219c0-193">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
