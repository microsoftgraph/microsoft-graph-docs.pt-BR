# <a name="reportroot-getoffice365groupsactivitystorage"></a><span data-ttu-id="a4275-101">reportRoot: getOffice365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="a4275-101">reportRoot: getOffice365GroupsActivityStorage</span></span>

<span data-ttu-id="a4275-102">Obtenha o armazenamento total usado em todas as caixas de correio de grupo e sites de grupo.</span><span class="sxs-lookup"><span data-stu-id="a4275-102">Get the total storage used across all group mailboxes and group sites.</span></span>

> <span data-ttu-id="a4275-103">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="a4275-103">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="a4275-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4275-104">Permissions</span></span>

<span data-ttu-id="a4275-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a4275-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="a4275-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4275-107">Permission type</span></span>                        | <span data-ttu-id="a4275-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4275-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a4275-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4275-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="a4275-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4275-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a4275-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4275-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4275-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4275-112">Not supported.</span></span>                           |
| <span data-ttu-id="a4275-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4275-113">Application</span></span>                            | <span data-ttu-id="a4275-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4275-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a4275-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4275-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a4275-116">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="a4275-116">Function parameters</span></span>

<span data-ttu-id="a4275-117">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a4275-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a4275-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a4275-118">Parameter</span></span> | <span data-ttu-id="a4275-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4275-119">Type</span></span>   | <span data-ttu-id="a4275-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4275-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a4275-121">ponto</span><span class="sxs-lookup"><span data-stu-id="a4275-121">period</span></span>    | <span data-ttu-id="a4275-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4275-122">string</span></span> | <span data-ttu-id="a4275-123">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a4275-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a4275-124">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="a4275-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a4275-125">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a4275-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a4275-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4275-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="a4275-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4275-127">Request headers</span></span>

| <span data-ttu-id="a4275-128">Nome</span><span class="sxs-lookup"><span data-stu-id="a4275-128">Name</span></span>          | <span data-ttu-id="a4275-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4275-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="a4275-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4275-130">Authorization</span></span> | <span data-ttu-id="a4275-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4275-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="a4275-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a4275-133">If-None-Match</span></span> | <span data-ttu-id="a4275-134">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="a4275-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="a4275-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a4275-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a4275-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4275-136">Response</span></span>

<span data-ttu-id="a4275-137">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="a4275-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a4275-138">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="a4275-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a4275-139">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a4275-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a4275-140">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="a4275-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a4275-141">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="a4275-141">Report Refresh Date</span></span>
- <span data-ttu-id="a4275-142">Armazenamento de caixa de correio utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="a4275-142">Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="a4275-143">Armazenamento de site utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="a4275-143">Site Storage Used (Byte)</span></span>
- <span data-ttu-id="a4275-144">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="a4275-144">Report Date</span></span>
- <span data-ttu-id="a4275-145">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="a4275-145">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="a4275-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4275-146">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a4275-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4275-147">Request</span></span>

<span data-ttu-id="a4275-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4275-148">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivitystorage"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityStorage(period='D7')
```

#### <a name="response"></a><span data-ttu-id="a4275-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4275-149">Response</span></span>

<span data-ttu-id="a4275-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a4275-150">The following is an example of the response.</span></span>

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

<span data-ttu-id="a4275-151">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="a4275-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mailbox Storage Used (Byte),Site Storage Used (Byte),Report Date,Report Period
```
