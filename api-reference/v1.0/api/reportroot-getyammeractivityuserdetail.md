---
title: 'reportRoot: getYammerActivityUserDetail'
description: Obtenha dados sobre as atividades do Yammer por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 890617cd8d41e2790dc4067a4e54fed4aa87e786
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320347"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="fa65a-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="fa65a-103">reportRoot: getYammerActivityUserDetail</span></span>

<span data-ttu-id="fa65a-104">Obtenha dados sobre as atividades do Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="fa65a-104">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="fa65a-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades do Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="fa65a-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="fa65a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa65a-106">Permissions</span></span>

<span data-ttu-id="fa65a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa65a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa65a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa65a-109">Permission type</span></span>                        | <span data-ttu-id="fa65a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa65a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fa65a-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa65a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa65a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa65a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fa65a-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa65a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa65a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa65a-114">Not supported.</span></span>                           |
| <span data-ttu-id="fa65a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa65a-115">Application</span></span>                            | <span data-ttu-id="fa65a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa65a-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fa65a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa65a-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="fa65a-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="fa65a-118">Function parameters</span></span>

<span data-ttu-id="fa65a-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="fa65a-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="fa65a-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fa65a-120">Parameter</span></span> | <span data-ttu-id="fa65a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa65a-121">Type</span></span>   | <span data-ttu-id="fa65a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa65a-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fa65a-123">ponto</span><span class="sxs-lookup"><span data-stu-id="fa65a-123">period</span></span>    | <span data-ttu-id="fa65a-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa65a-124">string</span></span> | <span data-ttu-id="fa65a-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="fa65a-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fa65a-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="fa65a-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fa65a-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="fa65a-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="fa65a-128">data</span><span class="sxs-lookup"><span data-stu-id="fa65a-128">date</span></span>      | <span data-ttu-id="fa65a-129">Data</span><span class="sxs-lookup"><span data-stu-id="fa65a-129">Date</span></span>   | <span data-ttu-id="fa65a-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="fa65a-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="fa65a-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="fa65a-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="fa65a-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="fa65a-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="fa65a-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="fa65a-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa65a-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa65a-134">Request headers</span></span>

| <span data-ttu-id="fa65a-135">Nome</span><span class="sxs-lookup"><span data-stu-id="fa65a-135">Name</span></span>          | <span data-ttu-id="fa65a-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa65a-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="fa65a-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa65a-137">Authorization</span></span> | <span data-ttu-id="fa65a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa65a-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="fa65a-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="fa65a-140">If-None-Match</span></span> | <span data-ttu-id="fa65a-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="fa65a-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="fa65a-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="fa65a-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="fa65a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa65a-143">Response</span></span>

<span data-ttu-id="fa65a-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="fa65a-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fa65a-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="fa65a-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fa65a-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="fa65a-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fa65a-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="fa65a-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fa65a-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="fa65a-148">Report Refresh Date</span></span>
- <span data-ttu-id="fa65a-149">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="fa65a-149">User Principal Name</span></span>
- <span data-ttu-id="fa65a-150">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="fa65a-150">Display Name</span></span>
- <span data-ttu-id="fa65a-151">Estado do usuário</span><span class="sxs-lookup"><span data-stu-id="fa65a-151">User State</span></span>
- <span data-ttu-id="fa65a-152">Data de alteração de estado</span><span class="sxs-lookup"><span data-stu-id="fa65a-152">State Change Date</span></span>
- <span data-ttu-id="fa65a-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="fa65a-153">Last Activity Date</span></span>
- <span data-ttu-id="fa65a-154">Contagem de Postagens</span><span class="sxs-lookup"><span data-stu-id="fa65a-154">Posted Count</span></span>
- <span data-ttu-id="fa65a-155">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="fa65a-155">Read Count</span></span>
- <span data-ttu-id="fa65a-156">Contagem de Curtidas</span><span class="sxs-lookup"><span data-stu-id="fa65a-156">Liked Count</span></span>
- <span data-ttu-id="fa65a-157">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="fa65a-157">Assigned Products</span></span>
- <span data-ttu-id="fa65a-158">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="fa65a-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="fa65a-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa65a-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fa65a-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa65a-160">Request</span></span>

<span data-ttu-id="fa65a-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa65a-161">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fa65a-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa65a-162">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa65a-163">C#</span><span class="sxs-lookup"><span data-stu-id="fa65a-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa65a-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa65a-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa65a-165">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fa65a-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fa65a-166">Java</span><span class="sxs-lookup"><span data-stu-id="fa65a-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammeractivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fa65a-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa65a-167">Response</span></span>

<span data-ttu-id="fa65a-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fa65a-168">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="fa65a-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa65a-169">Request</span></span>

<span data-ttu-id="fa65a-170">Se o `date` parâmetro for especificado, o relatório será delimitado às atividades que ocorreram na data especificada.</span><span class="sxs-lookup"><span data-stu-id="fa65a-170">If the `date` parameter is specified, the report is scoped to activities that took place on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="fa65a-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa65a-171">Response</span></span>

<span data-ttu-id="fa65a-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fa65a-172">The following is an example of the response.</span></span>

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


<span data-ttu-id="fa65a-173">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="fa65a-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Posted Count,Read Count,Liked Count,Assigned Products,Report Period
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
