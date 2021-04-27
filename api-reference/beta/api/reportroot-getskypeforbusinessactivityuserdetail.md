---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Obtenha dados sobre a atividade do Skype for Business por usuário.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 21c43c0098ae1a9efe7a018d51fd320a19caec17
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049741"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="61cc0-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="61cc0-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="61cc0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61cc0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61cc0-105">Obtenha dados sobre a atividade do Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="61cc0-105">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="61cc0-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Microsoft 365 - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="61cc0-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="61cc0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="61cc0-107">Permissions</span></span>

<span data-ttu-id="61cc0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61cc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="61cc0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61cc0-110">Permission type</span></span>                        | <span data-ttu-id="61cc0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61cc0-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="61cc0-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61cc0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="61cc0-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="61cc0-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="61cc0-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61cc0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61cc0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61cc0-115">Not supported.</span></span>                           |
| <span data-ttu-id="61cc0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61cc0-116">Application</span></span>                            | <span data-ttu-id="61cc0-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="61cc0-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="61cc0-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="61cc0-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="61cc0-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="61cc0-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="61cc0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61cc0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="61cc0-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="61cc0-121">Function parameters</span></span>

<span data-ttu-id="61cc0-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="61cc0-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="61cc0-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="61cc0-123">Parameter</span></span> | <span data-ttu-id="61cc0-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="61cc0-124">Type</span></span>   | <span data-ttu-id="61cc0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="61cc0-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="61cc0-126">ponto</span><span class="sxs-lookup"><span data-stu-id="61cc0-126">period</span></span>    | <span data-ttu-id="61cc0-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61cc0-127">string</span></span> | <span data-ttu-id="61cc0-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="61cc0-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="61cc0-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="61cc0-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="61cc0-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="61cc0-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="61cc0-131">data</span><span class="sxs-lookup"><span data-stu-id="61cc0-131">date</span></span>      | <span data-ttu-id="61cc0-132">Data</span><span class="sxs-lookup"><span data-stu-id="61cc0-132">Date</span></span>   | <span data-ttu-id="61cc0-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="61cc0-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="61cc0-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="61cc0-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="61cc0-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="61cc0-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="61cc0-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="61cc0-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="61cc0-137">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="61cc0-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="61cc0-138">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="61cc0-138">The default output type is text/csv.</span></span> <span data-ttu-id="61cc0-139">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="61cc0-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61cc0-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61cc0-140">Request headers</span></span>

| <span data-ttu-id="61cc0-141">Nome</span><span class="sxs-lookup"><span data-stu-id="61cc0-141">Name</span></span>          | <span data-ttu-id="61cc0-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="61cc0-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="61cc0-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="61cc0-143">Authorization</span></span> | <span data-ttu-id="61cc0-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61cc0-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="61cc0-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="61cc0-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="61cc0-147">CSV</span><span class="sxs-lookup"><span data-stu-id="61cc0-147">CSV</span></span>

