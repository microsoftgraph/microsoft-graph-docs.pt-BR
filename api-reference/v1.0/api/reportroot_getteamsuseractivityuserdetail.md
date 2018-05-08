# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="b855e-101">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="b855e-101">reportRoot: getTeamsUserActivityUserDetail</span></span>

<span data-ttu-id="b855e-102">Obtém detalhes sobre a atividade de usuários do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="b855e-102">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="b855e-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="b855e-103">Permissions</span></span>

<span data-ttu-id="b855e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b855e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="b855e-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b855e-106">Permission type</span></span>                        | <span data-ttu-id="b855e-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b855e-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b855e-108">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b855e-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="b855e-109">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b855e-109">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b855e-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b855e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b855e-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b855e-111">Not supported.</span></span>                           |
| <span data-ttu-id="b855e-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b855e-112">Application</span></span>                            | <span data-ttu-id="b855e-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b855e-113">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b855e-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b855e-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='{period_value}')
GET /reports/getTeamsUserActivityUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="b855e-115">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="b855e-115">Request parameters</span></span>

<span data-ttu-id="b855e-116">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b855e-116">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b855e-117">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b855e-117">Parameter</span></span> | <span data-ttu-id="b855e-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="b855e-118">Type</span></span>   | <span data-ttu-id="b855e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b855e-119">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b855e-120">ponto</span><span class="sxs-lookup"><span data-stu-id="b855e-120">period</span></span>    | <span data-ttu-id="b855e-121">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b855e-121">string</span></span> | <span data-ttu-id="b855e-122">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b855e-122">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b855e-123">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="b855e-123">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b855e-124">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b855e-124">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b855e-125">data</span><span class="sxs-lookup"><span data-stu-id="b855e-125">date</span></span>      | <span data-ttu-id="b855e-126">Data</span><span class="sxs-lookup"><span data-stu-id="b855e-126">Date</span></span>   | <span data-ttu-id="b855e-127">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="b855e-127">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b855e-128">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="b855e-128">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b855e-129">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="b855e-129">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b855e-130">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="b855e-130">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b855e-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b855e-131">Request headers</span></span>

| <span data-ttu-id="b855e-132">Nome</span><span class="sxs-lookup"><span data-stu-id="b855e-132">Name</span></span>          | <span data-ttu-id="b855e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b855e-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b855e-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="b855e-134">Authorization</span></span> | <span data-ttu-id="b855e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b855e-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b855e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b855e-137">Response</span></span>

<span data-ttu-id="b855e-138">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="b855e-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b855e-139">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="b855e-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b855e-140">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b855e-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b855e-141">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="b855e-141">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="b855e-142">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="b855e-142">Report Refresh Date</span></span>
- <span data-ttu-id="b855e-143">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="b855e-143">User Principal Name</span></span>
- <span data-ttu-id="b855e-144">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="b855e-144">Last Activity Date</span></span>
- <span data-ttu-id="b855e-145">Excluído</span><span class="sxs-lookup"><span data-stu-id="b855e-145">Is Deleted</span></span>
- <span data-ttu-id="b855e-146">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="b855e-146">Deleted Date</span></span>
- <span data-ttu-id="b855e-147">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="b855e-147">Assigned Products</span></span>
- <span data-ttu-id="b855e-148">Número de mensagens de chat de equipe</span><span class="sxs-lookup"><span data-stu-id="b855e-148">Team Chat Message Count</span></span>
- <span data-ttu-id="b855e-149">Contagem de mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="b855e-149">Private Chat Message Count</span></span>
- <span data-ttu-id="b855e-150">Contagem de chamadas</span><span class="sxs-lookup"><span data-stu-id="b855e-150">Call Count</span></span>
- <span data-ttu-id="b855e-151">Contagem de reuniões</span><span class="sxs-lookup"><span data-stu-id="b855e-151">Meeting Count</span></span>
- <span data-ttu-id="b855e-152">Tem outra ação</span><span class="sxs-lookup"><span data-stu-id="b855e-152">Has Other Action</span></span>
- <span data-ttu-id="b855e-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="b855e-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b855e-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b855e-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b855e-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b855e-155">Request</span></span>

<span data-ttu-id="b855e-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b855e-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b855e-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b855e-157">Response</span></span>

<span data-ttu-id="b855e-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b855e-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b855e-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="b855e-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
```
