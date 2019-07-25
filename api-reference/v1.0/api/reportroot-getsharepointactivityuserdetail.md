---
title: 'reportRoot: getSharePointActivityUserDetail'
description: Obtenha dados sobre as atividades do SharePoint por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 72c6a9c9ed25ebc6a7351be599bf03fdd272f9b5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893465"
---
# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="05743-103">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="05743-103">reportRoot: getSharePointActivityUserDetail</span></span>

<span data-ttu-id="05743-104">Obtenha dados sobre as atividades do SharePoint por usuário.</span><span class="sxs-lookup"><span data-stu-id="05743-104">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="05743-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="05743-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="05743-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="05743-106">Permissions</span></span>

<span data-ttu-id="05743-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05743-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05743-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05743-109">Permission type</span></span>                        | <span data-ttu-id="05743-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05743-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="05743-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05743-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="05743-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="05743-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="05743-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05743-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05743-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05743-114">Not supported.</span></span>                           |
| <span data-ttu-id="05743-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05743-115">Application</span></span>                            | <span data-ttu-id="05743-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="05743-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="05743-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05743-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="05743-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="05743-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="05743-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="05743-119">Function parameters</span></span>

<span data-ttu-id="05743-120">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="05743-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="05743-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="05743-121">Parameter</span></span> | <span data-ttu-id="05743-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="05743-122">Type</span></span>   | <span data-ttu-id="05743-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="05743-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="05743-124">ponto</span><span class="sxs-lookup"><span data-stu-id="05743-124">period</span></span>    | <span data-ttu-id="05743-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05743-125">string</span></span> | <span data-ttu-id="05743-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="05743-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="05743-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="05743-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="05743-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="05743-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="05743-129">data</span><span class="sxs-lookup"><span data-stu-id="05743-129">date</span></span>      | <span data-ttu-id="05743-130">Data</span><span class="sxs-lookup"><span data-stu-id="05743-130">Date</span></span>   | <span data-ttu-id="05743-131">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="05743-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="05743-132">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="05743-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="05743-133">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="05743-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="05743-134">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="05743-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="05743-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05743-135">Request headers</span></span>

| <span data-ttu-id="05743-136">Nome</span><span class="sxs-lookup"><span data-stu-id="05743-136">Name</span></span>          | <span data-ttu-id="05743-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="05743-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="05743-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="05743-138">Authorization</span></span> | <span data-ttu-id="05743-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05743-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="05743-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="05743-141">If-None-Match</span></span> | <span data-ttu-id="05743-142">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="05743-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="05743-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="05743-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="05743-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="05743-144">Response</span></span>

<span data-ttu-id="05743-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="05743-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="05743-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="05743-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="05743-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="05743-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="05743-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="05743-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="05743-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="05743-149">Report Refresh Date</span></span>
- <span data-ttu-id="05743-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="05743-150">User Principal Name</span></span>
- <span data-ttu-id="05743-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="05743-151">Is Deleted</span></span>
- <span data-ttu-id="05743-152">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="05743-152">Deleted Date</span></span>
- <span data-ttu-id="05743-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="05743-153">Last Activity Date</span></span>
- <span data-ttu-id="05743-154">Contagem de arquivos exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="05743-154">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="05743-155">Contagem de arquivos sincronizados</span><span class="sxs-lookup"><span data-stu-id="05743-155">Synced File Count</span></span>
- <span data-ttu-id="05743-156">Contagem de arquivos compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="05743-156">Shared Internally File Count</span></span>
- <span data-ttu-id="05743-157">Contagem de arquivos compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="05743-157">Shared Externally File Count</span></span>
- <span data-ttu-id="05743-158">Contagem de páginas visitadas</span><span class="sxs-lookup"><span data-stu-id="05743-158">Visited Page Count</span></span>
- <span data-ttu-id="05743-159">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="05743-159">Assigned Products</span></span>
- <span data-ttu-id="05743-160">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="05743-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="05743-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05743-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="05743-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05743-162">Request</span></span>

<span data-ttu-id="05743-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="05743-163">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="05743-164">C#</span><span class="sxs-lookup"><span data-stu-id="05743-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="05743-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="05743-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="05743-166">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="05743-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="05743-167">Java</span><span class="sxs-lookup"><span data-stu-id="05743-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="05743-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="05743-168">Response</span></span>

<span data-ttu-id="05743-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="05743-169">The following is an example of the response.</span></span>

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

<span data-ttu-id="05743-170">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="05743-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Visited Page Count,Assigned Products,Report Period
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
