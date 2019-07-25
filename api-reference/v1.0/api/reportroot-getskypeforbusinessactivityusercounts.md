---
title: 'reportRoot: getSkypeForBusinessActivityUserCounts'
description: Obtenha as tendências de quantos usuários únicos organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business. O relatório também inclui o número de sessões ponto a ponto.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 6e73319028d48d5e50f7f46de8ffbca64e923427
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892525"
---
# <a name="reportroot-getskypeforbusinessactivityusercounts"></a><span data-ttu-id="a22a3-104">reportRoot: getSkypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="a22a3-104">reportRoot: getSkypeForBusinessActivityUserCounts</span></span>

<span data-ttu-id="a22a3-105">Obtenha as tendências de quantos usuários únicos organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="a22a3-105">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="a22a3-106">O relatório também inclui o número de sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="a22a3-106">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="a22a3-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="a22a3-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="a22a3-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a22a3-108">Permissions</span></span>

<span data-ttu-id="a22a3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a22a3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a22a3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a22a3-111">Permission type</span></span>                        | <span data-ttu-id="a22a3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a22a3-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a22a3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a22a3-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a22a3-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a22a3-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a22a3-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a22a3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a22a3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a22a3-116">Not supported.</span></span>                           |
| <span data-ttu-id="a22a3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a22a3-117">Application</span></span>                            | <span data-ttu-id="a22a3-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a22a3-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a22a3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a22a3-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a22a3-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="a22a3-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a22a3-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="a22a3-121">Function parameters</span></span>

<span data-ttu-id="a22a3-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a22a3-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a22a3-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a22a3-123">Parameter</span></span> | <span data-ttu-id="a22a3-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="a22a3-124">Type</span></span>   | <span data-ttu-id="a22a3-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="a22a3-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a22a3-126">ponto</span><span class="sxs-lookup"><span data-stu-id="a22a3-126">period</span></span>    | <span data-ttu-id="a22a3-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a22a3-127">string</span></span> | <span data-ttu-id="a22a3-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a22a3-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a22a3-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="a22a3-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a22a3-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a22a3-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a22a3-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a22a3-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="a22a3-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a22a3-132">Request headers</span></span>

| <span data-ttu-id="a22a3-133">Nome</span><span class="sxs-lookup"><span data-stu-id="a22a3-133">Name</span></span>          | <span data-ttu-id="a22a3-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="a22a3-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="a22a3-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="a22a3-135">Authorization</span></span> | <span data-ttu-id="a22a3-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a22a3-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="a22a3-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a22a3-138">If-None-Match</span></span> | <span data-ttu-id="a22a3-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="a22a3-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="a22a3-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a22a3-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a22a3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a22a3-141">Response</span></span>

<span data-ttu-id="a22a3-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="a22a3-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a22a3-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="a22a3-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a22a3-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a22a3-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a22a3-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="a22a3-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a22a3-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="a22a3-146">Report Refresh Date</span></span>
- <span data-ttu-id="a22a3-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="a22a3-147">Report Date</span></span>
- <span data-ttu-id="a22a3-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="a22a3-148">Report Period</span></span>
- <span data-ttu-id="a22a3-149">Ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="a22a3-149">Peer-to-peer</span></span>
- <span data-ttu-id="a22a3-150">Organizadas</span><span class="sxs-lookup"><span data-stu-id="a22a3-150">Organized</span></span>
- <span data-ttu-id="a22a3-151">Participadas</span><span class="sxs-lookup"><span data-stu-id="a22a3-151">Participated</span></span>

## <a name="example"></a><span data-ttu-id="a22a3-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a22a3-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a22a3-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a22a3-153">Request</span></span>

<span data-ttu-id="a22a3-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a22a3-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a22a3-155">C#</span><span class="sxs-lookup"><span data-stu-id="a22a3-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a22a3-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="a22a3-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a22a3-157">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a22a3-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a22a3-158">Java</span><span class="sxs-lookup"><span data-stu-id="a22a3-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessactivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a22a3-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="a22a3-159">Response</span></span>

<span data-ttu-id="a22a3-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a22a3-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="a22a3-161">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="a22a3-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
