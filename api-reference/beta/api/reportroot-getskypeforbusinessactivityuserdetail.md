---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Obtenha dados sobre a atividade do Skype for Business por usuário.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 45fd9007690efad03a86f4e72d78d9b493e6635d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931150"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="f36b8-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="f36b8-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

> <span data-ttu-id="f36b8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f36b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f36b8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f36b8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f36b8-106">Obtenha dados sobre a atividade do Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="f36b8-106">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="f36b8-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="f36b8-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="f36b8-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f36b8-108">Permissions</span></span>

<span data-ttu-id="f36b8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f36b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f36b8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f36b8-111">Permission type</span></span>                        | <span data-ttu-id="f36b8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f36b8-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f36b8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f36b8-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f36b8-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f36b8-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f36b8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f36b8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f36b8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f36b8-116">Not supported.</span></span>                           |
| <span data-ttu-id="f36b8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f36b8-117">Application</span></span>                            | <span data-ttu-id="f36b8-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f36b8-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f36b8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f36b8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="f36b8-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="f36b8-120">Function parameters</span></span>

<span data-ttu-id="f36b8-121">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f36b8-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="f36b8-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f36b8-122">Parameter</span></span> | <span data-ttu-id="f36b8-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f36b8-123">Type</span></span>   | <span data-ttu-id="f36b8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f36b8-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f36b8-125">ponto</span><span class="sxs-lookup"><span data-stu-id="f36b8-125">period</span></span>    | <span data-ttu-id="f36b8-126">string</span><span class="sxs-lookup"><span data-stu-id="f36b8-126">string</span></span> | <span data-ttu-id="f36b8-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f36b8-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f36b8-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="f36b8-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f36b8-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f36b8-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="f36b8-130">data</span><span class="sxs-lookup"><span data-stu-id="f36b8-130">date</span></span>      | <span data-ttu-id="f36b8-131">Data</span><span class="sxs-lookup"><span data-stu-id="f36b8-131">Date</span></span>   | <span data-ttu-id="f36b8-132">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="f36b8-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="f36b8-133">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="f36b8-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="f36b8-134">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="f36b8-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="f36b8-135">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="f36b8-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="f36b8-136">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="f36b8-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f36b8-137">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="f36b8-137">The default output type is text/csv.</span></span> <span data-ttu-id="f36b8-138">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="f36b8-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f36b8-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f36b8-139">Request headers</span></span>

| <span data-ttu-id="f36b8-140">Nome</span><span class="sxs-lookup"><span data-stu-id="f36b8-140">Name</span></span>          | <span data-ttu-id="f36b8-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="f36b8-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f36b8-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="f36b8-142">Authorization</span></span> | <span data-ttu-id="f36b8-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f36b8-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f36b8-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f36b8-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f36b8-146">CSV</span><span class="sxs-lookup"><span data-stu-id="f36b8-146">CSV</span></span>

