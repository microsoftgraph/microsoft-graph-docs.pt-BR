---
title: 'reportRoot: getEmailActivityUserCounts'
description: Permite que você compreenda as tendências do número de usuários únicos que estão executando atividades de email, como enviar, ler e receber.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: cf4a310e18cb8f9d9c4cf3a3d6e0a10ed11d7383
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867618"
---
# <a name="reportroot-getemailactivityusercounts"></a><span data-ttu-id="2b043-103">reportRoot: getEmailActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="2b043-103">reportRoot: getEmailActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b043-104">Permite que você compreenda as tendências do número de usuários únicos que estão executando atividades de email, como enviar, ler e receber.</span><span class="sxs-lookup"><span data-stu-id="2b043-104">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span>

> <span data-ttu-id="2b043-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="2b043-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="2b043-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2b043-106">Permissions</span></span>

<span data-ttu-id="2b043-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b043-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2b043-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b043-109">Permission type</span></span>                        | <span data-ttu-id="2b043-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b043-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2b043-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b043-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2b043-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b043-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2b043-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b043-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b043-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b043-114">Not supported.</span></span>                           |
| <span data-ttu-id="2b043-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b043-115">Application</span></span>                            | <span data-ttu-id="2b043-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b043-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="2b043-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="2b043-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="2b043-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="2b043-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="2b043-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b043-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="2b043-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="2b043-120">Function parameters</span></span>

<span data-ttu-id="2b043-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="2b043-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2b043-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2b043-122">Parameter</span></span> | <span data-ttu-id="2b043-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b043-123">Type</span></span>   | <span data-ttu-id="2b043-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b043-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2b043-125">ponto</span><span class="sxs-lookup"><span data-stu-id="2b043-125">period</span></span>    | <span data-ttu-id="2b043-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2b043-126">string</span></span> | <span data-ttu-id="2b043-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="2b043-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2b043-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="2b043-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2b043-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="2b043-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2b043-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b043-130">Required.</span></span> |

<span data-ttu-id="2b043-131">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2b043-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2b043-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="2b043-132">The default output type is text/csv.</span></span> <span data-ttu-id="2b043-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="2b043-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b043-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b043-134">Request headers</span></span>

| <span data-ttu-id="2b043-135">Nome</span><span class="sxs-lookup"><span data-stu-id="2b043-135">Name</span></span>          | <span data-ttu-id="2b043-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b043-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2b043-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b043-137">Authorization</span></span> | <span data-ttu-id="2b043-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b043-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2b043-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b043-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="2b043-141">CSV</span><span class="sxs-lookup"><span data-stu-id="2b043-141">CSV</span></span>

<span data-ttu-id="2b043-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="2b043-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2b043-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="2b043-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2b043-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2b043-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2b043-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="2b043-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2b043-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="2b043-146">Report Refresh Date</span></span>
- <span data-ttu-id="2b043-147">Enviar</span><span class="sxs-lookup"><span data-stu-id="2b043-147">Send</span></span>
- <span data-ttu-id="2b043-148">Receber</span><span class="sxs-lookup"><span data-stu-id="2b043-148">Receive</span></span>
- <span data-ttu-id="2b043-149">Ler</span><span class="sxs-lookup"><span data-stu-id="2b043-149">Read</span></span>
- <span data-ttu-id="2b043-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="2b043-150">Report Date</span></span>
- <span data-ttu-id="2b043-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="2b043-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="2b043-152">JSON</span><span class="sxs-lookup"><span data-stu-id="2b043-152">JSON</span></span>

<span data-ttu-id="2b043-153">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[emailActivitySummary](../resources/emailactivitysummary.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b043-153">If successful, this method returns a `200 OK` response code and an **[emailActivitySummary](../resources/emailactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b043-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b043-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="2b043-155">CSV</span><span class="sxs-lookup"><span data-stu-id="2b043-155">CSV</span></span>

<span data-ttu-id="2b043-156">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="2b043-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2b043-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b043-157">Request</span></span>

<span data-ttu-id="2b043-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b043-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2b043-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b043-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2b043-160">C#</span><span class="sxs-lookup"><span data-stu-id="2b043-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2b043-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b043-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2b043-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b043-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2b043-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b043-163">Response</span></span>

<span data-ttu-id="2b043-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2b043-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2b043-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="2b043-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="2b043-166">JSON</span><span class="sxs-lookup"><span data-stu-id="2b043-166">JSON</span></span>

<span data-ttu-id="2b043-167">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="2b043-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2b043-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b043-168">Request</span></span>

<span data-ttu-id="2b043-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b043-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2b043-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b043-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2b043-171">C#</span><span class="sxs-lookup"><span data-stu-id="2b043-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2b043-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b043-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2b043-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b043-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2b043-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b043-174">Response</span></span>

<span data-ttu-id="2b043-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2b043-175">The following is an example of the response.</span></span>

> <span data-ttu-id="2b043-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b043-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "send": 69, 
      "receive": 197, 
      "read": 158, 
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
