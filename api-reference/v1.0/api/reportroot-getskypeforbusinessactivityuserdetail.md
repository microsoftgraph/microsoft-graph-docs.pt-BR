---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Obtenha dados sobre a atividade do Skype for Business por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f9452b0e87be245101102056818086be5a417fdc
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895927"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="088ab-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="088ab-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="088ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="088ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="088ab-105">Obtenha dados sobre a atividade do Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="088ab-105">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="088ab-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-Skype for Business Activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="088ab-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="088ab-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="088ab-107">Permissions</span></span>

<span data-ttu-id="088ab-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="088ab-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="088ab-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="088ab-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="088ab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="088ab-110">Permission type</span></span>                        | <span data-ttu-id="088ab-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="088ab-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="088ab-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="088ab-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="088ab-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="088ab-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="088ab-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="088ab-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="088ab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="088ab-115">Not supported.</span></span>                           |
| <span data-ttu-id="088ab-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="088ab-116">Application</span></span>                            | <span data-ttu-id="088ab-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="088ab-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="088ab-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="088ab-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="088ab-119">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="088ab-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="088ab-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="088ab-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="088ab-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="088ab-121">Function parameters</span></span>

<span data-ttu-id="088ab-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="088ab-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="088ab-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="088ab-123">Parameter</span></span> | <span data-ttu-id="088ab-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="088ab-124">Type</span></span>   | <span data-ttu-id="088ab-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="088ab-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="088ab-126">ponto</span><span class="sxs-lookup"><span data-stu-id="088ab-126">period</span></span>    | <span data-ttu-id="088ab-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="088ab-127">string</span></span> | <span data-ttu-id="088ab-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="088ab-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="088ab-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="088ab-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="088ab-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="088ab-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="088ab-131">data</span><span class="sxs-lookup"><span data-stu-id="088ab-131">date</span></span>      | <span data-ttu-id="088ab-132">Data</span><span class="sxs-lookup"><span data-stu-id="088ab-132">Date</span></span>   | <span data-ttu-id="088ab-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="088ab-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="088ab-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="088ab-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="088ab-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="088ab-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="088ab-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="088ab-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="088ab-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="088ab-137">Request headers</span></span>

| <span data-ttu-id="088ab-138">Nome</span><span class="sxs-lookup"><span data-stu-id="088ab-138">Name</span></span>          | <span data-ttu-id="088ab-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="088ab-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="088ab-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="088ab-140">Authorization</span></span> | <span data-ttu-id="088ab-141">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="088ab-141">Bearer {token}.</span></span> <span data-ttu-id="088ab-142">Required.</span><span class="sxs-lookup"><span data-stu-id="088ab-142">Required.</span></span>                |
| <span data-ttu-id="088ab-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="088ab-143">If-None-Match</span></span> | <span data-ttu-id="088ab-144">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="088ab-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="088ab-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="088ab-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="088ab-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="088ab-146">Response</span></span>

<span data-ttu-id="088ab-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="088ab-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="088ab-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="088ab-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="088ab-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="088ab-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="088ab-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="088ab-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="088ab-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="088ab-151">Report Refresh Date</span></span>
- <span data-ttu-id="088ab-152">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="088ab-152">User Principal Name</span></span>
- <span data-ttu-id="088ab-153">Excluído</span><span class="sxs-lookup"><span data-stu-id="088ab-153">Is Deleted</span></span>
- <span data-ttu-id="088ab-154">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="088ab-154">Deleted Date</span></span>
- <span data-ttu-id="088ab-155">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="088ab-155">Last Activity Date</span></span>
- <span data-ttu-id="088ab-156">Contagem total de sessão de ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="088ab-156">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="088ab-157">Contagem total de conferência organizada</span><span class="sxs-lookup"><span data-stu-id="088ab-157">Total Organized Conference Count</span></span>
- <span data-ttu-id="088ab-158">Contagem total de conferência participada</span><span class="sxs-lookup"><span data-stu-id="088ab-158">Total Participated Conference Count</span></span>
- <span data-ttu-id="088ab-159">Data da última atividade ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="088ab-159">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="088ab-160">Data da última atividade da conferência organizada</span><span class="sxs-lookup"><span data-stu-id="088ab-160">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="088ab-161">Data da última atividade da conferência participada</span><span class="sxs-lookup"><span data-stu-id="088ab-161">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="088ab-162">Contagem de mensagens instantâneas ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="088ab-162">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="088ab-163">Contagem de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="088ab-163">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="088ab-164">Minutos de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="088ab-164">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="088ab-165">Contagem de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="088ab-165">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="088ab-166">Minutos de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="088ab-166">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="088ab-167">Contagem de compartilhamentos de aplicativos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="088ab-167">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="088ab-168">Contagem de transferências de arquivos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="088ab-168">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="088ab-169">Contagem de mensagens instantâneas em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="088ab-169">Organized Conference IM Count</span></span>
- <span data-ttu-id="088ab-170">Contagem de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="088ab-170">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="088ab-171">Minutos de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="088ab-171">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="088ab-172">Contagem de compartilhamentos de aplicativos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="088ab-172">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="088ab-173">Contagem de Web em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="088ab-173">Organized Conference Web Count</span></span>
- <span data-ttu-id="088ab-174">Contagem de chamadas dial-in/out por terceiros em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="088ab-174">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="088ab-175">Contagem de chamadas dial-in/out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="088ab-175">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="088ab-176">Minutos de chamadas dial-in pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="088ab-176">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="088ab-177">Minutos de chamadas dial-out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="088ab-177">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="088ab-178">Contagem de mensagens instantâneas em conferência participada</span><span class="sxs-lookup"><span data-stu-id="088ab-178">Paricipated Conference IM Count</span></span>
- <span data-ttu-id="088ab-179">Contagem de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="088ab-179">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="088ab-180">Minutos de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="088ab-180">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="088ab-181">Contagem de compartilhamentos de aplicativos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="088ab-181">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="088ab-182">Contagem de Web em conferência participada</span><span class="sxs-lookup"><span data-stu-id="088ab-182">Participated Conference Web Count</span></span>
- <span data-ttu-id="088ab-183">Contagem de chamadas dial-in/out por terceiros em conferência participada</span><span class="sxs-lookup"><span data-stu-id="088ab-183">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="088ab-184">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="088ab-184">Assigned Products</span></span>
- <span data-ttu-id="088ab-185">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="088ab-185">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="088ab-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="088ab-186">Example</span></span>

#### <a name="request"></a><span data-ttu-id="088ab-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="088ab-187">Request</span></span>

<span data-ttu-id="088ab-188">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="088ab-188">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="088ab-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="088ab-189">Response</span></span>

<span data-ttu-id="088ab-190">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="088ab-190">The following is an example of the response.</span></span>

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

<span data-ttu-id="088ab-191">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="088ab-191">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
