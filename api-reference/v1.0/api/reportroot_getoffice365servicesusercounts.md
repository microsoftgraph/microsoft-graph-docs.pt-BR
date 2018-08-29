# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="56288-101">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="56288-101">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="56288-102">Obtenha a contagem de usuários por tipo de atividade e serviço.</span><span class="sxs-lookup"><span data-stu-id="56288-102">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="56288-103">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="56288-103">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="56288-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="56288-104">Permissions</span></span>

<span data-ttu-id="56288-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="56288-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="56288-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56288-107">Permission type</span></span>                        | <span data-ttu-id="56288-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56288-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="56288-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56288-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="56288-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="56288-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="56288-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56288-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56288-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56288-112">Not supported.</span></span>                           |
| <span data-ttu-id="56288-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56288-113">Application</span></span>                            | <span data-ttu-id="56288-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="56288-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="56288-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56288-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="56288-116">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="56288-116">Request parameters</span></span>

<span data-ttu-id="56288-117">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="56288-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="56288-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="56288-118">Parameter</span></span> | <span data-ttu-id="56288-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="56288-119">Type</span></span>   | <span data-ttu-id="56288-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="56288-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="56288-121">ponto</span><span class="sxs-lookup"><span data-stu-id="56288-121">period</span></span>    | <span data-ttu-id="56288-122">string</span><span class="sxs-lookup"><span data-stu-id="56288-122">string</span></span> | <span data-ttu-id="56288-123">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="56288-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="56288-124">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="56288-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="56288-125">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="56288-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="56288-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56288-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="56288-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56288-127">Request headers</span></span>

| <span data-ttu-id="56288-128">Nome</span><span class="sxs-lookup"><span data-stu-id="56288-128">Name</span></span>          | <span data-ttu-id="56288-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="56288-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="56288-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="56288-130">Authorization</span></span> | <span data-ttu-id="56288-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56288-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="56288-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="56288-133">If-None-Match</span></span> | <span data-ttu-id="56288-134">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="56288-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="56288-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="56288-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="56288-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="56288-136">Response</span></span>

<span data-ttu-id="56288-137">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="56288-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="56288-138">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="56288-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="56288-139">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="56288-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="56288-140">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="56288-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="56288-141">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="56288-141">Report Refresh Date</span></span>
- <span data-ttu-id="56288-142">Exchange ativo</span><span class="sxs-lookup"><span data-stu-id="56288-142">Exchange Active</span></span>
- <span data-ttu-id="56288-143">Exchange inativo</span><span class="sxs-lookup"><span data-stu-id="56288-143">Exchange Inactive</span></span>
- <span data-ttu-id="56288-144">OneDrive ativo</span><span class="sxs-lookup"><span data-stu-id="56288-144">OneDrive Active</span></span>
- <span data-ttu-id="56288-145">OneDrive inativo</span><span class="sxs-lookup"><span data-stu-id="56288-145">OneDrive Inactive</span></span>
- <span data-ttu-id="56288-146">SharePoint ativo</span><span class="sxs-lookup"><span data-stu-id="56288-146">SharePoint Active</span></span>
- <span data-ttu-id="56288-147">SharePoint inativo</span><span class="sxs-lookup"><span data-stu-id="56288-147">SharePoint Inactive</span></span>
- <span data-ttu-id="56288-148">Skype for Business ativo</span><span class="sxs-lookup"><span data-stu-id="56288-148">Skype For Business Active</span></span>
- <span data-ttu-id="56288-149">Skype for Business inativo</span><span class="sxs-lookup"><span data-stu-id="56288-149">Skype For Business Inactive</span></span>
- <span data-ttu-id="56288-150">Yammer ativa</span><span class="sxs-lookup"><span data-stu-id="56288-150">Yammer Active</span></span>
- <span data-ttu-id="56288-151">Yammer inativa</span><span class="sxs-lookup"><span data-stu-id="56288-151">Yammer Inactive</span></span>
- <span data-ttu-id="56288-152">Teams ativo</span><span class="sxs-lookup"><span data-stu-id="56288-152">Teams Active</span></span>
- <span data-ttu-id="56288-153">Teams inativo</span><span class="sxs-lookup"><span data-stu-id="56288-153">Teams Inactive</span></span>
- <span data-ttu-id="56288-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="56288-154">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="56288-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56288-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="56288-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56288-156">Request</span></span>

<span data-ttu-id="56288-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="56288-157">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365servicesusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ServicesUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="56288-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="56288-158">Response</span></span>

<span data-ttu-id="56288-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="56288-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="56288-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="56288-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Report Period
```
