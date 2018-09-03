# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="b3d32-101">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="b3d32-101">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

<span data-ttu-id="b3d32-102">Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="b3d32-102">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3d32-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3d32-103">Permissions</span></span>

<span data-ttu-id="b3d32-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b3d32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="b3d32-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3d32-106">Permission type</span></span>                        | <span data-ttu-id="b3d32-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3d32-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b3d32-108">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3d32-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3d32-109">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3d32-109">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b3d32-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3d32-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3d32-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3d32-111">Not supported.</span></span>                           |
| <span data-ttu-id="b3d32-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3d32-112">Application</span></span>                            | <span data-ttu-id="b3d32-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3d32-113">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b3d32-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3d32-114">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='{period_value}')
GET /reports/getTeamsDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="b3d32-115">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b3d32-115">Function parameters</span></span>

<span data-ttu-id="b3d32-116">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b3d32-116">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b3d32-117">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b3d32-117">Parameter</span></span> | <span data-ttu-id="b3d32-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3d32-118">Type</span></span>   | <span data-ttu-id="b3d32-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3d32-119">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b3d32-120">ponto</span><span class="sxs-lookup"><span data-stu-id="b3d32-120">period</span></span>    | <span data-ttu-id="b3d32-121">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3d32-121">string</span></span> | <span data-ttu-id="b3d32-122">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b3d32-122">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b3d32-123">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="b3d32-123">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b3d32-124">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b3d32-124">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b3d32-125">data</span><span class="sxs-lookup"><span data-stu-id="b3d32-125">date</span></span>      | <span data-ttu-id="b3d32-126">Data</span><span class="sxs-lookup"><span data-stu-id="b3d32-126">Date</span></span>   | <span data-ttu-id="b3d32-127">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="b3d32-127">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b3d32-128">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="b3d32-128">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b3d32-129">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="b3d32-129">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b3d32-130">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="b3d32-130">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3d32-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3d32-131">Request headers</span></span>

| <span data-ttu-id="b3d32-132">Nome</span><span class="sxs-lookup"><span data-stu-id="b3d32-132">Name</span></span>          | <span data-ttu-id="b3d32-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3d32-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b3d32-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3d32-134">Authorization</span></span> | <span data-ttu-id="b3d32-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3d32-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b3d32-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3d32-137">Response</span></span>

<span data-ttu-id="b3d32-138">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="b3d32-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b3d32-139">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="b3d32-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b3d32-140">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b3d32-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b3d32-141">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="b3d32-141">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="b3d32-142">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="b3d32-142">Report Refresh Date</span></span>
- <span data-ttu-id="b3d32-143">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="b3d32-143">User Principal Name</span></span>
- <span data-ttu-id="b3d32-144">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="b3d32-144">Last Activity Date</span></span>
- <span data-ttu-id="b3d32-145">Excluído</span><span class="sxs-lookup"><span data-stu-id="b3d32-145">Is Deleted</span></span>
- <span data-ttu-id="b3d32-146">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="b3d32-146">Deleted Date</span></span>
- <span data-ttu-id="b3d32-147">Usou Web</span><span class="sxs-lookup"><span data-stu-id="b3d32-147">Used Web</span></span>
- <span data-ttu-id="b3d32-148">Usou Windows Phone</span><span class="sxs-lookup"><span data-stu-id="b3d32-148">Used Windows Phone</span></span>
- <span data-ttu-id="b3d32-149">Usou iOS</span><span class="sxs-lookup"><span data-stu-id="b3d32-149">Used iOS</span></span>
- <span data-ttu-id="b3d32-150">Usou Mac</span><span class="sxs-lookup"><span data-stu-id="b3d32-150">Used Mac</span></span>
- <span data-ttu-id="b3d32-151">Usou telefone Android</span><span class="sxs-lookup"><span data-stu-id="b3d32-151">Used Android Phone</span></span>
- <span data-ttu-id="b3d32-152">Usou Windows</span><span class="sxs-lookup"><span data-stu-id="b3d32-152">Used Windows</span></span>
- <span data-ttu-id="b3d32-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="b3d32-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b3d32-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3d32-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b3d32-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3d32-155">Request</span></span>

<span data-ttu-id="b3d32-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3d32-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b3d32-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3d32-157">Response</span></span>

<span data-ttu-id="b3d32-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3d32-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="b3d32-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="b3d32-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
```
