---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts'
description: Obtenha tendências de uso do número de usuários únicos e o tipo de sessões ponto a ponto realizadas em sua organização. Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos em sessões ponto a ponto.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 498be215e2746b0088b5449900d70bdb245696b8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460830"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityusercounts"></a><span data-ttu-id="490e4-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="490e4-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span></span>

<span data-ttu-id="490e4-105">Obtenha tendências de uso do número de usuários únicos e o tipo de sessões ponto a ponto realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="490e4-105">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="490e4-106">Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos em sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="490e4-106">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span>

> <span data-ttu-id="490e4-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade ponto a ponto do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="490e4-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="490e4-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="490e4-108">Permissions</span></span>

<span data-ttu-id="490e4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="490e4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="490e4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="490e4-111">Permission type</span></span>                        | <span data-ttu-id="490e4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="490e4-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="490e4-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="490e4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="490e4-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="490e4-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="490e4-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="490e4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="490e4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="490e4-116">Not supported.</span></span>                           |
| <span data-ttu-id="490e4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="490e4-117">Application</span></span>                            | <span data-ttu-id="490e4-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="490e4-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="490e4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="490e4-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="490e4-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="490e4-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="490e4-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="490e4-121">Function parameters</span></span>

<span data-ttu-id="490e4-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="490e4-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="490e4-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="490e4-123">Parameter</span></span> | <span data-ttu-id="490e4-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="490e4-124">Type</span></span>   | <span data-ttu-id="490e4-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="490e4-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="490e4-126">ponto</span><span class="sxs-lookup"><span data-stu-id="490e4-126">period</span></span>    | <span data-ttu-id="490e4-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="490e4-127">string</span></span> | <span data-ttu-id="490e4-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="490e4-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="490e4-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="490e4-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="490e4-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="490e4-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="490e4-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="490e4-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="490e4-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="490e4-132">Request headers</span></span>

| <span data-ttu-id="490e4-133">Nome</span><span class="sxs-lookup"><span data-stu-id="490e4-133">Name</span></span>          | <span data-ttu-id="490e4-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="490e4-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="490e4-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="490e4-135">Authorization</span></span> | <span data-ttu-id="490e4-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="490e4-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="490e4-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="490e4-138">If-None-Match</span></span> | <span data-ttu-id="490e4-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="490e4-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="490e4-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="490e4-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="490e4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="490e4-141">Response</span></span>

<span data-ttu-id="490e4-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="490e4-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="490e4-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="490e4-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="490e4-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="490e4-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="490e4-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="490e4-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="490e4-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="490e4-146">Report Refresh Date</span></span>
- <span data-ttu-id="490e4-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="490e4-147">Report Date</span></span>
- <span data-ttu-id="490e4-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="490e4-148">Report Period</span></span>
- <span data-ttu-id="490e4-149">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="490e4-149">IM</span></span>
- <span data-ttu-id="490e4-150">Áudio</span><span class="sxs-lookup"><span data-stu-id="490e4-150">Audio</span></span>
- <span data-ttu-id="490e4-151">Vídeo</span><span class="sxs-lookup"><span data-stu-id="490e4-151">Video</span></span>
- <span data-ttu-id="490e4-152">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="490e4-152">App Sharing</span></span>
- <span data-ttu-id="490e4-153">Transferência de arquivos</span><span class="sxs-lookup"><span data-stu-id="490e4-153">File Transfer</span></span>

## <a name="example"></a><span data-ttu-id="490e4-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="490e4-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="490e4-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="490e4-155">Request</span></span>

<span data-ttu-id="490e4-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="490e4-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="490e4-157">C#</span><span class="sxs-lookup"><span data-stu-id="490e4-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="490e4-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="490e4-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="490e4-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="490e4-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="490e4-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="490e4-160">Response</span></span>

<span data-ttu-id="490e4-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="490e4-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="490e4-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="490e4-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
