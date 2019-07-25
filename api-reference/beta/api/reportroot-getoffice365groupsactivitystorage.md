---
title: 'reportRoot: getOffice365GroupsActivityStorage'
description: Obtenha o armazenamento total usado em todas as caixas de correio de grupo e sites de grupo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: acdb27f2b331706d625ea2dc42d7e14636d253b9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873254"
---
# <a name="reportroot-getoffice365groupsactivitystorage"></a><span data-ttu-id="7bc76-103">reportRoot: getOffice365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="7bc76-103">reportRoot: getOffice365GroupsActivityStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bc76-104">Obtenha o armazenamento total usado em todas as caixas de correio de grupo e sites de grupo.</span><span class="sxs-lookup"><span data-stu-id="7bc76-104">Get the total storage used across all group mailboxes and group sites.</span></span>

> <span data-ttu-id="7bc76-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="7bc76-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="7bc76-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7bc76-106">Permissions</span></span>

<span data-ttu-id="7bc76-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bc76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7bc76-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bc76-109">Permission type</span></span>                        | <span data-ttu-id="7bc76-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7bc76-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7bc76-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bc76-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7bc76-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7bc76-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7bc76-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bc76-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bc76-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bc76-114">Not supported.</span></span>                           |
| <span data-ttu-id="7bc76-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bc76-115">Application</span></span>                            | <span data-ttu-id="7bc76-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7bc76-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7bc76-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7bc76-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="7bc76-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="7bc76-118">Function parameters</span></span>

<span data-ttu-id="7bc76-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="7bc76-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7bc76-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7bc76-120">Parameter</span></span> | <span data-ttu-id="7bc76-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bc76-121">Type</span></span>   | <span data-ttu-id="7bc76-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bc76-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7bc76-123">ponto</span><span class="sxs-lookup"><span data-stu-id="7bc76-123">period</span></span>    | <span data-ttu-id="7bc76-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bc76-124">string</span></span> | <span data-ttu-id="7bc76-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7bc76-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7bc76-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="7bc76-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7bc76-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7bc76-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7bc76-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bc76-128">Required.</span></span> |

<span data-ttu-id="7bc76-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7bc76-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7bc76-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="7bc76-130">The default output type is text/csv.</span></span> <span data-ttu-id="7bc76-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="7bc76-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7bc76-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7bc76-132">Request headers</span></span>

| <span data-ttu-id="7bc76-133">Nome</span><span class="sxs-lookup"><span data-stu-id="7bc76-133">Name</span></span>          | <span data-ttu-id="7bc76-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bc76-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7bc76-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="7bc76-135">Authorization</span></span> | <span data-ttu-id="7bc76-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bc76-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7bc76-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bc76-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7bc76-139">CSV</span><span class="sxs-lookup"><span data-stu-id="7bc76-139">CSV</span></span>

<span data-ttu-id="7bc76-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="7bc76-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7bc76-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="7bc76-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7bc76-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7bc76-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7bc76-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="7bc76-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7bc76-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="7bc76-144">Report Refresh Date</span></span>
- <span data-ttu-id="7bc76-145">Armazenamento de caixa de correio utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="7bc76-145">Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="7bc76-146">Armazenamento de site utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="7bc76-146">Site Storage Used (Byte)</span></span>
- <span data-ttu-id="7bc76-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="7bc76-147">Report Date</span></span>
- <span data-ttu-id="7bc76-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="7bc76-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7bc76-149">JSON</span><span class="sxs-lookup"><span data-stu-id="7bc76-149">JSON</span></span>

<span data-ttu-id="7bc76-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7bc76-150">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bc76-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7bc76-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7bc76-152">CSV</span><span class="sxs-lookup"><span data-stu-id="7bc76-152">CSV</span></span>

<span data-ttu-id="7bc76-153">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="7bc76-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7bc76-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bc76-154">Request</span></span>

<span data-ttu-id="7bc76-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7bc76-155">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7bc76-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bc76-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitystorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityStorage(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7bc76-157">C#</span><span class="sxs-lookup"><span data-stu-id="7bc76-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitystorage-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bc76-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="7bc76-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitystorage-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7bc76-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7bc76-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitystorage-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7bc76-160">Java</span><span class="sxs-lookup"><span data-stu-id="7bc76-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365groupsactivitystorage-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7bc76-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bc76-161">Response</span></span>

<span data-ttu-id="7bc76-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7bc76-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7bc76-163">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="7bc76-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mailbox Storage Used (Byte),Site Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="7bc76-164">JSON</span><span class="sxs-lookup"><span data-stu-id="7bc76-164">JSON</span></span>

<span data-ttu-id="7bc76-165">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="7bc76-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7bc76-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bc76-166">Request</span></span>

<span data-ttu-id="7bc76-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7bc76-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7bc76-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bc76-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitystorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityStorage(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7bc76-169">C#</span><span class="sxs-lookup"><span data-stu-id="7bc76-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitystorage-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bc76-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="7bc76-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitystorage-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7bc76-171">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7bc76-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitystorage-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7bc76-172">Java</span><span class="sxs-lookup"><span data-stu-id="7bc76-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365groupsactivitystorage-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7bc76-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bc76-173">Response</span></span>

<span data-ttu-id="7bc76-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7bc76-174">The following is an example of the response.</span></span>

> <span data-ttu-id="7bc76-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7bc76-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "mailboxStorageUsedInBytes": 523143237898, 
      "siteStorageUsedInBytes": 31124384, 
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
