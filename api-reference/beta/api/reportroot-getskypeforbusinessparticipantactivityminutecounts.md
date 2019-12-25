---
title: 'reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts'
description: Obtenha as tendências de uso da duração em minutos e o tipo de sessões de conferência das quais os usuários de sua organização participaram. Tipos de sessões de conferência incluem áudio/vídeo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 18542fc96fbb706201c4398296e3fa1017dc062f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868986"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="5fe6e-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="5fe6e-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fe6e-105">Obtenha as tendências de uso da duração em minutos e o tipo de sessões de conferência das quais os usuários de sua organização participaram.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-105">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="5fe6e-106">Tipos de sessões de conferência incluem áudio/vídeo.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-106">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="5fe6e-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do participante da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="5fe6e-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="5fe6e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="5fe6e-108">Permissions</span></span>

<span data-ttu-id="5fe6e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fe6e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5fe6e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5fe6e-111">Permission type</span></span>                        | <span data-ttu-id="5fe6e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5fe6e-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5fe6e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5fe6e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5fe6e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5fe6e-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5fe6e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5fe6e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fe6e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-116">Not supported.</span></span>                           |
| <span data-ttu-id="5fe6e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5fe6e-117">Application</span></span>                            | <span data-ttu-id="5fe6e-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5fe6e-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="5fe6e-119">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5fe6e-120">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="5fe6e-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5fe6e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5fe6e-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5fe6e-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="5fe6e-122">Function parameters</span></span>

<span data-ttu-id="5fe6e-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5fe6e-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5fe6e-124">Parameter</span></span> | <span data-ttu-id="5fe6e-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="5fe6e-125">Type</span></span>   | <span data-ttu-id="5fe6e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fe6e-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5fe6e-127">ponto</span><span class="sxs-lookup"><span data-stu-id="5fe6e-127">period</span></span>    | <span data-ttu-id="5fe6e-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5fe6e-128">string</span></span> | <span data-ttu-id="5fe6e-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5fe6e-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5fe6e-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5fe6e-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-132">Required.</span></span> |

<span data-ttu-id="5fe6e-133">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5fe6e-134">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-134">The default output type is text/csv.</span></span> <span data-ttu-id="5fe6e-135">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5fe6e-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5fe6e-136">Request headers</span></span>

| <span data-ttu-id="5fe6e-137">Nome</span><span class="sxs-lookup"><span data-stu-id="5fe6e-137">Name</span></span>          | <span data-ttu-id="5fe6e-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fe6e-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5fe6e-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="5fe6e-139">Authorization</span></span> | <span data-ttu-id="5fe6e-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5fe6e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fe6e-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5fe6e-143">CSV</span><span class="sxs-lookup"><span data-stu-id="5fe6e-143">CSV</span></span>

<span data-ttu-id="5fe6e-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5fe6e-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5fe6e-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5fe6e-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5fe6e-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="5fe6e-148">Report Refresh Date</span></span>
- <span data-ttu-id="5fe6e-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="5fe6e-149">Report Date</span></span>
- <span data-ttu-id="5fe6e-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="5fe6e-150">Report Period</span></span>
- <span data-ttu-id="5fe6e-151">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="5fe6e-151">Audio/Video</span></span>

### <a name="json"></a><span data-ttu-id="5fe6e-152">JSON</span><span class="sxs-lookup"><span data-stu-id="5fe6e-152">JSON</span></span>

<span data-ttu-id="5fe6e-153">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-153">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fe6e-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5fe6e-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5fe6e-155">CSV</span><span class="sxs-lookup"><span data-stu-id="5fe6e-155">CSV</span></span>

<span data-ttu-id="5fe6e-156">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5fe6e-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5fe6e-157">Request</span></span>

<span data-ttu-id="5fe6e-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5fe6e-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="5fe6e-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5fe6e-160">C#</span><span class="sxs-lookup"><span data-stu-id="5fe6e-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivityminutecounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5fe6e-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5fe6e-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivityminutecounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5fe6e-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5fe6e-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivityminutecounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5fe6e-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fe6e-163">Response</span></span>

<span data-ttu-id="5fe6e-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5fe6e-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video
```

### <a name="json"></a><span data-ttu-id="5fe6e-166">JSON</span><span class="sxs-lookup"><span data-stu-id="5fe6e-166">JSON</span></span>

<span data-ttu-id="5fe6e-167">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5fe6e-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5fe6e-168">Request</span></span>

<span data-ttu-id="5fe6e-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5fe6e-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="5fe6e-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5fe6e-171">C#</span><span class="sxs-lookup"><span data-stu-id="5fe6e-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessparticipantactivityminutecounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5fe6e-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5fe6e-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessparticipantactivityminutecounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5fe6e-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5fe6e-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessparticipantactivityminutecounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5fe6e-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fe6e-174">Response</span></span>

<span data-ttu-id="5fe6e-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-175">The following is an example of the response.</span></span>

> <span data-ttu-id="5fe6e-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5fe6e-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityMinuteCounts)", 
  "value": [
    {
      "audiovideo": 6267, 
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
