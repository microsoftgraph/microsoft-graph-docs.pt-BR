---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Obtenha dados sobre a atividade do Skype for Business por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 34f80d21620eaa65a44e7c5a0ae8303ec43dfbb7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572896"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="361db-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="361db-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="361db-104">Obtenha dados sobre a atividade do Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="361db-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="361db-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="361db-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="361db-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="361db-106">Permissions</span></span>

<span data-ttu-id="361db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="361db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="361db-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="361db-109">Permission type</span></span>                        | <span data-ttu-id="361db-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="361db-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="361db-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="361db-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="361db-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="361db-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="361db-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="361db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="361db-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="361db-114">Not supported.</span></span>                           |
| <span data-ttu-id="361db-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="361db-115">Application</span></span>                            | <span data-ttu-id="361db-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="361db-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="361db-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="361db-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="361db-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="361db-118">Function parameters</span></span>

<span data-ttu-id="361db-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="361db-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="361db-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="361db-120">Parameter</span></span> | <span data-ttu-id="361db-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="361db-121">Type</span></span>   | <span data-ttu-id="361db-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="361db-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="361db-123">ponto</span><span class="sxs-lookup"><span data-stu-id="361db-123">period</span></span>    | <span data-ttu-id="361db-124">string</span><span class="sxs-lookup"><span data-stu-id="361db-124">string</span></span> | <span data-ttu-id="361db-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="361db-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="361db-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="361db-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="361db-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="361db-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="361db-128">data</span><span class="sxs-lookup"><span data-stu-id="361db-128">date</span></span>      | <span data-ttu-id="361db-129">Data</span><span class="sxs-lookup"><span data-stu-id="361db-129">Date</span></span>   | <span data-ttu-id="361db-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="361db-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="361db-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="361db-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="361db-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="361db-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="361db-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="361db-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="361db-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="361db-134">Request headers</span></span>

| <span data-ttu-id="361db-135">Nome</span><span class="sxs-lookup"><span data-stu-id="361db-135">Name</span></span>          | <span data-ttu-id="361db-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="361db-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="361db-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="361db-137">Authorization</span></span> | <span data-ttu-id="361db-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="361db-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="361db-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="361db-140">If-None-Match</span></span> | <span data-ttu-id="361db-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="361db-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="361db-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="361db-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="361db-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="361db-143">Response</span></span>

<span data-ttu-id="361db-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="361db-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="361db-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="361db-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="361db-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="361db-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="361db-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="361db-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="361db-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="361db-148">Report Refresh Date</span></span>
- <span data-ttu-id="361db-149">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="361db-149">User Principal Name</span></span>
- <span data-ttu-id="361db-150">Excluído</span><span class="sxs-lookup"><span data-stu-id="361db-150">Is Deleted</span></span>
- <span data-ttu-id="361db-151">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="361db-151">Deleted Date</span></span>
- <span data-ttu-id="361db-152">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="361db-152">Last Activity Date</span></span>
- <span data-ttu-id="361db-153">Contagem total de sessão de ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="361db-153">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="361db-154">Contagem total de conferência organizada</span><span class="sxs-lookup"><span data-stu-id="361db-154">Total Organized Conference Count</span></span>
- <span data-ttu-id="361db-155">Contagem total de conferência participada</span><span class="sxs-lookup"><span data-stu-id="361db-155">Total Participated Conference Count</span></span>
- <span data-ttu-id="361db-156">Data da última atividade ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="361db-156">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="361db-157">Data da última atividade da conferência organizada</span><span class="sxs-lookup"><span data-stu-id="361db-157">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="361db-158">Data da última atividade da conferência participada</span><span class="sxs-lookup"><span data-stu-id="361db-158">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="361db-159">Contagem de mensagens instantâneas ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="361db-159">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="361db-160">Contagem de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="361db-160">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="361db-161">Minutos de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="361db-161">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="361db-162">Contagem de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="361db-162">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="361db-163">Minutos de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="361db-163">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="361db-164">Contagem de compartilhamentos de aplicativos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="361db-164">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="361db-165">Contagem de transferências de arquivos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="361db-165">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="361db-166">Contagem de mensagens instantâneas em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="361db-166">Organized Conference IM Count</span></span>
- <span data-ttu-id="361db-167">Contagem de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="361db-167">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="361db-168">Minutos de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="361db-168">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="361db-169">Contagem de compartilhamentos de aplicativos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="361db-169">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="361db-170">Contagem de Web em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="361db-170">Organized Conference Web Count</span></span>
- <span data-ttu-id="361db-171">Contagem de chamadas dial-in/out por terceiros em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="361db-171">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="361db-172">Contagem de chamadas dial-in/out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="361db-172">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="361db-173">Minutos de chamadas dial-in pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="361db-173">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="361db-174">Minutos de chamadas dial-out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="361db-174">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="361db-175">Contagem de mensagens instantâneas em conferência participada</span><span class="sxs-lookup"><span data-stu-id="361db-175">Paricipated Conference IM Count</span></span>
- <span data-ttu-id="361db-176">Contagem de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="361db-176">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="361db-177">Minutos de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="361db-177">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="361db-178">Contagem de compartilhamentos de aplicativos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="361db-178">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="361db-179">Contagem de Web em conferência participada</span><span class="sxs-lookup"><span data-stu-id="361db-179">Participated Conference Web Count</span></span>
- <span data-ttu-id="361db-180">Contagem de chamadas dial-in/out por terceiros em conferência participada</span><span class="sxs-lookup"><span data-stu-id="361db-180">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="361db-181">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="361db-181">Assigned Products</span></span>
- <span data-ttu-id="361db-182">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="361db-182">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="361db-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="361db-183">Example</span></span>

#### <a name="request"></a><span data-ttu-id="361db-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="361db-184">Request</span></span>

<span data-ttu-id="361db-185">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="361db-185">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="361db-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="361db-186">Response</span></span>

<span data-ttu-id="361db-187">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="361db-187">The following is an example of the response.</span></span>

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

<span data-ttu-id="361db-188">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="361db-188">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Total Peer-to-peer Session Count,Total Organized Conference Count,Total Participated Conference Count,Peer-to-peer Last Activity Date,Organized Conference Last Activity Date,Participated Conference Last Activity Date,Peer-to-peer IM Count,Peer-to-peer Audio Count,Peer-to-peer Audio Minutes,Peer-to-peer Video Count,Peer-to-peer Video Minutes,Peer-to-peer App Sharing Count,Peer-to-peer File Transfer Count,Organized Conference IM Count,Organized Conference Audio/Video Count,Organized Conference Audio/Video Minutes,Organized Conference App Sharing Count,Organized Conference Web Count,Organized Conference Dial-in/out 3rd Party Count,Organized Conference Dial-in/out Microsoft Count,Organized Conference Dial-in Microsoft Minutes,Organized Conference Dial-out Microsoft Minutes,Paricipated Conference IM Count,Participated Conference Audio/Video Count,Participated Conference Audio/Video Minutes,Participated Conference App Sharing Count,Participated Conference Web Count,Participated Conference Dial-in/out 3rd Party Count,Assigned Products,Report Period
```
