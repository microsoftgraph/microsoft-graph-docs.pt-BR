---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: Obtenha a contagem de usuários únicos conectados ao Exchange Online usando qualquer aplicativo de email.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: de7e63d57d8816fc3787dcf5572af2d36231f482
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728276"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="2d4b4-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="2d4b4-103">reportRoot: getEmailAppUsageUserCounts</span></span>

<span data-ttu-id="2d4b4-104">Obtenha a contagem de usuários únicos conectados ao Exchange Online usando qualquer aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-104">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="2d4b4-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="2d4b4-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="2d4b4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2d4b4-106">Permissions</span></span>

<span data-ttu-id="2d4b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d4b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d4b4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d4b4-109">Permission type</span></span>                        | <span data-ttu-id="2d4b4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2d4b4-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2d4b4-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d4b4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d4b4-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d4b4-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2d4b4-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d4b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d4b4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-114">Not supported.</span></span>                           |
| <span data-ttu-id="2d4b4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d4b4-115">Application</span></span>                            | <span data-ttu-id="2d4b4-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d4b4-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2d4b4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d4b4-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="2d4b4-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="2d4b4-118">Function parameters</span></span>

<span data-ttu-id="2d4b4-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2d4b4-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2d4b4-120">Parameter</span></span> | <span data-ttu-id="2d4b4-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d4b4-121">Type</span></span>   | <span data-ttu-id="2d4b4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d4b4-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2d4b4-123">ponto</span><span class="sxs-lookup"><span data-stu-id="2d4b4-123">period</span></span>    | <span data-ttu-id="2d4b4-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d4b4-124">string</span></span> | <span data-ttu-id="2d4b4-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2d4b4-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2d4b4-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2d4b4-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="2d4b4-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d4b4-129">Request headers</span></span>

| <span data-ttu-id="2d4b4-130">Nome</span><span class="sxs-lookup"><span data-stu-id="2d4b4-130">Name</span></span>          | <span data-ttu-id="2d4b4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d4b4-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="2d4b4-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d4b4-132">Authorization</span></span> | <span data-ttu-id="2d4b4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="2d4b4-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="2d4b4-135">If-None-Match</span></span> | <span data-ttu-id="2d4b4-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="2d4b4-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="2d4b4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d4b4-138">Response</span></span>

<span data-ttu-id="2d4b4-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2d4b4-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2d4b4-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2d4b4-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2d4b4-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="2d4b4-143">Report Refresh Date</span></span>
- <span data-ttu-id="2d4b4-144">Mail para Mac</span><span class="sxs-lookup"><span data-stu-id="2d4b4-144">Mail For Mac</span></span>
- <span data-ttu-id="2d4b4-145">Outlook para Mac</span><span class="sxs-lookup"><span data-stu-id="2d4b4-145">Outlook For Mac</span></span>
- <span data-ttu-id="2d4b4-146">Outlook para Windows</span><span class="sxs-lookup"><span data-stu-id="2d4b4-146">Outlook For Windows</span></span>
- <span data-ttu-id="2d4b4-147">Outlook para Celular</span><span class="sxs-lookup"><span data-stu-id="2d4b4-147">Outlook For Mobile</span></span>
- <span data-ttu-id="2d4b4-148">Outro para Celular</span><span class="sxs-lookup"><span data-stu-id="2d4b4-148">Other For Mobile</span></span>
- <span data-ttu-id="2d4b4-149">Outlook para Web</span><span class="sxs-lookup"><span data-stu-id="2d4b4-149">Outlook For Web</span></span>
- <span data-ttu-id="2d4b4-150">Aplicativo POP3</span><span class="sxs-lookup"><span data-stu-id="2d4b4-150">POP3 App</span></span>
- <span data-ttu-id="2d4b4-151">Aplicativo IMAP4</span><span class="sxs-lookup"><span data-stu-id="2d4b4-151">IMAP4 App</span></span>
- <span data-ttu-id="2d4b4-152">Aplicativo SMTP</span><span class="sxs-lookup"><span data-stu-id="2d4b4-152">SMTP App</span></span>
- <span data-ttu-id="2d4b4-153">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="2d4b4-153">Report Date</span></span>
- <span data-ttu-id="2d4b4-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="2d4b4-154">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="2d4b4-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d4b4-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2d4b4-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d4b4-156">Request</span></span>

<span data-ttu-id="2d4b4-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2d4b4-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d4b4-158">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2d4b4-159">C#</span><span class="sxs-lookup"><span data-stu-id="2d4b4-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2d4b4-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d4b4-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2d4b4-161">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2d4b4-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2d4b4-162">Java</span><span class="sxs-lookup"><span data-stu-id="2d4b4-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailappusageusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2d4b4-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d4b4-163">Response</span></span>

<span data-ttu-id="2d4b4-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="2d4b4-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="2d4b4-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Date,Report Period
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
