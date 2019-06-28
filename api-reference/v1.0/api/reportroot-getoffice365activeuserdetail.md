---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Obtenha dados sobre os usuários ativos do Office 365.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e759936f736a5949ca154943bcfa9cf12672271c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268709"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="108cb-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="108cb-103">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="108cb-104">Obtenha dados sobre os usuários ativos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="108cb-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="108cb-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="108cb-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="108cb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="108cb-106">Permissions</span></span>

<span data-ttu-id="108cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="108cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="108cb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="108cb-109">Permission type</span></span>                        | <span data-ttu-id="108cb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="108cb-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="108cb-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="108cb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="108cb-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="108cb-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="108cb-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="108cb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="108cb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="108cb-114">Not supported.</span></span>                           |
| <span data-ttu-id="108cb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="108cb-115">Application</span></span>                            | <span data-ttu-id="108cb-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="108cb-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="108cb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="108cb-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="108cb-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="108cb-118">Function parameters</span></span>

<span data-ttu-id="108cb-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="108cb-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="108cb-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="108cb-120">Parameter</span></span> | <span data-ttu-id="108cb-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="108cb-121">Type</span></span>   | <span data-ttu-id="108cb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="108cb-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="108cb-123">ponto</span><span class="sxs-lookup"><span data-stu-id="108cb-123">period</span></span>    | <span data-ttu-id="108cb-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="108cb-124">string</span></span> | <span data-ttu-id="108cb-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="108cb-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="108cb-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="108cb-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="108cb-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="108cb-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="108cb-128">data</span><span class="sxs-lookup"><span data-stu-id="108cb-128">date</span></span>      | <span data-ttu-id="108cb-129">Data</span><span class="sxs-lookup"><span data-stu-id="108cb-129">Date</span></span>   | <span data-ttu-id="108cb-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="108cb-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="108cb-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="108cb-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="108cb-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="108cb-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="108cb-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="108cb-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="108cb-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="108cb-134">Request headers</span></span>

| <span data-ttu-id="108cb-135">Nome</span><span class="sxs-lookup"><span data-stu-id="108cb-135">Name</span></span>          | <span data-ttu-id="108cb-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="108cb-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="108cb-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="108cb-137">Authorization</span></span> | <span data-ttu-id="108cb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="108cb-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="108cb-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="108cb-140">If-None-Match</span></span> | <span data-ttu-id="108cb-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="108cb-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="108cb-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="108cb-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="108cb-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="108cb-143">Response</span></span>

<span data-ttu-id="108cb-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="108cb-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="108cb-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="108cb-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="108cb-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="108cb-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="108cb-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="108cb-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="108cb-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="108cb-148">Report Refresh Date</span></span>
- <span data-ttu-id="108cb-149">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="108cb-149">User Principal Name</span></span>
- <span data-ttu-id="108cb-150">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="108cb-150">Display Name</span></span>
- <span data-ttu-id="108cb-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="108cb-151">Is Deleted</span></span>
- <span data-ttu-id="108cb-152">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="108cb-152">Deleted Date</span></span>
- <span data-ttu-id="108cb-153">Tem a licença do Exchange</span><span class="sxs-lookup"><span data-stu-id="108cb-153">Has Exchange License</span></span>
- <span data-ttu-id="108cb-154">Tem a licença do OneDrive</span><span class="sxs-lookup"><span data-stu-id="108cb-154">Has OneDrive License</span></span>
- <span data-ttu-id="108cb-155">Tem a licença do SharePoint</span><span class="sxs-lookup"><span data-stu-id="108cb-155">Has SharePoint License</span></span>
- <span data-ttu-id="108cb-156">Tem a licença do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="108cb-156">Has Skype For Business License</span></span>
- <span data-ttu-id="108cb-157">Tem a licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="108cb-157">Has Yammer License</span></span>
- <span data-ttu-id="108cb-158">Tem a licença do Teams</span><span class="sxs-lookup"><span data-stu-id="108cb-158">Has Teams License</span></span>
- <span data-ttu-id="108cb-159">Data da última atividade do Exchange</span><span class="sxs-lookup"><span data-stu-id="108cb-159">Exchange Last Activity Date</span></span>
- <span data-ttu-id="108cb-160">Data da última atividade do OneDrive</span><span class="sxs-lookup"><span data-stu-id="108cb-160">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="108cb-161">Data da última atividade do SharePoint</span><span class="sxs-lookup"><span data-stu-id="108cb-161">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="108cb-162">Data da última atividade do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="108cb-162">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="108cb-163">Data da última atividade do Yammer</span><span class="sxs-lookup"><span data-stu-id="108cb-163">Yammer Last Activity Date</span></span>
- <span data-ttu-id="108cb-164">Data da última atividade do Teams</span><span class="sxs-lookup"><span data-stu-id="108cb-164">Teams Last Activity Date</span></span>
- <span data-ttu-id="108cb-165">Data de atribuição da licença do Exchange</span><span class="sxs-lookup"><span data-stu-id="108cb-165">Exchange License Assign Date</span></span>
- <span data-ttu-id="108cb-166">Data de atribuição da licença do OneDrive</span><span class="sxs-lookup"><span data-stu-id="108cb-166">OneDrive License Assign Date</span></span>
- <span data-ttu-id="108cb-167">Data de atribuição da licença do SharePoint</span><span class="sxs-lookup"><span data-stu-id="108cb-167">SharePoint License Assign Date</span></span>
- <span data-ttu-id="108cb-168">Data de atribuição da licença do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="108cb-168">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="108cb-169">Data de atribuição da licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="108cb-169">Yammer License Assign Date</span></span>
- <span data-ttu-id="108cb-170">Data de atribuição da licença do Teams</span><span class="sxs-lookup"><span data-stu-id="108cb-170">Teams License Assign Date</span></span>
- <span data-ttu-id="108cb-171">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="108cb-171">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="108cb-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="108cb-172">Example</span></span>

#### <a name="request"></a><span data-ttu-id="108cb-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="108cb-173">Request</span></span>

<span data-ttu-id="108cb-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="108cb-174">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="108cb-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="108cb-175">Response</span></span>

<span data-ttu-id="108cb-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="108cb-176">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="108cb-177">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="108cb-177">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="108cb-178">C#</span><span class="sxs-lookup"><span data-stu-id="108cb-178">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="108cb-179">Javascript</span><span class="sxs-lookup"><span data-stu-id="108cb-179">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeuserdetail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="108cb-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="108cb-180">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeuserdetail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="108cb-181">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="108cb-181">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
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
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activeuserdetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activeuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activeuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
