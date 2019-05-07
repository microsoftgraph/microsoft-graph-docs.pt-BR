---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Obtenha dados sobre os usuários ativos do Office 365.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 134ec4804a17bc70d16246474bc4de6b7514eb93
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33606601"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="c015c-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="c015c-103">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="c015c-104">Obtenha dados sobre os usuários ativos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="c015c-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="c015c-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="c015c-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="c015c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c015c-106">Permissions</span></span>

<span data-ttu-id="c015c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c015c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c015c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c015c-109">Permission type</span></span>                        | <span data-ttu-id="c015c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c015c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c015c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c015c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c015c-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c015c-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c015c-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c015c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c015c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c015c-114">Not supported.</span></span>                           |
| <span data-ttu-id="c015c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c015c-115">Application</span></span>                            | <span data-ttu-id="c015c-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c015c-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c015c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c015c-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="c015c-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="c015c-118">Function parameters</span></span>

<span data-ttu-id="c015c-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c015c-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="c015c-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c015c-120">Parameter</span></span> | <span data-ttu-id="c015c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c015c-121">Type</span></span>   | <span data-ttu-id="c015c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c015c-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c015c-123">ponto</span><span class="sxs-lookup"><span data-stu-id="c015c-123">period</span></span>    | <span data-ttu-id="c015c-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c015c-124">string</span></span> | <span data-ttu-id="c015c-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="c015c-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c015c-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="c015c-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c015c-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="c015c-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="c015c-128">data</span><span class="sxs-lookup"><span data-stu-id="c015c-128">date</span></span>      | <span data-ttu-id="c015c-129">Data</span><span class="sxs-lookup"><span data-stu-id="c015c-129">Date</span></span>   | <span data-ttu-id="c015c-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="c015c-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="c015c-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="c015c-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="c015c-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="c015c-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="c015c-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="c015c-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c015c-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c015c-134">Request headers</span></span>

| <span data-ttu-id="c015c-135">Nome</span><span class="sxs-lookup"><span data-stu-id="c015c-135">Name</span></span>          | <span data-ttu-id="c015c-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="c015c-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c015c-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="c015c-137">Authorization</span></span> | <span data-ttu-id="c015c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c015c-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c015c-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c015c-140">If-None-Match</span></span> | <span data-ttu-id="c015c-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="c015c-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c015c-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c015c-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c015c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c015c-143">Response</span></span>

<span data-ttu-id="c015c-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="c015c-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c015c-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="c015c-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c015c-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c015c-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c015c-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="c015c-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c015c-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="c015c-148">Report Refresh Date</span></span>
- <span data-ttu-id="c015c-149">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="c015c-149">User Principal Name</span></span>
- <span data-ttu-id="c015c-150">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="c015c-150">Display Name</span></span>
- <span data-ttu-id="c015c-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="c015c-151">Is Deleted</span></span>
- <span data-ttu-id="c015c-152">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="c015c-152">Deleted Date</span></span>
- <span data-ttu-id="c015c-153">Tem a licença do Exchange</span><span class="sxs-lookup"><span data-stu-id="c015c-153">Has Exchange License</span></span>
- <span data-ttu-id="c015c-154">Tem a licença do OneDrive</span><span class="sxs-lookup"><span data-stu-id="c015c-154">Has OneDrive License</span></span>
- <span data-ttu-id="c015c-155">Tem a licença do SharePoint</span><span class="sxs-lookup"><span data-stu-id="c015c-155">Has SharePoint License</span></span>
- <span data-ttu-id="c015c-156">Tem a licença do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="c015c-156">Has Skype For Business License</span></span>
- <span data-ttu-id="c015c-157">Tem a licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="c015c-157">Has Yammer License</span></span>
- <span data-ttu-id="c015c-158">Tem a licença do Teams</span><span class="sxs-lookup"><span data-stu-id="c015c-158">Has Teams License</span></span>
- <span data-ttu-id="c015c-159">Data da última atividade do Exchange</span><span class="sxs-lookup"><span data-stu-id="c015c-159">Exchange Last Activity Date</span></span>
- <span data-ttu-id="c015c-160">Data da última atividade do OneDrive</span><span class="sxs-lookup"><span data-stu-id="c015c-160">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="c015c-161">Data da última atividade do SharePoint</span><span class="sxs-lookup"><span data-stu-id="c015c-161">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="c015c-162">Data da última atividade do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="c015c-162">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="c015c-163">Data da última atividade do Yammer</span><span class="sxs-lookup"><span data-stu-id="c015c-163">Yammer Last Activity Date</span></span>
- <span data-ttu-id="c015c-164">Data da última atividade do Teams</span><span class="sxs-lookup"><span data-stu-id="c015c-164">Teams Last Activity Date</span></span>
- <span data-ttu-id="c015c-165">Data de atribuição da licença do Exchange</span><span class="sxs-lookup"><span data-stu-id="c015c-165">Exchange License Assign Date</span></span>
- <span data-ttu-id="c015c-166">Data de atribuição da licença do OneDrive</span><span class="sxs-lookup"><span data-stu-id="c015c-166">OneDrive License Assign Date</span></span>
- <span data-ttu-id="c015c-167">Data de atribuição da licença do SharePoint</span><span class="sxs-lookup"><span data-stu-id="c015c-167">SharePoint License Assign Date</span></span>
- <span data-ttu-id="c015c-168">Data de atribuição da licença do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="c015c-168">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="c015c-169">Data de atribuição da licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="c015c-169">Yammer License Assign Date</span></span>
- <span data-ttu-id="c015c-170">Data de atribuição da licença do Teams</span><span class="sxs-lookup"><span data-stu-id="c015c-170">Teams License Assign Date</span></span>
- <span data-ttu-id="c015c-171">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="c015c-171">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="c015c-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c015c-172">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c015c-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c015c-173">Request</span></span>

<span data-ttu-id="c015c-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c015c-174">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="c015c-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="c015c-175">Response</span></span>

<span data-ttu-id="c015c-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c015c-176">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c015c-177">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="c015c-177">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c015c-178">C#</span><span class="sxs-lookup"><span data-stu-id="c015c-178">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c015c-179">Javascript</span><span class="sxs-lookup"><span data-stu-id="c015c-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeuserdetail-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="c015c-180">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="c015c-180">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activeuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activeuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
