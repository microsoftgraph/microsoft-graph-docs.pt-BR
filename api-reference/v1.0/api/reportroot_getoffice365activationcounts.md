# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="d962b-101">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="d962b-101">reportRoot: getOffice365ActivationCounts</span></span>

<span data-ttu-id="d962b-102">Obtenha a contagem de ativações do Office 365 em desktops e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="d962b-102">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="d962b-103">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="d962b-103">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="d962b-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="d962b-104">Permissions</span></span>

<span data-ttu-id="d962b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d962b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="d962b-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d962b-107">Permission type</span></span>                        | <span data-ttu-id="d962b-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d962b-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d962b-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d962b-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="d962b-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d962b-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d962b-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d962b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d962b-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d962b-112">Not supported.</span></span>                           |
| <span data-ttu-id="d962b-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d962b-113">Application</span></span>                            | <span data-ttu-id="d962b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d962b-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d962b-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d962b-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="request-headers"></a><span data-ttu-id="d962b-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d962b-116">Request headers</span></span>

| <span data-ttu-id="d962b-117">Nome</span><span class="sxs-lookup"><span data-stu-id="d962b-117">Name</span></span>          | <span data-ttu-id="d962b-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="d962b-118">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d962b-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="d962b-119">Authorization</span></span> | <span data-ttu-id="d962b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d962b-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d962b-122">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d962b-122">If-None-Match</span></span> | <span data-ttu-id="d962b-123">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="d962b-123">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d962b-124">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d962b-124">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d962b-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="d962b-125">Response</span></span>

<span data-ttu-id="d962b-126">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d962b-126">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d962b-127">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d962b-127">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d962b-128">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d962b-128">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d962b-129">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d962b-129">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d962b-130">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d962b-130">Report Refresh Date</span></span>
- <span data-ttu-id="d962b-131">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="d962b-131">Product Type</span></span>
- <span data-ttu-id="d962b-132">Windows</span><span class="sxs-lookup"><span data-stu-id="d962b-132">Windows</span></span>
- <span data-ttu-id="d962b-133">Mac</span><span class="sxs-lookup"><span data-stu-id="d962b-133">Mac</span></span>
- <span data-ttu-id="d962b-134">Android</span><span class="sxs-lookup"><span data-stu-id="d962b-134">Android</span></span>
- <span data-ttu-id="d962b-135">iOS</span><span class="sxs-lookup"><span data-stu-id="d962b-135">iOS</span></span>
- <span data-ttu-id="d962b-136">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="d962b-136">Windows 10 Mobile</span></span>

## <a name="example"></a><span data-ttu-id="d962b-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d962b-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d962b-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d962b-138">Request</span></span>

<span data-ttu-id="d962b-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d962b-139">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationCounts
```

#### <a name="response"></a><span data-ttu-id="d962b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d962b-140">Response</span></span>

<span data-ttu-id="d962b-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d962b-141">The following is an example of the response.</span></span>

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

<span data-ttu-id="d962b-142">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d962b-142">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
```
