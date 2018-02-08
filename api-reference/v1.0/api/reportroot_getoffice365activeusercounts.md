# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="d70f4-101">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="d70f4-101">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="d70f4-102">Obtenha a contagem de usuários ativos diários no período de relatório por produto.</span><span class="sxs-lookup"><span data-stu-id="d70f4-102">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="d70f4-103">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="d70f4-103">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="d70f4-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="d70f4-104">Permissions</span></span>

<span data-ttu-id="d70f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d70f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="d70f4-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d70f4-107">Permission type</span></span>                        | <span data-ttu-id="d70f4-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d70f4-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d70f4-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d70f4-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="d70f4-110">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d70f4-110">Not supported.</span></span>                           |
| <span data-ttu-id="d70f4-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d70f4-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d70f4-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d70f4-112">Not supported.</span></span>                           |
| <span data-ttu-id="d70f4-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d70f4-113">Application</span></span>                            | <span data-ttu-id="d70f4-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d70f4-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d70f4-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d70f4-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="d70f4-116">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="d70f4-116">Request parameters</span></span>

<span data-ttu-id="d70f4-117">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d70f4-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="d70f4-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d70f4-118">Parameter</span></span> | <span data-ttu-id="d70f4-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d70f4-119">Type</span></span>   | <span data-ttu-id="d70f4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d70f4-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d70f4-121">ponto</span><span class="sxs-lookup"><span data-stu-id="d70f4-121">period</span></span>    | <span data-ttu-id="d70f4-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d70f4-122">string</span></span> | <span data-ttu-id="d70f4-123">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d70f4-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d70f4-124">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="d70f4-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d70f4-125">Esses valores seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d70f4-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d70f4-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d70f4-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d70f4-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d70f4-127">Request headers</span></span>

| <span data-ttu-id="d70f4-128">Nome</span><span class="sxs-lookup"><span data-stu-id="d70f4-128">Name</span></span>          | <span data-ttu-id="d70f4-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="d70f4-129">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d70f4-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="d70f4-130">Authorization</span></span> | <span data-ttu-id="d70f4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d70f4-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d70f4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d70f4-133">Response</span></span>

<span data-ttu-id="d70f4-134">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d70f4-134">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d70f4-135">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d70f4-135">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d70f4-136">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d70f4-136">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d70f4-137">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d70f4-137">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d70f4-138">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d70f4-138">Report Refresh Date</span></span>
- <span data-ttu-id="d70f4-139">Office 365</span><span class="sxs-lookup"><span data-stu-id="d70f4-139">Office 365</span></span>
- <span data-ttu-id="d70f4-140">Exchange</span><span class="sxs-lookup"><span data-stu-id="d70f4-140">Exchange</span></span>
- <span data-ttu-id="d70f4-141">OneDrive</span><span class="sxs-lookup"><span data-stu-id="d70f4-141">OneDrive</span></span>
- <span data-ttu-id="d70f4-142">SharePoint</span><span class="sxs-lookup"><span data-stu-id="d70f4-142">SharePoint</span></span>
- <span data-ttu-id="d70f4-143">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="d70f4-143">Skype For Business</span></span> 
- <span data-ttu-id="d70f4-144">Yammer</span><span class="sxs-lookup"><span data-stu-id="d70f4-144">Yammer</span></span>
- <span data-ttu-id="d70f4-145">Teams</span><span class="sxs-lookup"><span data-stu-id="d70f4-145">Teams</span></span>
- <span data-ttu-id="d70f4-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="d70f4-146">Report Date</span></span>
- <span data-ttu-id="d70f4-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="d70f4-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="d70f4-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d70f4-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d70f4-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d70f4-149">Request</span></span>

<span data-ttu-id="d70f4-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d70f4-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="d70f4-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d70f4-151">Response</span></span>

<span data-ttu-id="d70f4-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d70f4-152">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d70f4-153">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d70f4-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
