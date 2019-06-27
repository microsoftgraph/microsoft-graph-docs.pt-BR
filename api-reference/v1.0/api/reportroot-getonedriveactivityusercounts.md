---
title: 'reportRoot: getOneDriveActivityUserCounts'
description: Obtenha a tendência no número de usuários ativos do OneDrive.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e99eb661c9abee6ea7156d7c60d6aab22bd52bde
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268576"
---
# <a name="reportroot-getonedriveactivityusercounts"></a><span data-ttu-id="e0bed-103">reportRoot: getOneDriveActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="e0bed-103">reportRoot: getOneDriveActivityUserCounts</span></span>

<span data-ttu-id="e0bed-104">Obtenha a tendência no número de usuários ativos do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e0bed-104">Get the trend in the number of active OneDrive users.</span></span>

> <span data-ttu-id="e0bed-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="e0bed-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="e0bed-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0bed-106">Permissions</span></span>

<span data-ttu-id="e0bed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0bed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0bed-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0bed-109">Permission type</span></span>                        | <span data-ttu-id="e0bed-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0bed-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e0bed-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0bed-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0bed-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0bed-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e0bed-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0bed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0bed-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0bed-114">Not supported.</span></span>                           |
| <span data-ttu-id="e0bed-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0bed-115">Application</span></span>                            | <span data-ttu-id="e0bed-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0bed-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e0bed-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0bed-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e0bed-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e0bed-118">Function parameters</span></span>

<span data-ttu-id="e0bed-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="e0bed-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e0bed-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e0bed-120">Parameter</span></span> | <span data-ttu-id="e0bed-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0bed-121">Type</span></span>   | <span data-ttu-id="e0bed-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0bed-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e0bed-123">ponto</span><span class="sxs-lookup"><span data-stu-id="e0bed-123">period</span></span>    | <span data-ttu-id="e0bed-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0bed-124">string</span></span> | <span data-ttu-id="e0bed-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e0bed-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e0bed-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="e0bed-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e0bed-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e0bed-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e0bed-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0bed-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e0bed-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0bed-129">Request headers</span></span>

| <span data-ttu-id="e0bed-130">Nome</span><span class="sxs-lookup"><span data-stu-id="e0bed-130">Name</span></span>          | <span data-ttu-id="e0bed-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0bed-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e0bed-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0bed-132">Authorization</span></span> | <span data-ttu-id="e0bed-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0bed-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e0bed-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e0bed-135">If-None-Match</span></span> | <span data-ttu-id="e0bed-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="e0bed-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e0bed-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e0bed-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e0bed-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0bed-138">Response</span></span>

<span data-ttu-id="e0bed-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="e0bed-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e0bed-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="e0bed-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e0bed-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e0bed-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e0bed-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="e0bed-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e0bed-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="e0bed-143">Report Refresh Date</span></span>
- <span data-ttu-id="e0bed-144">Exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="e0bed-144">Viewed Or Edited</span></span>
- <span data-ttu-id="e0bed-145">Sincronizados</span><span class="sxs-lookup"><span data-stu-id="e0bed-145">Synced</span></span>
- <span data-ttu-id="e0bed-146">Compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="e0bed-146">Shared Internally</span></span>
- <span data-ttu-id="e0bed-147">Compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="e0bed-147">Shared Externally</span></span>
- <span data-ttu-id="e0bed-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="e0bed-148">Report Date</span></span>
- <span data-ttu-id="e0bed-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="e0bed-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="e0bed-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0bed-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e0bed-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0bed-151">Request</span></span>

<span data-ttu-id="e0bed-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0bed-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="e0bed-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0bed-153">Response</span></span>

<span data-ttu-id="e0bed-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e0bed-154">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e0bed-155">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="e0bed-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e0bed-156">C#</span><span class="sxs-lookup"><span data-stu-id="e0bed-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0bed-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="e0bed-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityusercounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e0bed-158">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e0bed-158">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityusercounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="e0bed-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="e0bed-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getonedriveactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getonedriveactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getonedriveactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
