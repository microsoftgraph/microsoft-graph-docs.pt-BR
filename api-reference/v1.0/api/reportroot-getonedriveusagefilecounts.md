---
title: 'reportRoot: getOneDriveUsageFileCounts'
description: Obtenha o número total de arquivos em todos os sites e quantos são arquivos ativos. Um arquivo é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0aca7eec4c4991484a3ec4ab6a3a301b704e2144
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021904"
---
# <a name="reportroot-getonedriveusagefilecounts"></a><span data-ttu-id="aa4f7-104">reportRoot: getOneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="aa4f7-104">reportRoot: getOneDriveUsageFileCounts</span></span>

<span data-ttu-id="aa4f7-105">Obtenha o número total de arquivos em todos os sites e quantos são arquivos ativos.</span><span class="sxs-lookup"><span data-stu-id="aa4f7-105">Get the total number of files across all sites and how many are active files.</span></span> <span data-ttu-id="aa4f7-106">Um arquivo é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="aa4f7-106">A file is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="aa4f7-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="aa4f7-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="aa4f7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa4f7-108">Permissions</span></span>

<span data-ttu-id="aa4f7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa4f7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aa4f7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa4f7-111">Permission type</span></span>                        | <span data-ttu-id="aa4f7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa4f7-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="aa4f7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa4f7-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="aa4f7-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa4f7-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="aa4f7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa4f7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa4f7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa4f7-116">Not supported.</span></span>                           |
| <span data-ttu-id="aa4f7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa4f7-117">Application</span></span>                            | <span data-ttu-id="aa4f7-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa4f7-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="aa4f7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa4f7-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="aa4f7-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa4f7-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="aa4f7-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="aa4f7-121">Function parameters</span></span>

<span data-ttu-id="aa4f7-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="aa4f7-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="aa4f7-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="aa4f7-123">Parameter</span></span> | <span data-ttu-id="aa4f7-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa4f7-124">Type</span></span>   | <span data-ttu-id="aa4f7-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa4f7-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="aa4f7-126">ponto</span><span class="sxs-lookup"><span data-stu-id="aa4f7-126">period</span></span>    | <span data-ttu-id="aa4f7-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa4f7-127">string</span></span> | <span data-ttu-id="aa4f7-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="aa4f7-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="aa4f7-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="aa4f7-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="aa4f7-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="aa4f7-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="aa4f7-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa4f7-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="aa4f7-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa4f7-132">Request headers</span></span>

| <span data-ttu-id="aa4f7-133">Nome</span><span class="sxs-lookup"><span data-stu-id="aa4f7-133">Name</span></span>          | <span data-ttu-id="aa4f7-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa4f7-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="aa4f7-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa4f7-135">Authorization</span></span> | <span data-ttu-id="aa4f7-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa4f7-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="aa4f7-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="aa4f7-138">If-None-Match</span></span> | <span data-ttu-id="aa4f7-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="aa4f7-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="aa4f7-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="aa4f7-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="aa4f7-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa4f7-141">Response</span></span>

<span data-ttu-id="aa4f7-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="aa4f7-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="aa4f7-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="aa4f7-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="aa4f7-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="aa4f7-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="aa4f7-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="aa4f7-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="aa4f7-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="aa4f7-146">Report Refresh Date</span></span>
- <span data-ttu-id="aa4f7-147">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="aa4f7-147">Site Type</span></span>
- <span data-ttu-id="aa4f7-148">Total</span><span class="sxs-lookup"><span data-stu-id="aa4f7-148">Total</span></span>
- <span data-ttu-id="aa4f7-149">Ativo</span><span class="sxs-lookup"><span data-stu-id="aa4f7-149">Active</span></span>
- <span data-ttu-id="aa4f7-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="aa4f7-150">Report Date</span></span>
- <span data-ttu-id="aa4f7-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="aa4f7-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="aa4f7-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa4f7-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="aa4f7-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa4f7-153">Request</span></span>

<span data-ttu-id="aa4f7-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa4f7-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusagefilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageFileCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aa4f7-155">C#</span><span class="sxs-lookup"><span data-stu-id="aa4f7-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusagefilecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aa4f7-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="aa4f7-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusagefilecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aa4f7-157">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="aa4f7-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusagefilecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="aa4f7-158">Java</span><span class="sxs-lookup"><span data-stu-id="aa4f7-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveusagefilecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aa4f7-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa4f7-159">Response</span></span>

<span data-ttu-id="aa4f7-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aa4f7-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="aa4f7-161">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="aa4f7-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
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
