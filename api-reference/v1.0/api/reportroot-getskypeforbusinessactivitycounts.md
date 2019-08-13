---
title: 'reportRoot: getSkypeForBusinessActivityCounts'
description: Obtenha as tendências de quantos usuários organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business. O relatório também inclui o número de sessões ponto a ponto.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d845c5d61c58fc7dc5c7d05f462c70bb80466d92
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349324"
---
# <a name="reportroot-getskypeforbusinessactivitycounts"></a><span data-ttu-id="143b0-104">reportRoot: getSkypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="143b0-104">reportRoot: getSkypeForBusinessActivityCounts</span></span>

<span data-ttu-id="143b0-105">Obtenha as tendências de quantos usuários organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="143b0-105">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="143b0-106">O relatório também inclui o número de sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="143b0-106">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="143b0-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="143b0-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="143b0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="143b0-108">Permissions</span></span>

<span data-ttu-id="143b0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="143b0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="143b0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="143b0-111">Permission type</span></span>                        | <span data-ttu-id="143b0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="143b0-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="143b0-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="143b0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="143b0-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="143b0-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="143b0-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="143b0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="143b0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="143b0-116">Not supported.</span></span>                           |
| <span data-ttu-id="143b0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="143b0-117">Application</span></span>                            | <span data-ttu-id="143b0-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="143b0-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="143b0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="143b0-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="143b0-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="143b0-120">Function parameters</span></span>

<span data-ttu-id="143b0-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="143b0-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="143b0-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="143b0-122">Parameter</span></span> | <span data-ttu-id="143b0-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="143b0-123">Type</span></span>   | <span data-ttu-id="143b0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="143b0-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="143b0-125">ponto</span><span class="sxs-lookup"><span data-stu-id="143b0-125">period</span></span>    | <span data-ttu-id="143b0-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="143b0-126">string</span></span> | <span data-ttu-id="143b0-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="143b0-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="143b0-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="143b0-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="143b0-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="143b0-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="143b0-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="143b0-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="143b0-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="143b0-131">Request headers</span></span>

| <span data-ttu-id="143b0-132">Nome</span><span class="sxs-lookup"><span data-stu-id="143b0-132">Name</span></span>          | <span data-ttu-id="143b0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="143b0-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="143b0-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="143b0-134">Authorization</span></span> | <span data-ttu-id="143b0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="143b0-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="143b0-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="143b0-137">If-None-Match</span></span> | <span data-ttu-id="143b0-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="143b0-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="143b0-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="143b0-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="143b0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="143b0-140">Response</span></span>

<span data-ttu-id="143b0-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="143b0-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="143b0-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="143b0-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="143b0-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="143b0-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="143b0-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="143b0-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="143b0-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="143b0-145">Report Refresh Date</span></span>
- <span data-ttu-id="143b0-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="143b0-146">Report Date</span></span>
- <span data-ttu-id="143b0-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="143b0-147">Report Period</span></span>
- <span data-ttu-id="143b0-148">Ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="143b0-148">Peer-to-peer</span></span>
- <span data-ttu-id="143b0-149">Organizadas</span><span class="sxs-lookup"><span data-stu-id="143b0-149">Organized</span></span>
- <span data-ttu-id="143b0-150">Participadas</span><span class="sxs-lookup"><span data-stu-id="143b0-150">Participated</span></span>

## <a name="example"></a><span data-ttu-id="143b0-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="143b0-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="143b0-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="143b0-152">Request</span></span>

<span data-ttu-id="143b0-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="143b0-153">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="143b0-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="143b0-154">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="143b0-155">C#</span><span class="sxs-lookup"><span data-stu-id="143b0-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="143b0-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="143b0-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="143b0-157">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="143b0-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="143b0-158">Java</span><span class="sxs-lookup"><span data-stu-id="143b0-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessactivitycounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="143b0-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="143b0-159">Response</span></span>

<span data-ttu-id="143b0-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="143b0-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="143b0-161">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="143b0-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
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
