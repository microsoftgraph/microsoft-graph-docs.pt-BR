---
title: 'reportRoot: getYammerActivityUserCounts'
description: Obtenha as tendências do número de usuários exclusivos que postaram, leram e curtiram mensagens do Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 61dd07d7a709dfe0431665be618683774c8f55eb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021638"
---
# <a name="reportroot-getyammeractivityusercounts"></a><span data-ttu-id="11675-103">reportRoot: getYammerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="11675-103">reportRoot: getYammerActivityUserCounts</span></span>

<span data-ttu-id="11675-104">Obtenha as tendências do número de usuários exclusivos que postaram, leram e curtiram mensagens do Yammer.</span><span class="sxs-lookup"><span data-stu-id="11675-104">Get the trends on the number of unique users who posted, read, and liked Yammer messages.</span></span>

> <span data-ttu-id="11675-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades do Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="11675-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="11675-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="11675-106">Permissions</span></span>

<span data-ttu-id="11675-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11675-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11675-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11675-109">Permission type</span></span>                        | <span data-ttu-id="11675-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11675-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="11675-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11675-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="11675-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="11675-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="11675-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11675-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11675-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11675-114">Not supported.</span></span>                           |
| <span data-ttu-id="11675-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11675-115">Application</span></span>                            | <span data-ttu-id="11675-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="11675-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="11675-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11675-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="11675-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="11675-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="11675-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="11675-119">Function parameters</span></span>

<span data-ttu-id="11675-120">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="11675-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="11675-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="11675-121">Parameter</span></span> | <span data-ttu-id="11675-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="11675-122">Type</span></span>   | <span data-ttu-id="11675-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="11675-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="11675-124">ponto</span><span class="sxs-lookup"><span data-stu-id="11675-124">period</span></span>    | <span data-ttu-id="11675-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11675-125">string</span></span> | <span data-ttu-id="11675-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="11675-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="11675-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="11675-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="11675-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="11675-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="11675-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11675-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="11675-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11675-130">Request headers</span></span>

| <span data-ttu-id="11675-131">Nome</span><span class="sxs-lookup"><span data-stu-id="11675-131">Name</span></span>          | <span data-ttu-id="11675-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="11675-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="11675-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="11675-133">Authorization</span></span> | <span data-ttu-id="11675-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11675-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="11675-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="11675-136">If-None-Match</span></span> | <span data-ttu-id="11675-137">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="11675-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="11675-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="11675-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="11675-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="11675-139">Response</span></span>

<span data-ttu-id="11675-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="11675-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="11675-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="11675-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="11675-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="11675-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="11675-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="11675-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="11675-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="11675-144">Report Refresh Date</span></span>
- <span data-ttu-id="11675-145">Curtidos</span><span class="sxs-lookup"><span data-stu-id="11675-145">Liked</span></span>
- <span data-ttu-id="11675-146">Postados</span><span class="sxs-lookup"><span data-stu-id="11675-146">Posted</span></span>
- <span data-ttu-id="11675-147">Ler</span><span class="sxs-lookup"><span data-stu-id="11675-147">Read</span></span>
- <span data-ttu-id="11675-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="11675-148">Report Date</span></span>
- <span data-ttu-id="11675-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="11675-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="11675-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11675-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="11675-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11675-151">Request</span></span>

<span data-ttu-id="11675-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11675-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="11675-153">C#</span><span class="sxs-lookup"><span data-stu-id="11675-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="11675-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="11675-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="11675-155">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="11675-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="11675-156">Java</span><span class="sxs-lookup"><span data-stu-id="11675-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammeractivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="11675-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="11675-157">Response</span></span>

<span data-ttu-id="11675-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11675-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="11675-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="11675-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
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
