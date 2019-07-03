---
title: 'reportRoot: getSharePointActivityPages'
description: Obtenha o número de páginas exclusivas visitadas pelos usuários.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 640a4925e78dcda055c74cd32c65a3111b4836eb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35454955"
---
# <a name="reportroot-getsharepointactivitypages"></a><span data-ttu-id="3fe18-103">reportRoot: getSharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="3fe18-103">reportRoot: getSharePointActivityPages</span></span>

<span data-ttu-id="3fe18-104">Obtenha o número de páginas exclusivas visitadas pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="3fe18-104">Get the number of unique pages visited by users.</span></span>

> <span data-ttu-id="3fe18-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="3fe18-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="3fe18-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3fe18-106">Permissions</span></span>

<span data-ttu-id="3fe18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fe18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3fe18-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3fe18-109">Permission type</span></span>                        | <span data-ttu-id="3fe18-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3fe18-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3fe18-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3fe18-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3fe18-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fe18-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3fe18-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3fe18-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fe18-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fe18-114">Not supported.</span></span>                           |
| <span data-ttu-id="3fe18-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3fe18-115">Application</span></span>                            | <span data-ttu-id="3fe18-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fe18-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3fe18-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3fe18-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3fe18-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="3fe18-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityPages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3fe18-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3fe18-119">Function parameters</span></span>

<span data-ttu-id="3fe18-120">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="3fe18-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3fe18-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3fe18-121">Parameter</span></span> | <span data-ttu-id="3fe18-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fe18-122">Type</span></span>   | <span data-ttu-id="3fe18-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fe18-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3fe18-124">ponto</span><span class="sxs-lookup"><span data-stu-id="3fe18-124">period</span></span>    | <span data-ttu-id="3fe18-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fe18-125">string</span></span> | <span data-ttu-id="3fe18-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3fe18-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3fe18-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="3fe18-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3fe18-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3fe18-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3fe18-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fe18-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="3fe18-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3fe18-130">Request headers</span></span>

| <span data-ttu-id="3fe18-131">Nome</span><span class="sxs-lookup"><span data-stu-id="3fe18-131">Name</span></span>          | <span data-ttu-id="3fe18-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fe18-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="3fe18-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="3fe18-133">Authorization</span></span> | <span data-ttu-id="3fe18-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fe18-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="3fe18-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="3fe18-136">If-None-Match</span></span> | <span data-ttu-id="3fe18-137">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="3fe18-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="3fe18-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3fe18-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3fe18-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fe18-139">Response</span></span>

<span data-ttu-id="3fe18-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="3fe18-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3fe18-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="3fe18-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3fe18-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3fe18-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3fe18-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="3fe18-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3fe18-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="3fe18-144">Report Refresh Date</span></span>
- <span data-ttu-id="3fe18-145">Contagem de páginas visitadas</span><span class="sxs-lookup"><span data-stu-id="3fe18-145">Visited Page Count</span></span>
- <span data-ttu-id="3fe18-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="3fe18-146">Report Date</span></span>
- <span data-ttu-id="3fe18-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="3fe18-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="3fe18-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3fe18-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3fe18-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3fe18-149">Request</span></span>

<span data-ttu-id="3fe18-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3fe18-150">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivitypages"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityPages(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3fe18-151">C#</span><span class="sxs-lookup"><span data-stu-id="3fe18-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivitypages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3fe18-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="3fe18-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivitypages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3fe18-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3fe18-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivitypages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3fe18-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fe18-154">Response</span></span>

<span data-ttu-id="3fe18-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3fe18-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="3fe18-156">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="3fe18-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page Count,Report Date,Report Period
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
