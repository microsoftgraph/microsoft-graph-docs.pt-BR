---
title: 'reportRoot: getSkypeForBusinessActivityCounts'
description: Obtenha as tendências de quantos usuários organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business. O relatório também inclui o número de sessões ponto a ponto.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e570e0169743ebcf5d6814329563fe503a0a9c31
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869011"
---
# <a name="reportroot-getskypeforbusinessactivitycounts"></a><span data-ttu-id="25a6f-104">reportRoot: getSkypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="25a6f-104">reportRoot: getSkypeForBusinessActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25a6f-105">Obtenha as tendências de quantos usuários organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="25a6f-105">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="25a6f-106">O relatório também inclui o número de sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="25a6f-106">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="25a6f-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="25a6f-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="25a6f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="25a6f-108">Permissions</span></span>

<span data-ttu-id="25a6f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25a6f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="25a6f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25a6f-111">Permission type</span></span>                        | <span data-ttu-id="25a6f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25a6f-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="25a6f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25a6f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="25a6f-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="25a6f-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="25a6f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25a6f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25a6f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25a6f-116">Not supported.</span></span>                           |
| <span data-ttu-id="25a6f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25a6f-117">Application</span></span>                            | <span data-ttu-id="25a6f-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="25a6f-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="25a6f-119">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="25a6f-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="25a6f-120">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="25a6f-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="25a6f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25a6f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="25a6f-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="25a6f-122">Function parameters</span></span>

<span data-ttu-id="25a6f-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="25a6f-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="25a6f-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="25a6f-124">Parameter</span></span> | <span data-ttu-id="25a6f-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="25a6f-125">Type</span></span>   | <span data-ttu-id="25a6f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="25a6f-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="25a6f-127">ponto</span><span class="sxs-lookup"><span data-stu-id="25a6f-127">period</span></span>    | <span data-ttu-id="25a6f-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25a6f-128">string</span></span> | <span data-ttu-id="25a6f-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="25a6f-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="25a6f-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="25a6f-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="25a6f-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="25a6f-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="25a6f-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25a6f-132">Required.</span></span> |

<span data-ttu-id="25a6f-133">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="25a6f-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="25a6f-134">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="25a6f-134">The default output type is text/csv.</span></span> <span data-ttu-id="25a6f-135">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="25a6f-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25a6f-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25a6f-136">Request headers</span></span>

| <span data-ttu-id="25a6f-137">Nome</span><span class="sxs-lookup"><span data-stu-id="25a6f-137">Name</span></span>          | <span data-ttu-id="25a6f-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="25a6f-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="25a6f-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="25a6f-139">Authorization</span></span> | <span data-ttu-id="25a6f-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25a6f-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="25a6f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="25a6f-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="25a6f-143">CSV</span><span class="sxs-lookup"><span data-stu-id="25a6f-143">CSV</span></span>

<span data-ttu-id="25a6f-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="25a6f-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="25a6f-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="25a6f-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="25a6f-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="25a6f-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="25a6f-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="25a6f-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="25a6f-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="25a6f-148">Report Refresh Date</span></span>
- <span data-ttu-id="25a6f-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="25a6f-149">Report Date</span></span>
- <span data-ttu-id="25a6f-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="25a6f-150">Report Period</span></span>
- <span data-ttu-id="25a6f-151">Ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="25a6f-151">Peer-to-peer</span></span>
- <span data-ttu-id="25a6f-152">Organizadas</span><span class="sxs-lookup"><span data-stu-id="25a6f-152">Organized</span></span>
- <span data-ttu-id="25a6f-153">Participadas</span><span class="sxs-lookup"><span data-stu-id="25a6f-153">Participated</span></span>

### <a name="json"></a><span data-ttu-id="25a6f-154">JSON</span><span class="sxs-lookup"><span data-stu-id="25a6f-154">JSON</span></span>

<span data-ttu-id="25a6f-155">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25a6f-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25a6f-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25a6f-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="25a6f-157">CSV</span><span class="sxs-lookup"><span data-stu-id="25a6f-157">CSV</span></span>

<span data-ttu-id="25a6f-158">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="25a6f-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="25a6f-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25a6f-159">Request</span></span>

<span data-ttu-id="25a6f-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="25a6f-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="25a6f-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="25a6f-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="25a6f-162">C#</span><span class="sxs-lookup"><span data-stu-id="25a6f-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="25a6f-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25a6f-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="25a6f-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25a6f-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="25a6f-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="25a6f-165">Response</span></span>

<span data-ttu-id="25a6f-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="25a6f-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="25a6f-167">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="25a6f-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
```

### <a name="json"></a><span data-ttu-id="25a6f-168">JSON</span><span class="sxs-lookup"><span data-stu-id="25a6f-168">JSON</span></span>

<span data-ttu-id="25a6f-169">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="25a6f-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="25a6f-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25a6f-170">Request</span></span>

<span data-ttu-id="25a6f-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="25a6f-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="25a6f-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="25a6f-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="25a6f-173">C#</span><span class="sxs-lookup"><span data-stu-id="25a6f-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="25a6f-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25a6f-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="25a6f-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25a6f-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="25a6f-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="25a6f-176">Response</span></span>

<span data-ttu-id="25a6f-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="25a6f-177">The following is an example of the response.</span></span>

> <span data-ttu-id="25a6f-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25a6f-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 264

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessActivityCounts)", 
  "value": [
    {
      "peerToPeer": 3436, 
      "organized": 58, 
      "participated": 209, 
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
