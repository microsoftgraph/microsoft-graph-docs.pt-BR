---
title: 'reportRoot: getTeamsDeviceUsageUserCounts'
description: Obtém o número de usuários exclusivos diários do Microsoft Teams por tipo de dispositivo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 19063262c586144e57c507bd078fd6996d0ab0e4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454049"
---
# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="5f1f9-103">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="5f1f9-103">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

<span data-ttu-id="5f1f9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5f1f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f1f9-105">Obtém o número de usuários exclusivos diários do Microsoft Teams por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-105">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f1f9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f1f9-106">Permissions</span></span>

<span data-ttu-id="5f1f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f1f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5f1f9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f1f9-109">Permission type</span></span>                        | <span data-ttu-id="5f1f9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f1f9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5f1f9-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f1f9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f1f9-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f1f9-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5f1f9-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f1f9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f1f9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-114">Not supported.</span></span>                           |
| <span data-ttu-id="5f1f9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f1f9-115">Application</span></span>                            | <span data-ttu-id="5f1f9-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f1f9-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="5f1f9-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5f1f9-118">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="5f1f9-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5f1f9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f1f9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="5f1f9-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="5f1f9-120">Function parameters</span></span>

<span data-ttu-id="5f1f9-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5f1f9-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5f1f9-122">Parameter</span></span> | <span data-ttu-id="5f1f9-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f1f9-123">Type</span></span>   | <span data-ttu-id="5f1f9-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f1f9-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5f1f9-125">ponto</span><span class="sxs-lookup"><span data-stu-id="5f1f9-125">period</span></span>    | <span data-ttu-id="5f1f9-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f1f9-126">string</span></span> | <span data-ttu-id="5f1f9-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5f1f9-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5f1f9-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5f1f9-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-130">Required.</span></span> |

<span data-ttu-id="5f1f9-131">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5f1f9-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-132">The default output type is text/csv.</span></span> <span data-ttu-id="5f1f9-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f1f9-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f1f9-134">Request headers</span></span>

| <span data-ttu-id="5f1f9-135">Nome</span><span class="sxs-lookup"><span data-stu-id="5f1f9-135">Name</span></span>          | <span data-ttu-id="5f1f9-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f1f9-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5f1f9-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f1f9-137">Authorization</span></span> | <span data-ttu-id="5f1f9-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5f1f9-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f1f9-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5f1f9-141">CSV</span><span class="sxs-lookup"><span data-stu-id="5f1f9-141">CSV</span></span>

<span data-ttu-id="5f1f9-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5f1f9-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5f1f9-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5f1f9-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5f1f9-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="5f1f9-146">Report Refresh Date</span></span>
- <span data-ttu-id="5f1f9-147">Web</span><span class="sxs-lookup"><span data-stu-id="5f1f9-147">Web</span></span>
- <span data-ttu-id="5f1f9-148">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="5f1f9-148">Windows Phone</span></span>
- <span data-ttu-id="5f1f9-149">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="5f1f9-149">Android Phone</span></span>
- <span data-ttu-id="5f1f9-150">iOS</span><span class="sxs-lookup"><span data-stu-id="5f1f9-150">iOS</span></span>
- <span data-ttu-id="5f1f9-151">Mac</span><span class="sxs-lookup"><span data-stu-id="5f1f9-151">Mac</span></span>
- <span data-ttu-id="5f1f9-152">Windows</span><span class="sxs-lookup"><span data-stu-id="5f1f9-152">Windows</span></span>
- <span data-ttu-id="5f1f9-153">Data do Relatório</span><span class="sxs-lookup"><span data-stu-id="5f1f9-153">Report Date</span></span>
- <span data-ttu-id="5f1f9-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="5f1f9-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="5f1f9-155">JSON</span><span class="sxs-lookup"><span data-stu-id="5f1f9-155">JSON</span></span>

<span data-ttu-id="5f1f9-156">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-156">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f1f9-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f1f9-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5f1f9-158">CSV</span><span class="sxs-lookup"><span data-stu-id="5f1f9-158">CSV</span></span>

<span data-ttu-id="5f1f9-159">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5f1f9-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f1f9-160">Request</span></span>

<span data-ttu-id="5f1f9-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5f1f9-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f1f9-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="5f1f9-163">C#</span><span class="sxs-lookup"><span data-stu-id="5f1f9-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f1f9-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f1f9-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f1f9-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f1f9-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5f1f9-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f1f9-166">Response</span></span>

<span data-ttu-id="5f1f9-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5f1f9-168">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="5f1f9-169">JSON</span><span class="sxs-lookup"><span data-stu-id="5f1f9-169">JSON</span></span>

<span data-ttu-id="5f1f9-170">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5f1f9-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f1f9-171">Request</span></span>

<span data-ttu-id="5f1f9-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-172">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5f1f9-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f1f9-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="5f1f9-174">C#</span><span class="sxs-lookup"><span data-stu-id="5f1f9-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f1f9-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f1f9-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f1f9-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f1f9-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5f1f9-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f1f9-177">Response</span></span>

<span data-ttu-id="5f1f9-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-178">The following is an example of the response.</span></span>

> <span data-ttu-id="5f1f9-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f1f9-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 13, 
      "windowsPhone": 0, 
      "androidPhone": 22, 
      "ios": 75, 
      "mac": 16, 
      "windows": 257, 
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