<span data-ttu-id="61cc0-148">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="61cc0-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="61cc0-149">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="61cc0-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="61cc0-150">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="61cc0-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="61cc0-151">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="61cc0-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="61cc0-152">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="61cc0-152">Report Refresh Date</span></span>
- <span data-ttu-id="61cc0-153">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="61cc0-153">User Principal Name</span></span>
- <span data-ttu-id="61cc0-154">Excluído</span><span class="sxs-lookup"><span data-stu-id="61cc0-154">Is Deleted</span></span>
- <span data-ttu-id="61cc0-155">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="61cc0-155">Deleted Date</span></span>
- <span data-ttu-id="61cc0-156">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="61cc0-156">Last Activity Date</span></span>
- <span data-ttu-id="61cc0-157">Contagem total de sessão de ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="61cc0-157">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="61cc0-158">Contagem total de conferência organizada</span><span class="sxs-lookup"><span data-stu-id="61cc0-158">Total Organized Conference Count</span></span>
- <span data-ttu-id="61cc0-159">Contagem total de conferência participada</span><span class="sxs-lookup"><span data-stu-id="61cc0-159">Total Participated Conference Count</span></span>
- <span data-ttu-id="61cc0-160">Data da última atividade ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="61cc0-160">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="61cc0-161">Data da última atividade da conferência organizada</span><span class="sxs-lookup"><span data-stu-id="61cc0-161">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="61cc0-162">Data da última atividade da conferência participada</span><span class="sxs-lookup"><span data-stu-id="61cc0-162">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="61cc0-163">Contagem de mensagens instantâneas ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="61cc0-163">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="61cc0-164">Contagem de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="61cc0-164">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="61cc0-165">Minutos de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="61cc0-165">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="61cc0-166">Contagem de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="61cc0-166">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="61cc0-167">Minutos de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="61cc0-167">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="61cc0-168">Contagem de compartilhamentos de aplicativos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="61cc0-168">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="61cc0-169">Contagem de transferências de arquivos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="61cc0-169">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="61cc0-170">Contagem de mensagens instantâneas em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="61cc0-170">Organized Conference IM Count</span></span>
- <span data-ttu-id="61cc0-171">Contagem de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="61cc0-171">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="61cc0-172">Minutos de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="61cc0-172">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="61cc0-173">Contagem de compartilhamentos de aplicativos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="61cc0-173">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="61cc0-174">Contagem de Web em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="61cc0-174">Organized Conference Web Count</span></span>
- <span data-ttu-id="61cc0-175">Contagem de chamadas dial-in/out por terceiros em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="61cc0-175">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="61cc0-176">Contagem de chamadas dial-in/out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="61cc0-176">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="61cc0-177">Minutos de chamadas dial-in pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="61cc0-177">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="61cc0-178">Minutos de chamadas dial-out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="61cc0-178">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="61cc0-179">Contagem de IMs de Conferências Participadas</span><span class="sxs-lookup"><span data-stu-id="61cc0-179">Participated Conference IM Count</span></span>
- <span data-ttu-id="61cc0-180">Contagem de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="61cc0-180">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="61cc0-181">Minutos de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="61cc0-181">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="61cc0-182">Contagem de compartilhamentos de aplicativos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="61cc0-182">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="61cc0-183">Contagem de Web em conferência participada</span><span class="sxs-lookup"><span data-stu-id="61cc0-183">Participated Conference Web Count</span></span>
- <span data-ttu-id="61cc0-184">Contagem de chamadas dial-in/out por terceiros em conferência participada</span><span class="sxs-lookup"><span data-stu-id="61cc0-184">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="61cc0-185">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="61cc0-185">Assigned Products</span></span>
- <span data-ttu-id="61cc0-186">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="61cc0-186">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="61cc0-187">JSON</span><span class="sxs-lookup"><span data-stu-id="61cc0-187">JSON</span></span>

<span data-ttu-id="61cc0-188">Se tiver êxito, este método retornará um código de resposta e um `200 OK` **[objeto skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61cc0-188">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="61cc0-189">O tamanho padrão da página para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="61cc0-189">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="61cc0-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61cc0-190">Example</span></span>

### <a name="csv"></a><span data-ttu-id="61cc0-191">CSV</span><span class="sxs-lookup"><span data-stu-id="61cc0-191">CSV</span></span>

<span data-ttu-id="61cc0-192">A seguir, um exemplo que dá saída ao CSV.</span><span class="sxs-lookup"><span data-stu-id="61cc0-192">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="61cc0-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61cc0-193">Request</span></span>

<span data-ttu-id="61cc0-194">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="61cc0-194">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="61cc0-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="61cc0-195">Response</span></span>

<span data-ttu-id="61cc0-196">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="61cc0-196">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="61cc0-197">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="61cc0-197">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="61cc0-198">JSON</span><span class="sxs-lookup"><span data-stu-id="61cc0-198">JSON</span></span>

<span data-ttu-id="61cc0-199">A seguir, um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="61cc0-199">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="61cc0-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61cc0-200">Request</span></span>

<span data-ttu-id="61cc0-201">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="61cc0-201">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="61cc0-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="61cc0-202">Response</span></span>

<span data-ttu-id="61cc0-203">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="61cc0-203">The following is an example of the response.</span></span>

> <span data-ttu-id="61cc0-204">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="61cc0-204">**Note:** The response object shown here might be shortened for readability.</span></span>

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
        "Microsoft 365 ENTERPRISE E5", 
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


