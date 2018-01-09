# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="ee344-101">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="ee344-101">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="ee344-102">Obtenha a contagem de usuários ativos diários no período de relatório por produto.</span><span class="sxs-lookup"><span data-stu-id="ee344-102">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="ee344-103">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos]((https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)).</span><span class="sxs-lookup"><span data-stu-id="ee344-103">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users]((https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)).</span></span>

## <a name="permissions"></a><span data-ttu-id="ee344-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee344-104">Permissions</span></span>

<span data-ttu-id="ee344-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ee344-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="ee344-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee344-107">Permission type</span></span>                        | <span data-ttu-id="ee344-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee344-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ee344-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee344-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee344-110">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee344-110">Not supported.</span></span>                           |
| <span data-ttu-id="ee344-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee344-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee344-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee344-112">Not supported.</span></span>                           |
| <span data-ttu-id="ee344-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee344-113">Application</span></span>                            | <span data-ttu-id="ee344-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee344-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ee344-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee344-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="ee344-116">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="ee344-116">Request parameters</span></span>

<span data-ttu-id="ee344-117">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="ee344-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="ee344-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ee344-118">Parameter</span></span> | <span data-ttu-id="ee344-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee344-119">Type</span></span>   | <span data-ttu-id="ee344-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee344-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ee344-121">ponto</span><span class="sxs-lookup"><span data-stu-id="ee344-121">Period</span></span>    | <span data-ttu-id="ee344-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee344-122">string</span></span> | <span data-ttu-id="ee344-123">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ee344-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ee344-124">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="ee344-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ee344-125">Esses valores seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ee344-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ee344-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee344-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ee344-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee344-127">Request headers</span></span>

| <span data-ttu-id="ee344-128">Nome</span><span class="sxs-lookup"><span data-stu-id="ee344-128">Name</span></span>          | <span data-ttu-id="ee344-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee344-129">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ee344-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee344-130">Authorization</span></span> | <span data-ttu-id="ee344-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee344-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ee344-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee344-133">Response</span></span>

<span data-ttu-id="ee344-134">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="ee344-134">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ee344-135">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="ee344-135">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ee344-136">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ee344-136">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="ee344-137">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="ee344-137">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ee344-138">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="ee344-138">Report Refresh Date</span></span>
- <span data-ttu-id="ee344-139">Office 365</span><span class="sxs-lookup"><span data-stu-id="ee344-139">Office 365</span></span>
- <span data-ttu-id="ee344-140">Exchange</span><span class="sxs-lookup"><span data-stu-id="ee344-140">Exchange</span></span>
- <span data-ttu-id="ee344-141">OneDrive</span><span class="sxs-lookup"><span data-stu-id="ee344-141">OneDrive</span></span>
- <span data-ttu-id="ee344-142">SharePoint</span><span class="sxs-lookup"><span data-stu-id="ee344-142">SharePoint</span></span>
- <span data-ttu-id="ee344-143">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="ee344-143">Skype for Business</span></span> 
- <span data-ttu-id="ee344-144">Yammer</span><span class="sxs-lookup"><span data-stu-id="ee344-144">Yammer Integration</span></span>
- <span data-ttu-id="ee344-145">Teams</span><span class="sxs-lookup"><span data-stu-id="ee344-145">Teams app</span></span>
- <span data-ttu-id="ee344-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="ee344-146">Report Date</span></span>
- <span data-ttu-id="ee344-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="ee344-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ee344-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee344-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ee344-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee344-149">Request</span></span>

<span data-ttu-id="ee344-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee344-150">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="ee344-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee344-151">Response</span></span>

<span data-ttu-id="ee344-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ee344-152">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ee344-153">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="ee344-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```
