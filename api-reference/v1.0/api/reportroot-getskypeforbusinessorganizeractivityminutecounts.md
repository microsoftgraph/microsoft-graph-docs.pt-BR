---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts'
description: Obtenha tendências de uso na duração em minutos e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização. Tipos de sessões de conferência incluem áudio/vídeo e dial-in/out pela Microsoft.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f02f1eb78f7452f62378742f192c7023f4f037fd
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729494"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="7f7f1-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="7f7f1-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

<span data-ttu-id="7f7f1-105">Obtenha tendências de uso na duração em minutos e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização.</span><span class="sxs-lookup"><span data-stu-id="7f7f1-105">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="7f7f1-106">Tipos de sessões de conferência incluem áudio/vídeo e dial-in/out pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7f7f1-106">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="7f7f1-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do organizador da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="7f7f1-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f7f1-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f7f1-108">Permissions</span></span>

<span data-ttu-id="7f7f1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f7f1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f7f1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f7f1-111">Permission type</span></span>                        | <span data-ttu-id="7f7f1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f7f1-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7f7f1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f7f1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f7f1-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f7f1-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7f7f1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f7f1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f7f1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f7f1-116">Not supported.</span></span>                           |
| <span data-ttu-id="7f7f1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f7f1-117">Application</span></span>                            | <span data-ttu-id="7f7f1-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f7f1-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7f7f1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f7f1-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="7f7f1-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="7f7f1-120">Function parameters</span></span>

<span data-ttu-id="7f7f1-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="7f7f1-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7f7f1-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7f7f1-122">Parameter</span></span> | <span data-ttu-id="7f7f1-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f7f1-123">Type</span></span>   | <span data-ttu-id="7f7f1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f7f1-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7f7f1-125">ponto</span><span class="sxs-lookup"><span data-stu-id="7f7f1-125">period</span></span>    | <span data-ttu-id="7f7f1-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f7f1-126">string</span></span> | <span data-ttu-id="7f7f1-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7f7f1-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7f7f1-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="7f7f1-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7f7f1-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7f7f1-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7f7f1-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f7f1-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="7f7f1-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f7f1-131">Request headers</span></span>

| <span data-ttu-id="7f7f1-132">Nome</span><span class="sxs-lookup"><span data-stu-id="7f7f1-132">Name</span></span>          | <span data-ttu-id="7f7f1-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f7f1-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="7f7f1-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f7f1-134">Authorization</span></span> | <span data-ttu-id="7f7f1-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f7f1-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="7f7f1-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7f7f1-137">If-None-Match</span></span> | <span data-ttu-id="7f7f1-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="7f7f1-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="7f7f1-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7f7f1-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7f7f1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f7f1-140">Response</span></span>

<span data-ttu-id="7f7f1-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="7f7f1-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7f7f1-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="7f7f1-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7f7f1-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7f7f1-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7f7f1-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="7f7f1-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7f7f1-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="7f7f1-145">Report Refresh Date</span></span>
- <span data-ttu-id="7f7f1-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="7f7f1-146">Report Date</span></span>
- <span data-ttu-id="7f7f1-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="7f7f1-147">Report Period</span></span>
- <span data-ttu-id="7f7f1-148">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="7f7f1-148">Audio/Video</span></span>
- <span data-ttu-id="7f7f1-149">Dial-in pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="7f7f1-149">Dial-in Microsoft</span></span>
- <span data-ttu-id="7f7f1-150">Dial-out pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="7f7f1-150">Dial-out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="7f7f1-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f7f1-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7f7f1-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f7f1-152">Request</span></span>

<span data-ttu-id="7f7f1-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f7f1-153">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7f7f1-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f7f1-154">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7f7f1-155">C#</span><span class="sxs-lookup"><span data-stu-id="7f7f1-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivityminutecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f7f1-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f7f1-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivityminutecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7f7f1-157">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7f7f1-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivityminutecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7f7f1-158">Java</span><span class="sxs-lookup"><span data-stu-id="7f7f1-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessorganizeractivityminutecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7f7f1-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f7f1-159">Response</span></span>

<span data-ttu-id="7f7f1-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7f7f1-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="7f7f1-161">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="7f7f1-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video,Dial-in Microsoft,Dial-out Microsoft
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
