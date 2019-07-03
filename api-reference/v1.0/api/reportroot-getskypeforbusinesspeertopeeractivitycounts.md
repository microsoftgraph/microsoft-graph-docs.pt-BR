---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityCounts'
description: Obtenha tendências de uso no número e tipo de sessões realizadas em sua organização. Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: f1f1d104f85e85a475afd258b9428ce0971ba497
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444453"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivitycounts"></a><span data-ttu-id="27dde-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="27dde-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span></span>

<span data-ttu-id="27dde-105">Obtenha tendências de uso no número e tipo de sessões realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="27dde-105">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="27dde-106">Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos.</span><span class="sxs-lookup"><span data-stu-id="27dde-106">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span>

> <span data-ttu-id="27dde-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade ponto a ponto do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="27dde-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="27dde-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="27dde-108">Permissions</span></span>

<span data-ttu-id="27dde-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27dde-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27dde-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27dde-111">Permission type</span></span>                        | <span data-ttu-id="27dde-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27dde-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="27dde-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27dde-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="27dde-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="27dde-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="27dde-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27dde-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27dde-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27dde-116">Not supported.</span></span>                           |
| <span data-ttu-id="27dde-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27dde-117">Application</span></span>                            | <span data-ttu-id="27dde-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="27dde-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="27dde-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27dde-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="27dde-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="27dde-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="27dde-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="27dde-121">Function parameters</span></span>

<span data-ttu-id="27dde-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="27dde-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="27dde-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="27dde-123">Parameter</span></span> | <span data-ttu-id="27dde-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="27dde-124">Type</span></span>   | <span data-ttu-id="27dde-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="27dde-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="27dde-126">ponto</span><span class="sxs-lookup"><span data-stu-id="27dde-126">period</span></span>    | <span data-ttu-id="27dde-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27dde-127">string</span></span> | <span data-ttu-id="27dde-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="27dde-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="27dde-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="27dde-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="27dde-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="27dde-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="27dde-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27dde-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="27dde-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27dde-132">Request headers</span></span>

| <span data-ttu-id="27dde-133">Nome</span><span class="sxs-lookup"><span data-stu-id="27dde-133">Name</span></span>          | <span data-ttu-id="27dde-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="27dde-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="27dde-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="27dde-135">Authorization</span></span> | <span data-ttu-id="27dde-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27dde-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="27dde-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="27dde-138">If-None-Match</span></span> | <span data-ttu-id="27dde-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="27dde-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="27dde-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="27dde-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="27dde-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="27dde-141">Response</span></span>

<span data-ttu-id="27dde-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="27dde-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="27dde-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="27dde-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="27dde-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="27dde-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="27dde-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="27dde-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="27dde-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="27dde-146">Report Refresh Date</span></span>
- <span data-ttu-id="27dde-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="27dde-147">Report Date</span></span>
- <span data-ttu-id="27dde-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="27dde-148">Report Period</span></span>
- <span data-ttu-id="27dde-149">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="27dde-149">IM</span></span>
- <span data-ttu-id="27dde-150">Áudio</span><span class="sxs-lookup"><span data-stu-id="27dde-150">Audio</span></span>
- <span data-ttu-id="27dde-151">Vídeo</span><span class="sxs-lookup"><span data-stu-id="27dde-151">Video</span></span>
- <span data-ttu-id="27dde-152">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="27dde-152">App Sharing</span></span>
- <span data-ttu-id="27dde-153">Transferência de arquivos</span><span class="sxs-lookup"><span data-stu-id="27dde-153">File Transfer</span></span>

## <a name="example"></a><span data-ttu-id="27dde-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27dde-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="27dde-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27dde-155">Request</span></span>

<span data-ttu-id="27dde-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="27dde-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="27dde-157">C#</span><span class="sxs-lookup"><span data-stu-id="27dde-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27dde-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="27dde-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="27dde-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="27dde-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="27dde-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="27dde-160">Response</span></span>

<span data-ttu-id="27dde-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="27dde-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="27dde-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="27dde-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
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
