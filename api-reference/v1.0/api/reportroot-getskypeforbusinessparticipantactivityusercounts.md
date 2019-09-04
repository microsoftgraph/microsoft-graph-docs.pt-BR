---
title: 'reportRoot: getSkypeForBusinessParticipantActivityUserCounts'
description: Obtenha tendências de uso do número de usuários únicos e o tipo de sessões de conferência das quais os usuários de sua organização participaram. Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 2a73741fb93a6fabcbf68de55ef2280ed5cc985b
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729473"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityusercounts"></a><span data-ttu-id="1b4d0-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="1b4d0-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span></span>

<span data-ttu-id="1b4d0-105">Obtenha tendências de uso do número de usuários únicos e o tipo de sessões de conferência das quais os usuários de sua organização participaram.</span><span class="sxs-lookup"><span data-stu-id="1b4d0-105">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="1b4d0-106">Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros.</span><span class="sxs-lookup"><span data-stu-id="1b4d0-106">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="1b4d0-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do participante da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="1b4d0-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="1b4d0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b4d0-108">Permissions</span></span>

<span data-ttu-id="1b4d0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b4d0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1b4d0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b4d0-111">Permission type</span></span>                        | <span data-ttu-id="1b4d0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b4d0-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1b4d0-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b4d0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1b4d0-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b4d0-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1b4d0-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b4d0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b4d0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b4d0-116">Not supported.</span></span>                           |
| <span data-ttu-id="1b4d0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b4d0-117">Application</span></span>                            | <span data-ttu-id="1b4d0-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b4d0-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1b4d0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b4d0-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1b4d0-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="1b4d0-120">Function parameters</span></span>

<span data-ttu-id="1b4d0-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="1b4d0-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1b4d0-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1b4d0-122">Parameter</span></span> | <span data-ttu-id="1b4d0-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b4d0-123">Type</span></span>   | <span data-ttu-id="1b4d0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b4d0-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1b4d0-125">ponto</span><span class="sxs-lookup"><span data-stu-id="1b4d0-125">period</span></span>    | <span data-ttu-id="1b4d0-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b4d0-126">string</span></span> | <span data-ttu-id="1b4d0-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1b4d0-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1b4d0-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="1b4d0-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1b4d0-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1b4d0-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1b4d0-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b4d0-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="1b4d0-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b4d0-131">Request headers</span></span>

| <span data-ttu-id="1b4d0-132">Nome</span><span class="sxs-lookup"><span data-stu-id="1b4d0-132">Name</span></span>          | <span data-ttu-id="1b4d0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b4d0-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="1b4d0-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b4d0-134">Authorization</span></span> | <span data-ttu-id="1b4d0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b4d0-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="1b4d0-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="1b4d0-137">If-None-Match</span></span> | <span data-ttu-id="1b4d0-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="1b4d0-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="1b4d0-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1b4d0-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="1b4d0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b4d0-140">Response</span></span>

<span data-ttu-id="1b4d0-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="1b4d0-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1b4d0-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="1b4d0-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1b4d0-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1b4d0-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1b4d0-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="1b4d0-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1b4d0-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="1b4d0-145">Report Refresh Date</span></span>
- <span data-ttu-id="1b4d0-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="1b4d0-146">Report Date</span></span>
- <span data-ttu-id="1b4d0-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="1b4d0-147">Report Period</span></span>
- <span data-ttu-id="1b4d0-148">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="1b4d0-148">IM</span></span>
- <span data-ttu-id="1b4d0-149">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="1b4d0-149">Audio/Video</span></span>
- <span data-ttu-id="1b4d0-150">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="1b4d0-150">App Sharing</span></span>
- <span data-ttu-id="1b4d0-151">Web</span><span class="sxs-lookup"><span data-stu-id="1b4d0-151">Web</span></span>
- <span data-ttu-id="1b4d0-152">Dial-in/out por terceiros</span><span class="sxs-lookup"><span data-stu-id="1b4d0-152">Dial-in/out 3rd Party</span></span>

## <a name="example"></a><span data-ttu-id="1b4d0-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b4d0-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1b4d0-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b4d0-154">Request</span></span>

<span data-ttu-id="1b4d0-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b4d0-155">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1b4d0-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b4d0-156">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1b4d0-157">C#</span><span class="sxs-lookup"><span data-stu-id="1b4d0-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1b4d0-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b4d0-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1b4d0-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1b4d0-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1b4d0-160">Java</span><span class="sxs-lookup"><span data-stu-id="1b4d0-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessparticipantactivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1b4d0-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b4d0-161">Response</span></span>

<span data-ttu-id="1b4d0-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1b4d0-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="1b4d0-163">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="1b4d0-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
