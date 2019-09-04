---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: Obtenha dados sobre o uso do OneDrive por conta.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0d08c2b86030f7ca0b4bdff83f99e5e5f6a6179e
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728108"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="eab2d-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="eab2d-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

<span data-ttu-id="eab2d-104">Obtenha dados sobre o uso do OneDrive por conta.</span><span class="sxs-lookup"><span data-stu-id="eab2d-104">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="eab2d-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="eab2d-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="eab2d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eab2d-106">Permissions</span></span>

<span data-ttu-id="eab2d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eab2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eab2d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eab2d-109">Permission type</span></span>                        | <span data-ttu-id="eab2d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eab2d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="eab2d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eab2d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="eab2d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="eab2d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="eab2d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eab2d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eab2d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eab2d-114">Not supported.</span></span>                           |
| <span data-ttu-id="eab2d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eab2d-115">Application</span></span>                            | <span data-ttu-id="eab2d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="eab2d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="eab2d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eab2d-117">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="eab2d-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="eab2d-118">Function parameters</span></span>

<span data-ttu-id="eab2d-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="eab2d-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="eab2d-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="eab2d-120">Parameter</span></span> | <span data-ttu-id="eab2d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="eab2d-121">Type</span></span>   | <span data-ttu-id="eab2d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="eab2d-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="eab2d-123">ponto</span><span class="sxs-lookup"><span data-stu-id="eab2d-123">period</span></span>    | <span data-ttu-id="eab2d-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eab2d-124">string</span></span> | <span data-ttu-id="eab2d-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="eab2d-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="eab2d-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="eab2d-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="eab2d-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="eab2d-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="eab2d-128">data</span><span class="sxs-lookup"><span data-stu-id="eab2d-128">date</span></span>      | <span data-ttu-id="eab2d-129">Data</span><span class="sxs-lookup"><span data-stu-id="eab2d-129">Date</span></span>   | <span data-ttu-id="eab2d-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="eab2d-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="eab2d-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="eab2d-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="eab2d-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="eab2d-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="eab2d-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="eab2d-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eab2d-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eab2d-134">Request headers</span></span>

| <span data-ttu-id="eab2d-135">Nome</span><span class="sxs-lookup"><span data-stu-id="eab2d-135">Name</span></span>          | <span data-ttu-id="eab2d-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="eab2d-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="eab2d-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="eab2d-137">Authorization</span></span> | <span data-ttu-id="eab2d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eab2d-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="eab2d-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="eab2d-140">If-None-Match</span></span> | <span data-ttu-id="eab2d-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="eab2d-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="eab2d-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="eab2d-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="eab2d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="eab2d-143">Response</span></span>

<span data-ttu-id="eab2d-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="eab2d-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="eab2d-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="eab2d-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="eab2d-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="eab2d-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="eab2d-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="eab2d-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="eab2d-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="eab2d-148">Report Refresh Date</span></span>
- <span data-ttu-id="eab2d-149">URL do site</span><span class="sxs-lookup"><span data-stu-id="eab2d-149">Site URL</span></span>
- <span data-ttu-id="eab2d-150">Nome de exibição do proprietário</span><span class="sxs-lookup"><span data-stu-id="eab2d-150">Owner Display Name</span></span>
- <span data-ttu-id="eab2d-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="eab2d-151">Is Deleted</span></span>
- <span data-ttu-id="eab2d-152">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="eab2d-152">Last Activity Date</span></span>
- <span data-ttu-id="eab2d-153">Contagem de arquivos</span><span class="sxs-lookup"><span data-stu-id="eab2d-153">File Count</span></span>
- <span data-ttu-id="eab2d-154">Contagem de arquivos ativos</span><span class="sxs-lookup"><span data-stu-id="eab2d-154">Active File Count</span></span>
- <span data-ttu-id="eab2d-155">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="eab2d-155">Storage Used (Byte)</span></span>
- <span data-ttu-id="eab2d-156">Armazenamento alocado (bytes)</span><span class="sxs-lookup"><span data-stu-id="eab2d-156">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="eab2d-157">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="eab2d-157">Owner Principal Name</span></span>
- <span data-ttu-id="eab2d-158">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="eab2d-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="eab2d-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eab2d-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="eab2d-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eab2d-160">Request</span></span>

<span data-ttu-id="eab2d-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eab2d-161">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="eab2d-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="eab2d-162">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eab2d-163">C#</span><span class="sxs-lookup"><span data-stu-id="eab2d-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eab2d-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eab2d-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eab2d-165">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="eab2d-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="eab2d-166">Java</span><span class="sxs-lookup"><span data-stu-id="eab2d-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="eab2d-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="eab2d-167">Response</span></span>

<span data-ttu-id="eab2d-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eab2d-168">The following is an example of the response.</span></span>

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

<span data-ttu-id="eab2d-169">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="eab2d-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Owner Principal Name,Report Period
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
