---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: Obtenha tendências de uso da duração em minutos e tipo de sessões ponto a ponto realizadas em sua organização. Tipos de sessões incluem áudio e vídeo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 1563d38e24e4c2fd74539a7f4d7116360bcda0af
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729452"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="34672-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="34672-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

<span data-ttu-id="34672-105">Obtenha tendências de uso da duração em minutos e tipo de sessões ponto a ponto realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="34672-105">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="34672-106">Tipos de sessões incluem áudio e vídeo.</span><span class="sxs-lookup"><span data-stu-id="34672-106">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="34672-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade ponto a ponto do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="34672-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="34672-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="34672-108">Permissions</span></span>

<span data-ttu-id="34672-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34672-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="34672-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34672-111">Permission type</span></span>                        | <span data-ttu-id="34672-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34672-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="34672-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34672-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="34672-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="34672-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="34672-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34672-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34672-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34672-116">Not supported.</span></span>                           |
| <span data-ttu-id="34672-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34672-117">Application</span></span>                            | <span data-ttu-id="34672-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="34672-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="34672-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34672-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="34672-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="34672-120">Function parameters</span></span>

<span data-ttu-id="34672-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="34672-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="34672-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="34672-122">Parameter</span></span> | <span data-ttu-id="34672-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="34672-123">Type</span></span>   | <span data-ttu-id="34672-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="34672-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="34672-125">ponto</span><span class="sxs-lookup"><span data-stu-id="34672-125">period</span></span>    | <span data-ttu-id="34672-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34672-126">string</span></span> | <span data-ttu-id="34672-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="34672-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="34672-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="34672-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="34672-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="34672-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="34672-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34672-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="34672-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34672-131">Request headers</span></span>

| <span data-ttu-id="34672-132">Nome</span><span class="sxs-lookup"><span data-stu-id="34672-132">Name</span></span>          | <span data-ttu-id="34672-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="34672-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="34672-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="34672-134">Authorization</span></span> | <span data-ttu-id="34672-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34672-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="34672-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="34672-137">If-None-Match</span></span> | <span data-ttu-id="34672-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="34672-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="34672-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="34672-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="34672-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="34672-140">Response</span></span>

<span data-ttu-id="34672-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="34672-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="34672-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="34672-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="34672-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="34672-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="34672-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="34672-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="34672-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="34672-145">Report Refresh Date</span></span>
- <span data-ttu-id="34672-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="34672-146">Report Date</span></span>
- <span data-ttu-id="34672-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="34672-147">Report Period</span></span>
- <span data-ttu-id="34672-148">Áudio</span><span class="sxs-lookup"><span data-stu-id="34672-148">Audio</span></span>
- <span data-ttu-id="34672-149">Vídeo</span><span class="sxs-lookup"><span data-stu-id="34672-149">Video</span></span>

## <a name="example"></a><span data-ttu-id="34672-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34672-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="34672-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34672-151">Request</span></span>

<span data-ttu-id="34672-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="34672-152">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="34672-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="34672-153">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="34672-154">C#</span><span class="sxs-lookup"><span data-stu-id="34672-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="34672-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34672-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="34672-156">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="34672-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="34672-157">Java</span><span class="sxs-lookup"><span data-stu-id="34672-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinesspeertopeeractivityminutecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="34672-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="34672-158">Response</span></span>

<span data-ttu-id="34672-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="34672-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="34672-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="34672-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio,Video
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
