---
title: 'reportRoot: getEmailActivityUserCounts'
description: Permite que você compreenda as tendências do número de usuários únicos que estão executando atividades de email, como enviar, ler e receber.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 192447ee724ae57ed3bfffae1ba76786969bf4ca
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728325"
---
# <a name="reportroot-getemailactivityusercounts"></a><span data-ttu-id="b8c51-103">reportRoot: getEmailActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="b8c51-103">reportRoot: getEmailActivityUserCounts</span></span>

<span data-ttu-id="b8c51-104">Permite que você compreenda as tendências do número de usuários únicos que estão executando atividades de email, como enviar, ler e receber.</span><span class="sxs-lookup"><span data-stu-id="b8c51-104">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span>

> <span data-ttu-id="b8c51-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="b8c51-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8c51-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8c51-106">Permissions</span></span>

<span data-ttu-id="b8c51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8c51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8c51-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8c51-109">Permission type</span></span>                        | <span data-ttu-id="b8c51-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8c51-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b8c51-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8c51-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8c51-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8c51-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b8c51-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8c51-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8c51-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8c51-114">Not supported.</span></span>                           |
| <span data-ttu-id="b8c51-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8c51-115">Application</span></span>                            | <span data-ttu-id="b8c51-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8c51-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b8c51-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8c51-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b8c51-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b8c51-118">Function parameters</span></span>

<span data-ttu-id="b8c51-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="b8c51-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b8c51-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b8c51-120">Parameter</span></span> | <span data-ttu-id="b8c51-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8c51-121">Type</span></span>   | <span data-ttu-id="b8c51-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8c51-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b8c51-123">ponto</span><span class="sxs-lookup"><span data-stu-id="b8c51-123">period</span></span>    | <span data-ttu-id="b8c51-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8c51-124">string</span></span> | <span data-ttu-id="b8c51-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b8c51-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b8c51-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="b8c51-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b8c51-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b8c51-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b8c51-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8c51-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b8c51-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8c51-129">Request headers</span></span>

| <span data-ttu-id="b8c51-130">Nome</span><span class="sxs-lookup"><span data-stu-id="b8c51-130">Name</span></span>          | <span data-ttu-id="b8c51-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8c51-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b8c51-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8c51-132">Authorization</span></span> | <span data-ttu-id="b8c51-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8c51-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b8c51-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b8c51-135">If-None-Match</span></span> | <span data-ttu-id="b8c51-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="b8c51-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b8c51-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b8c51-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b8c51-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8c51-138">Response</span></span>

<span data-ttu-id="b8c51-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="b8c51-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b8c51-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="b8c51-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b8c51-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b8c51-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b8c51-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="b8c51-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b8c51-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="b8c51-143">Report Refresh Date</span></span>
- <span data-ttu-id="b8c51-144">Enviar</span><span class="sxs-lookup"><span data-stu-id="b8c51-144">Send</span></span>
- <span data-ttu-id="b8c51-145">Receber</span><span class="sxs-lookup"><span data-stu-id="b8c51-145">Receive</span></span>
- <span data-ttu-id="b8c51-146">Ler</span><span class="sxs-lookup"><span data-stu-id="b8c51-146">Read</span></span>
- <span data-ttu-id="b8c51-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="b8c51-147">Report Date</span></span>
- <span data-ttu-id="b8c51-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="b8c51-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b8c51-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8c51-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b8c51-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8c51-150">Request</span></span>

<span data-ttu-id="b8c51-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8c51-151">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b8c51-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8c51-152">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b8c51-153">C#</span><span class="sxs-lookup"><span data-stu-id="b8c51-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8c51-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8c51-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b8c51-155">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b8c51-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b8c51-156">Java</span><span class="sxs-lookup"><span data-stu-id="b8c51-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailactivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b8c51-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8c51-157">Response</span></span>

<span data-ttu-id="b8c51-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b8c51-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="b8c51-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="b8c51-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
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
