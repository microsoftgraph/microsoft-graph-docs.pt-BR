---
title: 'reportRoot: getYammerActivityUserDetail'
description: Obtenha dados sobre as atividades do Yammer por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 44c36399bfbb24cdb9827b0232cb3f955bed8be2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024851"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="ef87d-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="ef87d-103">reportRoot: getYammerActivityUserDetail</span></span>

<span data-ttu-id="ef87d-104">Obtenha dados sobre as atividades do Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="ef87d-104">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="ef87d-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades do Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="ef87d-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="ef87d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ef87d-106">Permissions</span></span>

<span data-ttu-id="ef87d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef87d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ef87d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef87d-109">Permission type</span></span>                        | <span data-ttu-id="ef87d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef87d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ef87d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef87d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef87d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef87d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ef87d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef87d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef87d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef87d-114">Not supported.</span></span>                           |
| <span data-ttu-id="ef87d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef87d-115">Application</span></span>                            | <span data-ttu-id="ef87d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef87d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ef87d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef87d-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ef87d-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef87d-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="ef87d-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="ef87d-119">Function parameters</span></span>

<span data-ttu-id="ef87d-120">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ef87d-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="ef87d-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ef87d-121">Parameter</span></span> | <span data-ttu-id="ef87d-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef87d-122">Type</span></span>   | <span data-ttu-id="ef87d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef87d-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ef87d-124">ponto</span><span class="sxs-lookup"><span data-stu-id="ef87d-124">period</span></span>    | <span data-ttu-id="ef87d-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef87d-125">string</span></span> | <span data-ttu-id="ef87d-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ef87d-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ef87d-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="ef87d-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ef87d-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ef87d-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="ef87d-129">data</span><span class="sxs-lookup"><span data-stu-id="ef87d-129">date</span></span>      | <span data-ttu-id="ef87d-130">Data</span><span class="sxs-lookup"><span data-stu-id="ef87d-130">Date</span></span>   | <span data-ttu-id="ef87d-131">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="ef87d-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="ef87d-132">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="ef87d-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="ef87d-133">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="ef87d-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="ef87d-134">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="ef87d-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef87d-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef87d-135">Request headers</span></span>

| <span data-ttu-id="ef87d-136">Nome</span><span class="sxs-lookup"><span data-stu-id="ef87d-136">Name</span></span>          | <span data-ttu-id="ef87d-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef87d-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ef87d-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef87d-138">Authorization</span></span> | <span data-ttu-id="ef87d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef87d-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ef87d-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ef87d-141">If-None-Match</span></span> | <span data-ttu-id="ef87d-142">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="ef87d-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ef87d-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ef87d-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ef87d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef87d-144">Response</span></span>

<span data-ttu-id="ef87d-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="ef87d-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ef87d-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="ef87d-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ef87d-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ef87d-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ef87d-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="ef87d-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ef87d-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="ef87d-149">Report Refresh Date</span></span>
- <span data-ttu-id="ef87d-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="ef87d-150">User Principal Name</span></span>
- <span data-ttu-id="ef87d-151">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="ef87d-151">Display Name</span></span>
- <span data-ttu-id="ef87d-152">Estado do usuário</span><span class="sxs-lookup"><span data-stu-id="ef87d-152">User State</span></span>
- <span data-ttu-id="ef87d-153">Data de alteração de estado</span><span class="sxs-lookup"><span data-stu-id="ef87d-153">State Change Date</span></span>
- <span data-ttu-id="ef87d-154">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="ef87d-154">Last Activity Date</span></span>
- <span data-ttu-id="ef87d-155">Contagem de Postagens</span><span class="sxs-lookup"><span data-stu-id="ef87d-155">Posted Count</span></span>
- <span data-ttu-id="ef87d-156">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="ef87d-156">Read Count</span></span>
- <span data-ttu-id="ef87d-157">Contagem de Curtidas</span><span class="sxs-lookup"><span data-stu-id="ef87d-157">Liked Count</span></span>
- <span data-ttu-id="ef87d-158">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="ef87d-158">Assigned Products</span></span>
- <span data-ttu-id="ef87d-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="ef87d-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ef87d-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef87d-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ef87d-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef87d-161">Request</span></span>

<span data-ttu-id="ef87d-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef87d-162">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ef87d-163">C#</span><span class="sxs-lookup"><span data-stu-id="ef87d-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ef87d-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="ef87d-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ef87d-165">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ef87d-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ef87d-166">Java</span><span class="sxs-lookup"><span data-stu-id="ef87d-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammeractivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ef87d-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef87d-167">Response</span></span>

<span data-ttu-id="ef87d-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ef87d-168">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="ef87d-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef87d-169">Request</span></span>

<span data-ttu-id="ef87d-170">Se o `date` parâmetro for especificado, o relatório será delimitado às atividades que ocorreram na data especificada.</span><span class="sxs-lookup"><span data-stu-id="ef87d-170">If the `date` parameter is specified, the report is scoped to activities that took place on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="ef87d-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef87d-171">Response</span></span>

<span data-ttu-id="ef87d-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ef87d-172">The following is an example of the response.</span></span>

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


<span data-ttu-id="ef87d-173">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="ef87d-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