<span data-ttu-id="f36b8-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="f36b8-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f36b8-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="f36b8-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f36b8-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f36b8-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f36b8-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="f36b8-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f36b8-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="f36b8-151">Report Refresh Date</span></span>
- <span data-ttu-id="f36b8-152">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="f36b8-152">User Principal Name</span></span>
- <span data-ttu-id="f36b8-153">Excluído</span><span class="sxs-lookup"><span data-stu-id="f36b8-153">Is Deleted</span></span>
- <span data-ttu-id="f36b8-154">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="f36b8-154">Deleted Date</span></span>
- <span data-ttu-id="f36b8-155">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="f36b8-155">Last Activity Date</span></span>
- <span data-ttu-id="f36b8-156">Contagem total de sessão de ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="f36b8-156">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="f36b8-157">Contagem total de conferência organizada</span><span class="sxs-lookup"><span data-stu-id="f36b8-157">Total Organized Conference Count</span></span>
- <span data-ttu-id="f36b8-158">Contagem total de conferência participada</span><span class="sxs-lookup"><span data-stu-id="f36b8-158">Total Participated Conference Count</span></span>
- <span data-ttu-id="f36b8-159">Data da última atividade ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="f36b8-159">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="f36b8-160">Data da última atividade da conferência organizada</span><span class="sxs-lookup"><span data-stu-id="f36b8-160">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="f36b8-161">Data da última atividade da conferência participada</span><span class="sxs-lookup"><span data-stu-id="f36b8-161">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="f36b8-162">Contagem de mensagens instantâneas ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="f36b8-162">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="f36b8-163">Contagem de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="f36b8-163">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="f36b8-164">Minutos de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="f36b8-164">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="f36b8-165">Contagem de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="f36b8-165">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="f36b8-166">Minutos de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="f36b8-166">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="f36b8-167">Contagem de compartilhamentos de aplicativos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="f36b8-167">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="f36b8-168">Contagem de transferências de arquivos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="f36b8-168">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="f36b8-169">Contagem de mensagens instantâneas em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="f36b8-169">Organized Conference IM Count</span></span>
- <span data-ttu-id="f36b8-170">Contagem de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="f36b8-170">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="f36b8-171">Minutos de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="f36b8-171">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="f36b8-172">Contagem de compartilhamentos de aplicativos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="f36b8-172">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="f36b8-173">Contagem de Web em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="f36b8-173">Organized Conference Web Count</span></span>
- <span data-ttu-id="f36b8-174">Contagem de chamadas dial-in/out por terceiros em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="f36b8-174">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="f36b8-175">Contagem de chamadas dial-in/out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="f36b8-175">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="f36b8-176">Minutos de chamadas dial-in pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="f36b8-176">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="f36b8-177">Minutos de chamadas dial-out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="f36b8-177">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="f36b8-178">Contagem de mensagens Instantâneas de participou da conferência</span><span class="sxs-lookup"><span data-stu-id="f36b8-178">Participated Conference IM Count</span></span>
- <span data-ttu-id="f36b8-179">Contagem de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="f36b8-179">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="f36b8-180">Minutos de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="f36b8-180">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="f36b8-181">Contagem de compartilhamentos de aplicativos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="f36b8-181">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="f36b8-182">Contagem de Web em conferência participada</span><span class="sxs-lookup"><span data-stu-id="f36b8-182">Participated Conference Web Count</span></span>
- <span data-ttu-id="f36b8-183">Contagem de chamadas dial-in/out por terceiros em conferência participada</span><span class="sxs-lookup"><span data-stu-id="f36b8-183">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="f36b8-184">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="f36b8-184">Assigned Products</span></span>
- <span data-ttu-id="f36b8-185">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="f36b8-185">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="f36b8-186">JSON</span><span class="sxs-lookup"><span data-stu-id="f36b8-186">JSON</span></span>

<span data-ttu-id="f36b8-187">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f36b8-187">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="f36b8-188">O tamanho de página padrão para essa solicitação é 200 itens.</span><span class="sxs-lookup"><span data-stu-id="f36b8-188">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="f36b8-189">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f36b8-189">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f36b8-190">CSV</span><span class="sxs-lookup"><span data-stu-id="f36b8-190">CSV</span></span>

<span data-ttu-id="f36b8-191">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="f36b8-191">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f36b8-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f36b8-192">Request</span></span>

<span data-ttu-id="f36b8-193">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f36b8-193">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="f36b8-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="f36b8-194">Response</span></span>

<span data-ttu-id="f36b8-195">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f36b8-195">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f36b8-196">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="f36b8-196">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="f36b8-197">JSON</span><span class="sxs-lookup"><span data-stu-id="f36b8-197">JSON</span></span>

<span data-ttu-id="f36b8-198">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="f36b8-198">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f36b8-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f36b8-199">Request</span></span>

<span data-ttu-id="f36b8-200">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f36b8-200">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="f36b8-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="f36b8-201">Response</span></span>

<span data-ttu-id="f36b8-202">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f36b8-202">The following is an example of the response.</span></span>

> <span data-ttu-id="f36b8-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f36b8-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
