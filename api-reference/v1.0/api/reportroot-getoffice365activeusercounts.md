---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Obtenha a contagem de usuários ativos diários no período de relatório por produto.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9b79493e60ea6e9fdc24496ff39d73ebb3959109
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268695"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="a7ccf-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="a7ccf-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="a7ccf-104">Obtenha a contagem de usuários ativos diários no período de relatório por produto.</span><span class="sxs-lookup"><span data-stu-id="a7ccf-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="a7ccf-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="a7ccf-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="a7ccf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a7ccf-106">Permissions</span></span>

<span data-ttu-id="a7ccf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7ccf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a7ccf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7ccf-109">Permission type</span></span>                        | <span data-ttu-id="a7ccf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7ccf-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a7ccf-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7ccf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a7ccf-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7ccf-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a7ccf-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7ccf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7ccf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7ccf-114">Not supported.</span></span>                           |
| <span data-ttu-id="a7ccf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7ccf-115">Application</span></span>                            | <span data-ttu-id="a7ccf-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7ccf-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a7ccf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7ccf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a7ccf-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="a7ccf-118">Function parameters</span></span>

<span data-ttu-id="a7ccf-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a7ccf-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a7ccf-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a7ccf-120">Parameter</span></span> | <span data-ttu-id="a7ccf-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7ccf-121">Type</span></span>   | <span data-ttu-id="a7ccf-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7ccf-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a7ccf-123">ponto</span><span class="sxs-lookup"><span data-stu-id="a7ccf-123">period</span></span>    | <span data-ttu-id="a7ccf-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7ccf-124">string</span></span> | <span data-ttu-id="a7ccf-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a7ccf-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a7ccf-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="a7ccf-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a7ccf-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a7ccf-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a7ccf-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7ccf-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="a7ccf-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7ccf-129">Request headers</span></span>

| <span data-ttu-id="a7ccf-130">Nome</span><span class="sxs-lookup"><span data-stu-id="a7ccf-130">Name</span></span>          | <span data-ttu-id="a7ccf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7ccf-131">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a7ccf-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7ccf-132">Authorization</span></span> | <span data-ttu-id="a7ccf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7ccf-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a7ccf-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7ccf-135">Response</span></span>

<span data-ttu-id="a7ccf-136">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="a7ccf-136">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a7ccf-137">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="a7ccf-137">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a7ccf-138">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a7ccf-138">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a7ccf-139">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="a7ccf-139">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a7ccf-140">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="a7ccf-140">Report Refresh Date</span></span>
- <span data-ttu-id="a7ccf-141">Office 365</span><span class="sxs-lookup"><span data-stu-id="a7ccf-141">Office 365</span></span>
- <span data-ttu-id="a7ccf-142">Exchange</span><span class="sxs-lookup"><span data-stu-id="a7ccf-142">Exchange</span></span>
- <span data-ttu-id="a7ccf-143">OneDrive</span><span class="sxs-lookup"><span data-stu-id="a7ccf-143">OneDrive</span></span>
- <span data-ttu-id="a7ccf-144">SharePoint</span><span class="sxs-lookup"><span data-stu-id="a7ccf-144">SharePoint</span></span>
- <span data-ttu-id="a7ccf-145">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="a7ccf-145">Skype For Business</span></span> 
- <span data-ttu-id="a7ccf-146">Yammer</span><span class="sxs-lookup"><span data-stu-id="a7ccf-146">Yammer</span></span>
- <span data-ttu-id="a7ccf-147">Teams</span><span class="sxs-lookup"><span data-stu-id="a7ccf-147">Teams</span></span>
- <span data-ttu-id="a7ccf-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="a7ccf-148">Report Date</span></span>
- <span data-ttu-id="a7ccf-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="a7ccf-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="a7ccf-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7ccf-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a7ccf-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7ccf-151">Request</span></span>

<span data-ttu-id="a7ccf-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7ccf-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="a7ccf-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7ccf-153">Response</span></span>

<span data-ttu-id="a7ccf-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a7ccf-154">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a7ccf-155">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="a7ccf-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a7ccf-156">C#</span><span class="sxs-lookup"><span data-stu-id="a7ccf-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a7ccf-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="a7ccf-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeusercounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a7ccf-158">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a7ccf-158">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeusercounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="a7ccf-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="a7ccf-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activeusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activeusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activeusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
