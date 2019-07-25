---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityCounts'
description: Obtenha tendências de uso do número e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização. Os tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, Web, dial-in/out por terceiros, dial-in/out pela Microsoft.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9f57d6e21ca60855c58fd16bacf8a8fd0b38d9c7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892343"
---
# <a name="reportroot-getskypeforbusinessorganizeractivitycounts"></a><span data-ttu-id="6886e-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="6886e-104">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span></span>

<span data-ttu-id="6886e-105">Obtenha tendências de uso do número e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização.</span><span class="sxs-lookup"><span data-stu-id="6886e-105">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="6886e-106">Os tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, Web, dial-in/out por terceiros, dial-in/out pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6886e-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span>

> <span data-ttu-id="6886e-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do organizador da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="6886e-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="6886e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="6886e-108">Permissions</span></span>

<span data-ttu-id="6886e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6886e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6886e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6886e-111">Permission type</span></span>                        | <span data-ttu-id="6886e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6886e-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6886e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6886e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6886e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6886e-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6886e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6886e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6886e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6886e-116">Not supported.</span></span>                           |
| <span data-ttu-id="6886e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6886e-117">Application</span></span>                            | <span data-ttu-id="6886e-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6886e-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6886e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6886e-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6886e-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="6886e-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6886e-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="6886e-121">Function parameters</span></span>

<span data-ttu-id="6886e-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="6886e-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6886e-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6886e-123">Parameter</span></span> | <span data-ttu-id="6886e-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="6886e-124">Type</span></span>   | <span data-ttu-id="6886e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="6886e-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6886e-126">ponto</span><span class="sxs-lookup"><span data-stu-id="6886e-126">period</span></span>    | <span data-ttu-id="6886e-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6886e-127">string</span></span> | <span data-ttu-id="6886e-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="6886e-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6886e-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="6886e-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6886e-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="6886e-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6886e-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6886e-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="6886e-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6886e-132">Request headers</span></span>

| <span data-ttu-id="6886e-133">Nome</span><span class="sxs-lookup"><span data-stu-id="6886e-133">Name</span></span>          | <span data-ttu-id="6886e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="6886e-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="6886e-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="6886e-135">Authorization</span></span> | <span data-ttu-id="6886e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6886e-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="6886e-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="6886e-138">If-None-Match</span></span> | <span data-ttu-id="6886e-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="6886e-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="6886e-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6886e-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="6886e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6886e-141">Response</span></span>

<span data-ttu-id="6886e-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="6886e-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6886e-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="6886e-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6886e-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6886e-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6886e-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="6886e-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6886e-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="6886e-146">Report Refresh Date</span></span>
- <span data-ttu-id="6886e-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="6886e-147">Report Date</span></span>
- <span data-ttu-id="6886e-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="6886e-148">Report Period</span></span>
- <span data-ttu-id="6886e-149">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="6886e-149">IM</span></span>
- <span data-ttu-id="6886e-150">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="6886e-150">Audio/Video</span></span>
- <span data-ttu-id="6886e-151">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="6886e-151">App Sharing</span></span>
- <span data-ttu-id="6886e-152">Web</span><span class="sxs-lookup"><span data-stu-id="6886e-152">Web</span></span>
- <span data-ttu-id="6886e-153">Dial-in/out por terceiros</span><span class="sxs-lookup"><span data-stu-id="6886e-153">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="6886e-154">Dial-in/out pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="6886e-154">Dial-in/out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="6886e-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6886e-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6886e-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6886e-156">Request</span></span>

<span data-ttu-id="6886e-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6886e-157">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6886e-158">C#</span><span class="sxs-lookup"><span data-stu-id="6886e-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6886e-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="6886e-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6886e-160">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6886e-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6886e-161">Java</span><span class="sxs-lookup"><span data-stu-id="6886e-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessorganizeractivitycounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6886e-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="6886e-162">Response</span></span>

<span data-ttu-id="6886e-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6886e-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="6886e-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="6886e-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
  ]
}-->
