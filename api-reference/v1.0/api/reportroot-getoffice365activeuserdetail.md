---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Obtenha dados sobre os usuários ativos do Office 365.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 77bcab1728cede1721f28b38aaa5fec075816684
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729704"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="5999f-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="5999f-103">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="5999f-104">Obtenha dados sobre os usuários ativos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="5999f-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="5999f-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="5999f-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="5999f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5999f-106">Permissions</span></span>

<span data-ttu-id="5999f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5999f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5999f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5999f-109">Permission type</span></span>                        | <span data-ttu-id="5999f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5999f-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5999f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5999f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5999f-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5999f-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5999f-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5999f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5999f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5999f-114">Not supported.</span></span>                           |
| <span data-ttu-id="5999f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5999f-115">Application</span></span>                            | <span data-ttu-id="5999f-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5999f-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5999f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5999f-117">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="5999f-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="5999f-118">Function parameters</span></span>

<span data-ttu-id="5999f-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="5999f-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="5999f-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5999f-120">Parameter</span></span> | <span data-ttu-id="5999f-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5999f-121">Type</span></span>   | <span data-ttu-id="5999f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5999f-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5999f-123">ponto</span><span class="sxs-lookup"><span data-stu-id="5999f-123">period</span></span>    | <span data-ttu-id="5999f-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5999f-124">string</span></span> | <span data-ttu-id="5999f-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5999f-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5999f-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="5999f-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5999f-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5999f-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="5999f-128">data</span><span class="sxs-lookup"><span data-stu-id="5999f-128">date</span></span>      | <span data-ttu-id="5999f-129">Data</span><span class="sxs-lookup"><span data-stu-id="5999f-129">Date</span></span>   | <span data-ttu-id="5999f-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="5999f-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="5999f-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="5999f-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="5999f-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="5999f-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="5999f-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="5999f-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5999f-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5999f-134">Request headers</span></span>

| <span data-ttu-id="5999f-135">Nome</span><span class="sxs-lookup"><span data-stu-id="5999f-135">Name</span></span>          | <span data-ttu-id="5999f-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="5999f-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5999f-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="5999f-137">Authorization</span></span> | <span data-ttu-id="5999f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5999f-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5999f-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5999f-140">If-None-Match</span></span> | <span data-ttu-id="5999f-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="5999f-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5999f-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5999f-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5999f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5999f-143">Response</span></span>

<span data-ttu-id="5999f-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="5999f-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5999f-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="5999f-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5999f-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5999f-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5999f-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="5999f-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5999f-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="5999f-148">Report Refresh Date</span></span>
- <span data-ttu-id="5999f-149">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="5999f-149">User Principal Name</span></span>
- <span data-ttu-id="5999f-150">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="5999f-150">Display Name</span></span>
- <span data-ttu-id="5999f-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="5999f-151">Is Deleted</span></span>
- <span data-ttu-id="5999f-152">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="5999f-152">Deleted Date</span></span>
- <span data-ttu-id="5999f-153">Tem a licença do Exchange</span><span class="sxs-lookup"><span data-stu-id="5999f-153">Has Exchange License</span></span>
- <span data-ttu-id="5999f-154">Tem a licença do OneDrive</span><span class="sxs-lookup"><span data-stu-id="5999f-154">Has OneDrive License</span></span>
- <span data-ttu-id="5999f-155">Tem a licença do SharePoint</span><span class="sxs-lookup"><span data-stu-id="5999f-155">Has SharePoint License</span></span>
- <span data-ttu-id="5999f-156">Tem a licença do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="5999f-156">Has Skype For Business License</span></span>
- <span data-ttu-id="5999f-157">Tem a licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="5999f-157">Has Yammer License</span></span>
- <span data-ttu-id="5999f-158">Tem a licença do Teams</span><span class="sxs-lookup"><span data-stu-id="5999f-158">Has Teams License</span></span>
- <span data-ttu-id="5999f-159">Data da última atividade do Exchange</span><span class="sxs-lookup"><span data-stu-id="5999f-159">Exchange Last Activity Date</span></span>
- <span data-ttu-id="5999f-160">Data da última atividade do OneDrive</span><span class="sxs-lookup"><span data-stu-id="5999f-160">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="5999f-161">Data da última atividade do SharePoint</span><span class="sxs-lookup"><span data-stu-id="5999f-161">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="5999f-162">Data da última atividade do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="5999f-162">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="5999f-163">Data da última atividade do Yammer</span><span class="sxs-lookup"><span data-stu-id="5999f-163">Yammer Last Activity Date</span></span>
- <span data-ttu-id="5999f-164">Data da última atividade do Teams</span><span class="sxs-lookup"><span data-stu-id="5999f-164">Teams Last Activity Date</span></span>
- <span data-ttu-id="5999f-165">Data de atribuição da licença do Exchange</span><span class="sxs-lookup"><span data-stu-id="5999f-165">Exchange License Assign Date</span></span>
- <span data-ttu-id="5999f-166">Data de atribuição da licença do OneDrive</span><span class="sxs-lookup"><span data-stu-id="5999f-166">OneDrive License Assign Date</span></span>
- <span data-ttu-id="5999f-167">Data de atribuição da licença do SharePoint</span><span class="sxs-lookup"><span data-stu-id="5999f-167">SharePoint License Assign Date</span></span>
- <span data-ttu-id="5999f-168">Data de atribuição da licença do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="5999f-168">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="5999f-169">Data de atribuição da licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="5999f-169">Yammer License Assign Date</span></span>
- <span data-ttu-id="5999f-170">Data de atribuição da licença do Teams</span><span class="sxs-lookup"><span data-stu-id="5999f-170">Teams License Assign Date</span></span>
- <span data-ttu-id="5999f-171">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="5999f-171">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="5999f-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5999f-172">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5999f-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5999f-173">Request</span></span>

<span data-ttu-id="5999f-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5999f-174">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5999f-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="5999f-175">--Http</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5999f-176">C#</span><span class="sxs-lookup"><span data-stu-id="5999f-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5999f-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5999f-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5999f-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5999f-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5999f-179">Java</span><span class="sxs-lookup"><span data-stu-id="5999f-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activeuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5999f-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="5999f-180">Response</span></span>

<span data-ttu-id="5999f-181">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5999f-181">The following is an example of the response.</span></span>

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

<span data-ttu-id="5999f-182">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="5999f-182">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
  ]
}-->
