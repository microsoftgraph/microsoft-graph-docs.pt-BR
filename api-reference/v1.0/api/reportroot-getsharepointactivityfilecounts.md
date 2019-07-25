---
title: 'reportRoot: getSharePointActivityFileCounts'
description: Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 17e4d806f08cde191ba7757a183e452645ba8343
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893576"
---
# <a name="reportroot-getsharepointactivityfilecounts"></a><span data-ttu-id="cc000-103">reportRoot: getSharePointActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="cc000-103">reportRoot: getSharePointActivityFileCounts</span></span>

<span data-ttu-id="cc000-104">Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cc000-104">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span>

> <span data-ttu-id="cc000-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="cc000-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="cc000-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc000-106">Permissions</span></span>

<span data-ttu-id="cc000-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc000-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cc000-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc000-109">Permission type</span></span>                        | <span data-ttu-id="cc000-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc000-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cc000-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc000-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc000-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc000-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cc000-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc000-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc000-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc000-114">Not supported.</span></span>                           |
| <span data-ttu-id="cc000-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc000-115">Application</span></span>                            | <span data-ttu-id="cc000-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc000-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cc000-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc000-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cc000-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc000-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="cc000-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="cc000-119">Function parameters</span></span>

<span data-ttu-id="cc000-120">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="cc000-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="cc000-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cc000-121">Parameter</span></span> | <span data-ttu-id="cc000-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc000-122">Type</span></span>   | <span data-ttu-id="cc000-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc000-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cc000-124">ponto</span><span class="sxs-lookup"><span data-stu-id="cc000-124">period</span></span>    | <span data-ttu-id="cc000-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc000-125">string</span></span> | <span data-ttu-id="cc000-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="cc000-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cc000-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="cc000-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cc000-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="cc000-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="cc000-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc000-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="cc000-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc000-130">Request headers</span></span>

| <span data-ttu-id="cc000-131">Nome</span><span class="sxs-lookup"><span data-stu-id="cc000-131">Name</span></span>          | <span data-ttu-id="cc000-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc000-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="cc000-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc000-133">Authorization</span></span> | <span data-ttu-id="cc000-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc000-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="cc000-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="cc000-136">If-None-Match</span></span> | <span data-ttu-id="cc000-137">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="cc000-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="cc000-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cc000-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="cc000-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc000-139">Response</span></span>

<span data-ttu-id="cc000-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="cc000-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cc000-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="cc000-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cc000-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="cc000-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cc000-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="cc000-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cc000-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="cc000-144">Report Refresh Date</span></span>
- <span data-ttu-id="cc000-145">Exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="cc000-145">Viewed Or Edited</span></span>
- <span data-ttu-id="cc000-146">Sincronizados</span><span class="sxs-lookup"><span data-stu-id="cc000-146">Synced</span></span>
- <span data-ttu-id="cc000-147">Compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="cc000-147">Shared Internally</span></span>
- <span data-ttu-id="cc000-148">Compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="cc000-148">Shared Externally</span></span>
- <span data-ttu-id="cc000-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="cc000-149">Report Date</span></span>
- <span data-ttu-id="cc000-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="cc000-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="cc000-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc000-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cc000-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc000-152">Request</span></span>

<span data-ttu-id="cc000-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc000-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityfilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityFileCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cc000-154">C#</span><span class="sxs-lookup"><span data-stu-id="cc000-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityfilecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cc000-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="cc000-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityfilecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cc000-156">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="cc000-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityfilecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cc000-157">Java</span><span class="sxs-lookup"><span data-stu-id="cc000-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointactivityfilecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cc000-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc000-158">Response</span></span>

<span data-ttu-id="cc000-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cc000-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="cc000-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="cc000-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
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
