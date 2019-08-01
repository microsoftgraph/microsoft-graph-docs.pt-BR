---
title: 'reportRoot: getEmailActivityUserDetail'
description: Obtenha dados sobre as atividades de email que os usuários realizaram.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 9d9e24dfaebdc9a8321a3d2443e02d3fc9011311
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025159"
---
# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="83d8f-103">reportRoot: getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="83d8f-103">reportRoot: getEmailActivityUserDetail</span></span>

<span data-ttu-id="83d8f-104">Obtenha dados sobre as atividades de email que os usuários realizaram.</span><span class="sxs-lookup"><span data-stu-id="83d8f-104">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="83d8f-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="83d8f-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="83d8f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="83d8f-106">Permissions</span></span>

<span data-ttu-id="83d8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83d8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83d8f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83d8f-109">Permission type</span></span>                        | <span data-ttu-id="83d8f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83d8f-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="83d8f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83d8f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="83d8f-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="83d8f-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="83d8f-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83d8f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83d8f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83d8f-114">Not supported.</span></span>                           |
| <span data-ttu-id="83d8f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83d8f-115">Application</span></span>                            | <span data-ttu-id="83d8f-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="83d8f-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="83d8f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83d8f-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="83d8f-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="83d8f-118">--Http</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="83d8f-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="83d8f-119">Function parameters</span></span>

<span data-ttu-id="83d8f-120">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="83d8f-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="83d8f-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="83d8f-121">Parameter</span></span> | <span data-ttu-id="83d8f-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="83d8f-122">Type</span></span>   | <span data-ttu-id="83d8f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="83d8f-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="83d8f-124">ponto</span><span class="sxs-lookup"><span data-stu-id="83d8f-124">period</span></span>    | <span data-ttu-id="83d8f-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83d8f-125">string</span></span> | <span data-ttu-id="83d8f-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="83d8f-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="83d8f-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="83d8f-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="83d8f-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="83d8f-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="83d8f-129">data</span><span class="sxs-lookup"><span data-stu-id="83d8f-129">date</span></span>      | <span data-ttu-id="83d8f-130">Data</span><span class="sxs-lookup"><span data-stu-id="83d8f-130">Date</span></span>   | <span data-ttu-id="83d8f-131">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="83d8f-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="83d8f-132">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="83d8f-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="83d8f-133">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="83d8f-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="83d8f-134">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="83d8f-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="83d8f-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83d8f-135">Request headers</span></span>

| <span data-ttu-id="83d8f-136">Nome</span><span class="sxs-lookup"><span data-stu-id="83d8f-136">Name</span></span>          | <span data-ttu-id="83d8f-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="83d8f-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="83d8f-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="83d8f-138">Authorization</span></span> | <span data-ttu-id="83d8f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83d8f-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="83d8f-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="83d8f-141">If-None-Match</span></span> | <span data-ttu-id="83d8f-142">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="83d8f-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="83d8f-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="83d8f-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="83d8f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="83d8f-144">Response</span></span>

<span data-ttu-id="83d8f-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="83d8f-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="83d8f-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="83d8f-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="83d8f-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="83d8f-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="83d8f-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="83d8f-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="83d8f-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="83d8f-149">Report Refresh Date</span></span>
- <span data-ttu-id="83d8f-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="83d8f-150">User Principal Name</span></span>
- <span data-ttu-id="83d8f-151">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="83d8f-151">Display Name</span></span>
- <span data-ttu-id="83d8f-152">Excluído</span><span class="sxs-lookup"><span data-stu-id="83d8f-152">Is Deleted</span></span>
- <span data-ttu-id="83d8f-153">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="83d8f-153">Deleted Date</span></span>
- <span data-ttu-id="83d8f-154">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="83d8f-154">Last Activity Date</span></span>
- <span data-ttu-id="83d8f-155">Contagem de Envios</span><span class="sxs-lookup"><span data-stu-id="83d8f-155">Send Count</span></span>
- <span data-ttu-id="83d8f-156">Contagem de Recebimentos</span><span class="sxs-lookup"><span data-stu-id="83d8f-156">Receive Count</span></span>
- <span data-ttu-id="83d8f-157">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="83d8f-157">Read Count</span></span>
- <span data-ttu-id="83d8f-158">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="83d8f-158">Assigned Products</span></span>
- <span data-ttu-id="83d8f-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="83d8f-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="83d8f-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83d8f-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="83d8f-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83d8f-161">Request</span></span>

<span data-ttu-id="83d8f-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="83d8f-162">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="83d8f-163">C#</span><span class="sxs-lookup"><span data-stu-id="83d8f-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="83d8f-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="83d8f-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="83d8f-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83d8f-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="83d8f-166">Java</span><span class="sxs-lookup"><span data-stu-id="83d8f-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="83d8f-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="83d8f-167">Response</span></span>

<span data-ttu-id="83d8f-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="83d8f-168">The following is an example of the response.</span></span>

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

<span data-ttu-id="83d8f-169">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="83d8f-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Send Count,Receive Count,Read Count,Assigned Products,Report Period
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
