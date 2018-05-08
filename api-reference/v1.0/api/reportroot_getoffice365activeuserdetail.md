# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="469ee-101">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="469ee-101">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="469ee-102">Obtenha dados sobre os usuários ativos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="469ee-102">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="469ee-103">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="469ee-103">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="469ee-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="469ee-104">Permissions</span></span>

<span data-ttu-id="469ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="469ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="469ee-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="469ee-107">Permission type</span></span>                        | <span data-ttu-id="469ee-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="469ee-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="469ee-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="469ee-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="469ee-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="469ee-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="469ee-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="469ee-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="469ee-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="469ee-112">Not supported.</span></span>                           |
| <span data-ttu-id="469ee-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="469ee-113">Application</span></span>                            | <span data-ttu-id="469ee-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="469ee-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="469ee-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="469ee-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="469ee-116">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="469ee-116">Request parameters</span></span>

<span data-ttu-id="469ee-117">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="469ee-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="469ee-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="469ee-118">Parameter</span></span> | <span data-ttu-id="469ee-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="469ee-119">Type</span></span>   | <span data-ttu-id="469ee-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="469ee-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="469ee-121">ponto</span><span class="sxs-lookup"><span data-stu-id="469ee-121">period</span></span>    | <span data-ttu-id="469ee-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="469ee-122">string</span></span> | <span data-ttu-id="469ee-123">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="469ee-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="469ee-124">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="469ee-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="469ee-125">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="469ee-125">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="469ee-126">data</span><span class="sxs-lookup"><span data-stu-id="469ee-126">date</span></span>      | <span data-ttu-id="469ee-127">Data</span><span class="sxs-lookup"><span data-stu-id="469ee-127">Date</span></span>   | <span data-ttu-id="469ee-128">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="469ee-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="469ee-129">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="469ee-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="469ee-130">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="469ee-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="469ee-131">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="469ee-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="469ee-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="469ee-132">Request headers</span></span>

| <span data-ttu-id="469ee-133">Nome</span><span class="sxs-lookup"><span data-stu-id="469ee-133">Name</span></span>          | <span data-ttu-id="469ee-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="469ee-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="469ee-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="469ee-135">Authorization</span></span> | <span data-ttu-id="469ee-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="469ee-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="469ee-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="469ee-138">If-None-Match</span></span> | <span data-ttu-id="469ee-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="469ee-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="469ee-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="469ee-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="469ee-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="469ee-141">Response</span></span>

<span data-ttu-id="469ee-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="469ee-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="469ee-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="469ee-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="469ee-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="469ee-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="469ee-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="469ee-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="469ee-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="469ee-146">Report Refresh Date</span></span>
- <span data-ttu-id="469ee-147">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="469ee-147">User Principal Name</span></span>
- <span data-ttu-id="469ee-148">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="469ee-148">Display Name</span></span>
- <span data-ttu-id="469ee-149">Excluído</span><span class="sxs-lookup"><span data-stu-id="469ee-149">Is Deleted</span></span>
- <span data-ttu-id="469ee-150">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="469ee-150">Deleted Date</span></span>
- <span data-ttu-id="469ee-151">Tem a licença do Exchange</span><span class="sxs-lookup"><span data-stu-id="469ee-151">Has Exchange License</span></span>
- <span data-ttu-id="469ee-152">Tem a licença do OneDrive</span><span class="sxs-lookup"><span data-stu-id="469ee-152">Has OneDrive License</span></span>
- <span data-ttu-id="469ee-153">Tem a licença do SharePoint</span><span class="sxs-lookup"><span data-stu-id="469ee-153">Has SharePoint License</span></span>
- <span data-ttu-id="469ee-154">Tem a licença do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="469ee-154">Has Skype For Business License</span></span>
- <span data-ttu-id="469ee-155">Tem a licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="469ee-155">Has Yammer License</span></span>
- <span data-ttu-id="469ee-156">Tem a licença do Teams</span><span class="sxs-lookup"><span data-stu-id="469ee-156">Has Teams License</span></span>
- <span data-ttu-id="469ee-157">Data da última atividade do Exchange</span><span class="sxs-lookup"><span data-stu-id="469ee-157">Exchange Last Activity Date</span></span>
- <span data-ttu-id="469ee-158">Data da última atividade do OneDrive</span><span class="sxs-lookup"><span data-stu-id="469ee-158">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="469ee-159">Data da última atividade do SharePoint</span><span class="sxs-lookup"><span data-stu-id="469ee-159">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="469ee-160">Data da última atividade do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="469ee-160">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="469ee-161">Data da última atividade do Yammer</span><span class="sxs-lookup"><span data-stu-id="469ee-161">Yammer Last Activity Date</span></span>
- <span data-ttu-id="469ee-162">Data da última atividade do Teams</span><span class="sxs-lookup"><span data-stu-id="469ee-162">Teams Last Activity Date</span></span>
- <span data-ttu-id="469ee-163">Data de atribuição da licença do Exchange</span><span class="sxs-lookup"><span data-stu-id="469ee-163">Exchange License Assign Date</span></span>
- <span data-ttu-id="469ee-164">Data de atribuição da licença do OneDrive</span><span class="sxs-lookup"><span data-stu-id="469ee-164">OneDrive License Assign Date</span></span>
- <span data-ttu-id="469ee-165">Data de atribuição da licença do SharePoint</span><span class="sxs-lookup"><span data-stu-id="469ee-165">SharePoint License Assign Date</span></span>
- <span data-ttu-id="469ee-166">Data de atribuição da licença do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="469ee-166">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="469ee-167">Data de atribuição da licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="469ee-167">Yammer License Assign Date</span></span>
- <span data-ttu-id="469ee-168">Data de atribuição da licença do Teams</span><span class="sxs-lookup"><span data-stu-id="469ee-168">Teams License Assign Date</span></span>
- <span data-ttu-id="469ee-169">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="469ee-169">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="469ee-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="469ee-170">Example</span></span>

#### <a name="request"></a><span data-ttu-id="469ee-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="469ee-171">Request</span></span>

<span data-ttu-id="469ee-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="469ee-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="469ee-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="469ee-173">Response</span></span>

<span data-ttu-id="469ee-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="469ee-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="469ee-175">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="469ee-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
```
