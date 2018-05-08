# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="b5b6e-101">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="b5b6e-101">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="b5b6e-102">Obtenha dados sobre a atividade do Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-102">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="b5b6e-103">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="b5b6e-103">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="b5b6e-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5b6e-104">Permissions</span></span>

<span data-ttu-id="b5b6e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b5b6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="b5b6e-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5b6e-107">Permission type</span></span>                        | <span data-ttu-id="b5b6e-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5b6e-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b5b6e-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5b6e-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5b6e-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5b6e-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b5b6e-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5b6e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5b6e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-112">Not supported.</span></span>                           |
| <span data-ttu-id="b5b6e-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5b6e-113">Application</span></span>                            | <span data-ttu-id="b5b6e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5b6e-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b5b6e-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5b6e-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="b5b6e-116">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="b5b6e-116">Request parameters</span></span>

<span data-ttu-id="b5b6e-117">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b5b6e-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b5b6e-118">Parameter</span></span> | <span data-ttu-id="b5b6e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5b6e-119">Type</span></span>   | <span data-ttu-id="b5b6e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5b6e-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b5b6e-121">ponto</span><span class="sxs-lookup"><span data-stu-id="b5b6e-121">period</span></span>    | <span data-ttu-id="b5b6e-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5b6e-122">string</span></span> | <span data-ttu-id="b5b6e-123">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b5b6e-124">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b5b6e-125">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-125">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b5b6e-126">data</span><span class="sxs-lookup"><span data-stu-id="b5b6e-126">date</span></span>      | <span data-ttu-id="b5b6e-127">Data</span><span class="sxs-lookup"><span data-stu-id="b5b6e-127">Date</span></span>   | <span data-ttu-id="b5b6e-128">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b5b6e-129">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b5b6e-130">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b5b6e-131">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5b6e-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5b6e-132">Request headers</span></span>

| <span data-ttu-id="b5b6e-133">Nome</span><span class="sxs-lookup"><span data-stu-id="b5b6e-133">Name</span></span>          | <span data-ttu-id="b5b6e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5b6e-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b5b6e-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5b6e-135">Authorization</span></span> | <span data-ttu-id="b5b6e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b5b6e-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b5b6e-138">If-None-Match</span></span> | <span data-ttu-id="b5b6e-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b5b6e-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b5b6e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5b6e-141">Response</span></span>

<span data-ttu-id="b5b6e-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b5b6e-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b5b6e-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b5b6e-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b5b6e-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="b5b6e-146">Report Refresh Date</span></span>
- <span data-ttu-id="b5b6e-147">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="b5b6e-147">User Principal Name</span></span>
- <span data-ttu-id="b5b6e-148">Excluído</span><span class="sxs-lookup"><span data-stu-id="b5b6e-148">Is Deleted</span></span>
- <span data-ttu-id="b5b6e-149">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="b5b6e-149">Deleted Date</span></span>
- <span data-ttu-id="b5b6e-150">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="b5b6e-150">Last Activity Date</span></span>
- <span data-ttu-id="b5b6e-151">Contagem total de sessão de ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="b5b6e-151">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="b5b6e-152">Contagem total de conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-152">Total Organized Conference Count</span></span>
- <span data-ttu-id="b5b6e-153">Contagem total de conferência participada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-153">Total Participated Conference Count</span></span>
- <span data-ttu-id="b5b6e-154">Data da última atividade ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="b5b6e-154">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="b5b6e-155">Data da última atividade da conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-155">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="b5b6e-156">Data da última atividade da conferência participada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-156">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="b5b6e-157">Contagem de mensagens instantâneas ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="b5b6e-157">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="b5b6e-158">Contagem de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="b5b6e-158">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="b5b6e-159">Minutos de áudios ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="b5b6e-159">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="b5b6e-160">Contagem de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="b5b6e-160">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="b5b6e-161">Minutos de vídeos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="b5b6e-161">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="b5b6e-162">Contagem de compartilhamentos de aplicativos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="b5b6e-162">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="b5b6e-163">Contagem de transferências de arquivos ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="b5b6e-163">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="b5b6e-164">Contagem de mensagens instantâneas em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-164">Organized Conference IM Count</span></span>
- <span data-ttu-id="b5b6e-165">Contagem de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-165">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="b5b6e-166">Minutos de áudios/vídeos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-166">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="b5b6e-167">Contagem de compartilhamentos de aplicativos em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-167">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="b5b6e-168">Contagem de Web em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-168">Organized Conference Web Count</span></span>
- <span data-ttu-id="b5b6e-169">Contagem de chamadas dial-in/out por terceiros em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-169">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="b5b6e-170">Contagem de chamadas dial-in/out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-170">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="b5b6e-171">Minutos de chamadas dial-in pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-171">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="b5b6e-172">Minutos de chamadas dial-out pela Microsoft em conferência organizada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-172">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="b5b6e-173">Contagem de mensagens instantâneas em conferência participada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-173">Paricipated Conference IM Count</span></span>
- <span data-ttu-id="b5b6e-174">Contagem de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-174">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="b5b6e-175">Minutos de áudios/vídeos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-175">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="b5b6e-176">Contagem de compartilhamentos de aplicativos em conferência participada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-176">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="b5b6e-177">Contagem de Web em conferência participada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-177">Participated Conference Web Count</span></span>
- <span data-ttu-id="b5b6e-178">Contagem de chamadas dial-in/out por terceiros em conferência participada</span><span class="sxs-lookup"><span data-stu-id="b5b6e-178">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="b5b6e-179">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="b5b6e-179">Assigned Products</span></span>
- <span data-ttu-id="b5b6e-180">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="b5b6e-180">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b5b6e-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5b6e-181">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b5b6e-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5b6e-182">Request</span></span>

<span data-ttu-id="b5b6e-183">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-183">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b5b6e-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5b6e-184">Response</span></span>

<span data-ttu-id="b5b6e-185">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-185">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b5b6e-186">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="b5b6e-186">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Total Peer-to-peer Session Count,Total Organized Conference Count,Total Participated Conference Count,Peer-to-peer Last Activity Date,Organized Conference Last Activity Date,Participated Conference Last Activity Date,Peer-to-peer IM Count,Peer-to-peer Audio Count,Peer-to-peer Audio Minutes,Peer-to-peer Video Count,Peer-to-peer Video Minutes,Peer-to-peer App Sharing Count,Peer-to-peer File Transfer Count,Organized Conference IM Count,Organized Conference Audio/Video Count,Organized Conference Audio/Video Minutes,Organized Conference App Sharing Count,Organized Conference Web Count,Organized Conference Dial-in/out 3rd Party Count,Organized Conference Dial-in/out Microsoft Count,Organized Conference Dial-in Microsoft Minutes,Organized Conference Dial-out Microsoft Minutes,Paricipated Conference IM Count,Participated Conference Audio/Video Count,Participated Conference Audio/Video Minutes,Participated Conference App Sharing Count,Participated Conference Web Count,Participated Conference Dial-in/out 3rd Party Count,Assigned Products,Report Period
```
