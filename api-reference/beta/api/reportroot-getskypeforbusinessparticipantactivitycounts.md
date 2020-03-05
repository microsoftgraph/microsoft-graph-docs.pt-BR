---
title: 'reportRoot: getSkypeForBusinessParticipantActivityCounts'
description: Obtenha tendências de uso do número e o tipo de sessões de conferência das quais os usuários de sua organização participaram. Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7e8f1c3078fd49e5442bc7db968b0cf5641ab7e2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454091"
---
# <a name="reportroot-getskypeforbusinessparticipantactivitycounts"></a><span data-ttu-id="192b1-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span><span class="sxs-lookup"><span data-stu-id="192b1-104">reportRoot: getSkypeForBusinessParticipantActivityCounts</span></span>

<span data-ttu-id="192b1-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="192b1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="192b1-106">Obtenha tendências de uso do número e o tipo de sessões de conferência das quais os usuários de sua organização participaram.</span><span class="sxs-lookup"><span data-stu-id="192b1-106">Get usage trends on the number and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="192b1-107">Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros.</span><span class="sxs-lookup"><span data-stu-id="192b1-107">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="192b1-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do participante da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="192b1-108">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="192b1-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="192b1-109">Permissions</span></span>

<span data-ttu-id="192b1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="192b1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="192b1-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="192b1-112">Permission type</span></span>                        | <span data-ttu-id="192b1-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="192b1-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="192b1-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="192b1-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="192b1-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="192b1-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="192b1-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="192b1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="192b1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="192b1-117">Not supported.</span></span>                           |
| <span data-ttu-id="192b1-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="192b1-118">Application</span></span>                            | <span data-ttu-id="192b1-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="192b1-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="192b1-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="192b1-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="192b1-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="192b1-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="192b1-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="192b1-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="192b1-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="192b1-123">Function parameters</span></span>

<span data-ttu-id="192b1-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="192b1-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="192b1-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="192b1-125">Parameter</span></span> | <span data-ttu-id="192b1-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="192b1-126">Type</span></span>   | <span data-ttu-id="192b1-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="192b1-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="192b1-128">ponto</span><span class="sxs-lookup"><span data-stu-id="192b1-128">period</span></span>    | <span data-ttu-id="192b1-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="192b1-129">string</span></span> | <span data-ttu-id="192b1-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="192b1-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="192b1-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="192b1-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="192b1-132">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="192b1-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="192b1-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="192b1-133">Required.</span></span> |

<span data-ttu-id="192b1-134">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="192b1-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="192b1-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="192b1-135">The default output type is text/csv.</span></span> <span data-ttu-id="192b1-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="192b1-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="192b1-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="192b1-137">Request headers</span></span>

| <span data-ttu-id="192b1-138">Nome</span><span class="sxs-lookup"><span data-stu-id="192b1-138">Name</span></span>          | <span data-ttu-id="192b1-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="192b1-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="192b1-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="192b1-140">Authorization</span></span> | <span data-ttu-id="192b1-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="192b1-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="192b1-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="192b1-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="192b1-144">CSV</span><span class="sxs-lookup"><span data-stu-id="192b1-144">CSV</span></span>

<span data-ttu-id="192b1-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="192b1-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="192b1-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="192b1-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="192b1-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="192b1-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="192b1-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="192b1-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="192b1-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="192b1-149">Report Refresh Date</span></span>
- <span data-ttu-id="192b1-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="192b1-150">Report Date</span></span>
- <span data-ttu-id="192b1-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="192b1-151">Report Period</span></span>
- <span data-ttu-id="192b1-152">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="192b1-152">IM</span></span>
- <span data-ttu-id="192b1-153">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="192b1-153">Audio/Video</span></span>
- <span data-ttu-id="192b1-154">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="192b1-154">App Sharing</span></span>
- <span data-ttu-id="192b1-155">Web</span><span class="sxs-lookup"><span data-stu-id="192b1-155">Web</span></span>
- <span data-ttu-id="192b1-156">Dial-in/out por terceiros</span><span class="sxs-lookup"><span data-stu-id="192b1-156">Dial-in/out 3rd Party</span></span>

### <a name="json"></a><span data-ttu-id="192b1-157">JSON</span><span class="sxs-lookup"><span data-stu-id="192b1-157">JSON</span></span>

<span data-ttu-id="192b1-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="192b1-158">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="192b1-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="192b1-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="192b1-160">CSV</span><span class="sxs-lookup"><span data-stu-id="192b1-160">CSV</span></span>

<span data-ttu-id="192b1-161">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="192b1-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="192b1-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="192b1-162">Request</span></span>

<span data-ttu-id="192b1-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="192b1-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="192b1-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="192b1-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="192b1-165">C#</span><span class="sxs-lookup"><span data-stu-id="192b1-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="192b1-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="192b1-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="192b1-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="192b1-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="192b1-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="192b1-168">Response</span></span>

<span data-ttu-id="192b1-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="192b1-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="192b1-170">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="192b1-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="192b1-171">JSON</span><span class="sxs-lookup"><span data-stu-id="192b1-171">JSON</span></span>

<span data-ttu-id="192b1-172">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="192b1-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="192b1-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="192b1-173">Request</span></span>

<span data-ttu-id="192b1-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="192b1-174">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="192b1-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="192b1-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="192b1-176">C#</span><span class="sxs-lookup"><span data-stu-id="192b1-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="192b1-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="192b1-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="192b1-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="192b1-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="192b1-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="192b1-179">Response</span></span>

<span data-ttu-id="192b1-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="192b1-180">The following is an example of the response.</span></span>

> <span data-ttu-id="192b1-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="192b1-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 296

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityCounts)", 
  "value": [
    {
      "im": 162, 
      "audioVideo": 156, 
      "appSharing": 45, 
      "web": 12, 
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
