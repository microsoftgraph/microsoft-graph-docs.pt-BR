---
title: 'reportRoot: getSkypeForBusinessParticipantActivityUserCounts'
description: Obtenha tendências de uso do número de usuários únicos e o tipo de sessões de conferência das quais os usuários de sua organização participaram. Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a67571f7e4a407eabf67f05def1cde64a17212e7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871941"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityusercounts"></a><span data-ttu-id="1777e-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="1777e-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1777e-105">Obtenha tendências de uso do número de usuários únicos e o tipo de sessões de conferência das quais os usuários de sua organização participaram.</span><span class="sxs-lookup"><span data-stu-id="1777e-105">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="1777e-106">Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros.</span><span class="sxs-lookup"><span data-stu-id="1777e-106">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="1777e-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do participante da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="1777e-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="1777e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1777e-108">Permissions</span></span>

<span data-ttu-id="1777e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1777e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1777e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1777e-111">Permission type</span></span>                        | <span data-ttu-id="1777e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1777e-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1777e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1777e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1777e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1777e-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1777e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1777e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1777e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1777e-116">Not supported.</span></span>                           |
| <span data-ttu-id="1777e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1777e-117">Application</span></span>                            | <span data-ttu-id="1777e-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1777e-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1777e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1777e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1777e-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="1777e-120">Function parameters</span></span>

<span data-ttu-id="1777e-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="1777e-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1777e-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1777e-122">Parameter</span></span> | <span data-ttu-id="1777e-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="1777e-123">Type</span></span>   | <span data-ttu-id="1777e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1777e-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1777e-125">ponto</span><span class="sxs-lookup"><span data-stu-id="1777e-125">period</span></span>    | <span data-ttu-id="1777e-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1777e-126">string</span></span> | <span data-ttu-id="1777e-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1777e-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1777e-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="1777e-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1777e-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1777e-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1777e-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1777e-130">Required.</span></span> |

<span data-ttu-id="1777e-131">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1777e-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1777e-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="1777e-132">The default output type is text/csv.</span></span> <span data-ttu-id="1777e-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="1777e-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1777e-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1777e-134">Request headers</span></span>

| <span data-ttu-id="1777e-135">Nome</span><span class="sxs-lookup"><span data-stu-id="1777e-135">Name</span></span>          | <span data-ttu-id="1777e-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="1777e-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1777e-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="1777e-137">Authorization</span></span> | <span data-ttu-id="1777e-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1777e-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1777e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1777e-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1777e-141">CSV</span><span class="sxs-lookup"><span data-stu-id="1777e-141">CSV</span></span>

<span data-ttu-id="1777e-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="1777e-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1777e-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="1777e-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1777e-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1777e-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1777e-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="1777e-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1777e-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="1777e-146">Report Refresh Date</span></span>
- <span data-ttu-id="1777e-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="1777e-147">Report Date</span></span>
- <span data-ttu-id="1777e-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="1777e-148">Report Period</span></span>
- <span data-ttu-id="1777e-149">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="1777e-149">IM</span></span>
- <span data-ttu-id="1777e-150">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="1777e-150">Audio/Video</span></span>
- <span data-ttu-id="1777e-151">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="1777e-151">App Sharing</span></span>
- <span data-ttu-id="1777e-152">Web</span><span class="sxs-lookup"><span data-stu-id="1777e-152">Web</span></span>
- <span data-ttu-id="1777e-153">Dial-in/out por terceiros</span><span class="sxs-lookup"><span data-stu-id="1777e-153">Dial-in/out 3rd Party</span></span>

### <a name="json"></a><span data-ttu-id="1777e-154">JSON</span><span class="sxs-lookup"><span data-stu-id="1777e-154">JSON</span></span>

<span data-ttu-id="1777e-155">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1777e-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1777e-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1777e-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1777e-157">CSV</span><span class="sxs-lookup"><span data-stu-id="1777e-157">CSV</span></span>

<span data-ttu-id="1777e-158">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="1777e-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1777e-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1777e-159">Request</span></span>

<span data-ttu-id="1777e-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1777e-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1777e-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="1777e-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1777e-162">C#</span><span class="sxs-lookup"><span data-stu-id="1777e-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1777e-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="1777e-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1777e-164">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1777e-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1777e-165">Java</span><span class="sxs-lookup"><span data-stu-id="1777e-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessparticipantactivityusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1777e-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="1777e-166">Response</span></span>

<span data-ttu-id="1777e-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1777e-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1777e-168">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="1777e-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
```

### <a name="json"></a><span data-ttu-id="1777e-169">JSON</span><span class="sxs-lookup"><span data-stu-id="1777e-169">JSON</span></span>

<span data-ttu-id="1777e-170">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="1777e-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1777e-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1777e-171">Request</span></span>

<span data-ttu-id="1777e-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1777e-172">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1777e-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="1777e-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1777e-174">C#</span><span class="sxs-lookup"><span data-stu-id="1777e-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1777e-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="1777e-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1777e-176">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1777e-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1777e-177">Java</span><span class="sxs-lookup"><span data-stu-id="1777e-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessparticipantactivityusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1777e-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="1777e-178">Response</span></span>

<span data-ttu-id="1777e-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1777e-179">The following is an example of the response.</span></span>

> <span data-ttu-id="1777e-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1777e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 301

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityUserCounts)", 
  "value": [
    {
      "im": 137, 
      "audioVideo": 196, 
      "appSharing": 214, 
      "web": 30, 
      "dialInOut3rdParty": 2, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
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
