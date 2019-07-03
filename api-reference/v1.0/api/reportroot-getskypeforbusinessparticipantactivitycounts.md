---
title: 'reportRoot: getSkypeForBusinessParticipantActivityCounts'
description: Obtenha tendências de uso do número e o tipo de sessões de conferência das quais os usuários de sua organização participaram. Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e3df7ee23562fa3d7898fb2d144270451380dd58
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444418"
---
# <a name="reportroot-getskypeforbusinessparticipantactivitycounts"></a><span data-ttu-id="f403e-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span><span class="sxs-lookup"><span data-stu-id="f403e-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span></span>

<span data-ttu-id="f403e-105">Obtenha tendências de uso do número e o tipo de sessões de conferência das quais os usuários de sua organização participaram.</span><span class="sxs-lookup"><span data-stu-id="f403e-105">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="f403e-106">Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros.</span><span class="sxs-lookup"><span data-stu-id="f403e-106">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="f403e-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do participante da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="f403e-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="f403e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f403e-108">Permissions</span></span>

<span data-ttu-id="f403e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f403e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f403e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f403e-111">Permission type</span></span>                        | <span data-ttu-id="f403e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f403e-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f403e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f403e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f403e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f403e-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f403e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f403e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f403e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f403e-116">Not supported.</span></span>                           |
| <span data-ttu-id="f403e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f403e-117">Application</span></span>                            | <span data-ttu-id="f403e-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f403e-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f403e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f403e-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f403e-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="f403e-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f403e-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="f403e-121">Function parameters</span></span>

<span data-ttu-id="f403e-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="f403e-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f403e-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f403e-123">Parameter</span></span> | <span data-ttu-id="f403e-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="f403e-124">Type</span></span>   | <span data-ttu-id="f403e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f403e-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f403e-126">ponto</span><span class="sxs-lookup"><span data-stu-id="f403e-126">period</span></span>    | <span data-ttu-id="f403e-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f403e-127">string</span></span> | <span data-ttu-id="f403e-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f403e-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f403e-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="f403e-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f403e-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f403e-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f403e-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f403e-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f403e-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f403e-132">Request headers</span></span>

| <span data-ttu-id="f403e-133">Nome</span><span class="sxs-lookup"><span data-stu-id="f403e-133">Name</span></span>          | <span data-ttu-id="f403e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f403e-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f403e-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="f403e-135">Authorization</span></span> | <span data-ttu-id="f403e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f403e-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f403e-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f403e-138">If-None-Match</span></span> | <span data-ttu-id="f403e-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="f403e-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f403e-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f403e-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f403e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f403e-141">Response</span></span>

<span data-ttu-id="f403e-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="f403e-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f403e-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="f403e-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f403e-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f403e-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f403e-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="f403e-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f403e-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="f403e-146">Report Refresh Date</span></span>
- <span data-ttu-id="f403e-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="f403e-147">Report Date</span></span>
- <span data-ttu-id="f403e-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="f403e-148">Report Period</span></span>
- <span data-ttu-id="f403e-149">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="f403e-149">IM</span></span>
- <span data-ttu-id="f403e-150">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="f403e-150">Audio/Video</span></span>
- <span data-ttu-id="f403e-151">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="f403e-151">App Sharing</span></span>
- <span data-ttu-id="f403e-152">Web</span><span class="sxs-lookup"><span data-stu-id="f403e-152">Web</span></span>
- <span data-ttu-id="f403e-153">Dial-in/out por terceiros</span><span class="sxs-lookup"><span data-stu-id="f403e-153">Dial-in/out 3rd Party</span></span>

## <a name="example"></a><span data-ttu-id="f403e-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f403e-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f403e-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f403e-155">Request</span></span>

<span data-ttu-id="f403e-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f403e-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f403e-157">C#</span><span class="sxs-lookup"><span data-stu-id="f403e-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f403e-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="f403e-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f403e-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f403e-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f403e-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="f403e-160">Response</span></span>

<span data-ttu-id="f403e-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f403e-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="f403e-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="f403e-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
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
