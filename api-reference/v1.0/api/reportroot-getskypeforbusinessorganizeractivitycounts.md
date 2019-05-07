---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityCounts'
description: Obtenha tendências de uso do número e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização. Os tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, Web, dial-in/out por terceiros, dial-in/out pela Microsoft.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 35d751a2906929940acded4cf7d3b1bd325b512a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33604271"
---
# <a name="reportroot-getskypeforbusinessorganizeractivitycounts"></a><span data-ttu-id="dfb1b-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="dfb1b-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span></span>

<span data-ttu-id="dfb1b-105">Obtenha tendências de uso do número e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização.</span><span class="sxs-lookup"><span data-stu-id="dfb1b-105">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="dfb1b-106">Os tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, Web, dial-in/out por terceiros, dial-in/out pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="dfb1b-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span>

> <span data-ttu-id="dfb1b-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do organizador da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="dfb1b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="dfb1b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="dfb1b-108">Permissions</span></span>

<span data-ttu-id="dfb1b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfb1b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dfb1b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfb1b-111">Permission type</span></span>                        | <span data-ttu-id="dfb1b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dfb1b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dfb1b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfb1b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="dfb1b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfb1b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="dfb1b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfb1b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfb1b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfb1b-116">Not supported.</span></span>                           |
| <span data-ttu-id="dfb1b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfb1b-117">Application</span></span>                            | <span data-ttu-id="dfb1b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfb1b-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="dfb1b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfb1b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="dfb1b-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="dfb1b-120">Function parameters</span></span>

<span data-ttu-id="dfb1b-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="dfb1b-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="dfb1b-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dfb1b-122">Parameter</span></span> | <span data-ttu-id="dfb1b-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfb1b-123">Type</span></span>   | <span data-ttu-id="dfb1b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfb1b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="dfb1b-125">ponto</span><span class="sxs-lookup"><span data-stu-id="dfb1b-125">period</span></span>    | <span data-ttu-id="dfb1b-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dfb1b-126">string</span></span> | <span data-ttu-id="dfb1b-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="dfb1b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="dfb1b-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="dfb1b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="dfb1b-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="dfb1b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="dfb1b-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfb1b-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="dfb1b-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfb1b-131">Request headers</span></span>

| <span data-ttu-id="dfb1b-132">Nome</span><span class="sxs-lookup"><span data-stu-id="dfb1b-132">Name</span></span>          | <span data-ttu-id="dfb1b-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfb1b-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="dfb1b-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfb1b-134">Authorization</span></span> | <span data-ttu-id="dfb1b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfb1b-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="dfb1b-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="dfb1b-137">If-None-Match</span></span> | <span data-ttu-id="dfb1b-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="dfb1b-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="dfb1b-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="dfb1b-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="dfb1b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfb1b-140">Response</span></span>

<span data-ttu-id="dfb1b-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="dfb1b-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dfb1b-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="dfb1b-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dfb1b-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="dfb1b-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="dfb1b-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="dfb1b-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="dfb1b-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="dfb1b-145">Report Refresh Date</span></span>
- <span data-ttu-id="dfb1b-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="dfb1b-146">Report Date</span></span>
- <span data-ttu-id="dfb1b-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="dfb1b-147">Report Period</span></span>
- <span data-ttu-id="dfb1b-148">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="dfb1b-148">IM</span></span>
- <span data-ttu-id="dfb1b-149">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="dfb1b-149">Audio/Video</span></span>
- <span data-ttu-id="dfb1b-150">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="dfb1b-150">App Sharing</span></span>
- <span data-ttu-id="dfb1b-151">Web</span><span class="sxs-lookup"><span data-stu-id="dfb1b-151">Web</span></span>
- <span data-ttu-id="dfb1b-152">Dial-in/out por terceiros</span><span class="sxs-lookup"><span data-stu-id="dfb1b-152">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="dfb1b-153">Dial-in/out pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="dfb1b-153">Dial-in/out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="dfb1b-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfb1b-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dfb1b-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfb1b-155">Request</span></span>

<span data-ttu-id="dfb1b-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfb1b-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="dfb1b-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfb1b-157">Response</span></span>

<span data-ttu-id="dfb1b-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dfb1b-158">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="dfb1b-159">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="dfb1b-159">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dfb1b-160">Basic</span><span class="sxs-lookup"><span data-stu-id="dfb1b-160">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivitycounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfb1b-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfb1b-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessorganizeractivitycounts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="dfb1b-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="dfb1b-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
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
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessorganizeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessorganizeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
