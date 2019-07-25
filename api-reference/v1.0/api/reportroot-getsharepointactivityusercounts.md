---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Obtenha a tendência no número de usuários ativos. Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: ee26ef70cebe3d2b9ee8f0d0ae2583a1368ef3b9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893519"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="64f41-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="64f41-104">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="64f41-105">Obtenha a tendência no número de usuários ativos.</span><span class="sxs-lookup"><span data-stu-id="64f41-105">Get the trend in the number of active users.</span></span> <span data-ttu-id="64f41-106">Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="64f41-106">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="64f41-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="64f41-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="64f41-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="64f41-108">Permissions</span></span>

<span data-ttu-id="64f41-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64f41-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64f41-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64f41-111">Permission type</span></span>                        | <span data-ttu-id="64f41-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64f41-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="64f41-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64f41-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="64f41-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="64f41-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="64f41-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64f41-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64f41-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64f41-116">Not supported.</span></span>                           |
| <span data-ttu-id="64f41-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64f41-117">Application</span></span>                            | <span data-ttu-id="64f41-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="64f41-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="64f41-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64f41-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="64f41-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="64f41-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="64f41-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="64f41-121">Function parameters</span></span>

<span data-ttu-id="64f41-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="64f41-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="64f41-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="64f41-123">Parameter</span></span> | <span data-ttu-id="64f41-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="64f41-124">Type</span></span>   | <span data-ttu-id="64f41-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="64f41-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="64f41-126">ponto</span><span class="sxs-lookup"><span data-stu-id="64f41-126">period</span></span>    | <span data-ttu-id="64f41-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64f41-127">string</span></span> | <span data-ttu-id="64f41-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="64f41-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="64f41-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="64f41-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="64f41-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="64f41-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="64f41-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64f41-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="64f41-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64f41-132">Request headers</span></span>

| <span data-ttu-id="64f41-133">Nome</span><span class="sxs-lookup"><span data-stu-id="64f41-133">Name</span></span>          | <span data-ttu-id="64f41-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="64f41-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="64f41-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="64f41-135">Authorization</span></span> | <span data-ttu-id="64f41-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64f41-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="64f41-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="64f41-138">If-None-Match</span></span> | <span data-ttu-id="64f41-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="64f41-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="64f41-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="64f41-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="64f41-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="64f41-141">Response</span></span>

<span data-ttu-id="64f41-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="64f41-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="64f41-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="64f41-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="64f41-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="64f41-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="64f41-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="64f41-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="64f41-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="64f41-146">Report Refresh Date</span></span>
- <span data-ttu-id="64f41-147">Página visitada</span><span class="sxs-lookup"><span data-stu-id="64f41-147">Visited Page</span></span>
- <span data-ttu-id="64f41-148">Exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="64f41-148">Viewed Or Edited</span></span>
- <span data-ttu-id="64f41-149">Sincronizados</span><span class="sxs-lookup"><span data-stu-id="64f41-149">Synced</span></span>
- <span data-ttu-id="64f41-150">Compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="64f41-150">Shared Internally</span></span>
- <span data-ttu-id="64f41-151">Compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="64f41-151">Shared Externally</span></span>
- <span data-ttu-id="64f41-152">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="64f41-152">Report Date</span></span>
- <span data-ttu-id="64f41-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="64f41-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="64f41-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64f41-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="64f41-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64f41-155">Request</span></span>

<span data-ttu-id="64f41-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="64f41-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="64f41-157">C#</span><span class="sxs-lookup"><span data-stu-id="64f41-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="64f41-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="64f41-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="64f41-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="64f41-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="64f41-160">Java</span><span class="sxs-lookup"><span data-stu-id="64f41-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointactivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="64f41-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="64f41-161">Response</span></span>

<span data-ttu-id="64f41-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="64f41-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="64f41-163">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="64f41-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
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
