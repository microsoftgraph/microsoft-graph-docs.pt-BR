---
title: 'reportRoot: getSharePointSiteUsageStorage'
description: Obtenha a tendência de armazenamento alocado e consumido durante o período de relatório.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 37bfab80a4589aa9e720da24f1ad81610fe95181
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893346"
---
# <a name="reportroot-getsharepointsiteusagestorage"></a><span data-ttu-id="58053-103">reportRoot: getSharePointSiteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="58053-103">reportRoot: getSharePointSiteUsageStorage</span></span>

<span data-ttu-id="58053-104">Obtenha a tendência de armazenamento alocado e consumido durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="58053-104">Get the trend of storage allocated and consumed during the reporting period.</span></span>

> <span data-ttu-id="58053-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="58053-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="58053-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="58053-106">Permissions</span></span>

<span data-ttu-id="58053-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58053-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="58053-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58053-109">Permission type</span></span>                        | <span data-ttu-id="58053-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58053-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="58053-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58053-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="58053-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="58053-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="58053-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58053-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58053-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58053-114">Not supported.</span></span>                           |
| <span data-ttu-id="58053-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58053-115">Application</span></span>                            | <span data-ttu-id="58053-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="58053-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="58053-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58053-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="58053-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="58053-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="58053-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="58053-119">Function parameters</span></span>

<span data-ttu-id="58053-120">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="58053-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="58053-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="58053-121">Parameter</span></span> | <span data-ttu-id="58053-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="58053-122">Type</span></span>   | <span data-ttu-id="58053-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="58053-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="58053-124">ponto</span><span class="sxs-lookup"><span data-stu-id="58053-124">period</span></span>    | <span data-ttu-id="58053-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58053-125">string</span></span> | <span data-ttu-id="58053-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="58053-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="58053-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="58053-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="58053-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="58053-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="58053-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58053-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="58053-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58053-130">Request headers</span></span>

| <span data-ttu-id="58053-131">Nome</span><span class="sxs-lookup"><span data-stu-id="58053-131">Name</span></span>          | <span data-ttu-id="58053-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="58053-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="58053-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="58053-133">Authorization</span></span> | <span data-ttu-id="58053-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58053-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="58053-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="58053-136">If-None-Match</span></span> | <span data-ttu-id="58053-137">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="58053-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="58053-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="58053-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="58053-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="58053-139">Response</span></span>

<span data-ttu-id="58053-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="58053-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="58053-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="58053-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="58053-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="58053-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="58053-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="58053-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="58053-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="58053-144">Report Refresh Date</span></span>
- <span data-ttu-id="58053-145">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="58053-145">Site Type</span></span>
- <span data-ttu-id="58053-146">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="58053-146">Storage Used (Byte)</span></span>
- <span data-ttu-id="58053-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="58053-147">Report Date</span></span>
- <span data-ttu-id="58053-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="58053-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="58053-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58053-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="58053-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58053-150">Request</span></span>

<span data-ttu-id="58053-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="58053-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagestorage"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageStorage(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="58053-152">C#</span><span class="sxs-lookup"><span data-stu-id="58053-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagestorage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="58053-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="58053-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagestorage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="58053-154">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="58053-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagestorage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="58053-155">Java</span><span class="sxs-lookup"><span data-stu-id="58053-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusagestorage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="58053-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="58053-156">Response</span></span>

<span data-ttu-id="58053-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="58053-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="58053-158">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="58053-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Storage Used (Byte),Report Date,Report Period
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
