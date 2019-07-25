---
title: 'reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts'
description: Obtenha as tendências de uso da duração em minutos e o tipo de sessões de conferência das quais os usuários de sua organização participaram. Tipos de sessões de conferência incluem áudio/vídeo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 27b16e926d0efbe39e4ffd03a02a6b5dba31fa65
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892303"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="56b38-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="56b38-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

<span data-ttu-id="56b38-105">Obtenha as tendências de uso da duração em minutos e o tipo de sessões de conferência das quais os usuários de sua organização participaram.</span><span class="sxs-lookup"><span data-stu-id="56b38-105">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="56b38-106">Tipos de sessões de conferência incluem áudio/vídeo.</span><span class="sxs-lookup"><span data-stu-id="56b38-106">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="56b38-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do participante da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="56b38-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="56b38-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="56b38-108">Permissions</span></span>

<span data-ttu-id="56b38-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56b38-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56b38-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56b38-111">Permission type</span></span>                        | <span data-ttu-id="56b38-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56b38-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="56b38-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56b38-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="56b38-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="56b38-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="56b38-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56b38-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56b38-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56b38-116">Not supported.</span></span>                           |
| <span data-ttu-id="56b38-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56b38-117">Application</span></span>                            | <span data-ttu-id="56b38-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="56b38-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="56b38-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56b38-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="56b38-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="56b38-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="56b38-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="56b38-121">Function parameters</span></span>

<span data-ttu-id="56b38-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="56b38-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="56b38-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="56b38-123">Parameter</span></span> | <span data-ttu-id="56b38-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="56b38-124">Type</span></span>   | <span data-ttu-id="56b38-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="56b38-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="56b38-126">ponto</span><span class="sxs-lookup"><span data-stu-id="56b38-126">period</span></span>    | <span data-ttu-id="56b38-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56b38-127">string</span></span> | <span data-ttu-id="56b38-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="56b38-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="56b38-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="56b38-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="56b38-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="56b38-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="56b38-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56b38-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="56b38-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56b38-132">Request headers</span></span>

| <span data-ttu-id="56b38-133">Nome</span><span class="sxs-lookup"><span data-stu-id="56b38-133">Name</span></span>          | <span data-ttu-id="56b38-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="56b38-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="56b38-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="56b38-135">Authorization</span></span> | <span data-ttu-id="56b38-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56b38-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="56b38-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="56b38-138">If-None-Match</span></span> | <span data-ttu-id="56b38-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="56b38-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="56b38-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="56b38-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="56b38-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="56b38-141">Response</span></span>

<span data-ttu-id="56b38-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="56b38-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="56b38-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="56b38-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="56b38-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="56b38-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="56b38-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="56b38-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="56b38-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="56b38-146">Report Refresh Date</span></span>
- <span data-ttu-id="56b38-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="56b38-147">Report Date</span></span>
- <span data-ttu-id="56b38-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="56b38-148">Report Period</span></span>
- <span data-ttu-id="56b38-149">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="56b38-149">Audio/Video</span></span>

## <a name="example"></a><span data-ttu-id="56b38-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56b38-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="56b38-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56b38-151">Request</span></span>

<span data-ttu-id="56b38-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="56b38-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="56b38-153">C#</span><span class="sxs-lookup"><span data-stu-id="56b38-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivityminutecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56b38-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="56b38-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivityminutecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="56b38-155">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="56b38-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivityminutecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="56b38-156">Java</span><span class="sxs-lookup"><span data-stu-id="56b38-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessparticipantactivityminutecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="56b38-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="56b38-157">Response</span></span>

<span data-ttu-id="56b38-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="56b38-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="56b38-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="56b38-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video
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
