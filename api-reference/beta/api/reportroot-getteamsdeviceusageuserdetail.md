---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c3758796e5fd5fa2997019e137211b787d5f005b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868928"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="84dbf-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="84dbf-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84dbf-104">Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="84dbf-104">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="84dbf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="84dbf-105">Permissions</span></span>

<span data-ttu-id="84dbf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84dbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84dbf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84dbf-108">Permission type</span></span>                        | <span data-ttu-id="84dbf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="84dbf-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="84dbf-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84dbf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="84dbf-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="84dbf-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="84dbf-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84dbf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84dbf-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84dbf-113">Not supported.</span></span>                           |
| <span data-ttu-id="84dbf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84dbf-114">Application</span></span>                            | <span data-ttu-id="84dbf-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="84dbf-115">Reports.Read.All</span></span>                         |

<span data-ttu-id="84dbf-116">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="84dbf-116">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="84dbf-117">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="84dbf-117">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="84dbf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84dbf-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="84dbf-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="84dbf-119">Function parameters</span></span>

<span data-ttu-id="84dbf-120">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="84dbf-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="84dbf-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="84dbf-121">Parameter</span></span> | <span data-ttu-id="84dbf-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="84dbf-122">Type</span></span>   | <span data-ttu-id="84dbf-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="84dbf-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="84dbf-124">ponto</span><span class="sxs-lookup"><span data-stu-id="84dbf-124">period</span></span>    | <span data-ttu-id="84dbf-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84dbf-125">string</span></span> | <span data-ttu-id="84dbf-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="84dbf-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="84dbf-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="84dbf-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="84dbf-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="84dbf-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="84dbf-129">data</span><span class="sxs-lookup"><span data-stu-id="84dbf-129">date</span></span>      | <span data-ttu-id="84dbf-130">Data</span><span class="sxs-lookup"><span data-stu-id="84dbf-130">Date</span></span>   | <span data-ttu-id="84dbf-131">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="84dbf-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="84dbf-132">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="84dbf-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="84dbf-133">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="84dbf-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="84dbf-134">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="84dbf-134">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="84dbf-135">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="84dbf-135">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="84dbf-136">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="84dbf-136">The default output type is text/csv.</span></span> <span data-ttu-id="84dbf-137">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="84dbf-137">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84dbf-138">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84dbf-138">Request headers</span></span>

| <span data-ttu-id="84dbf-139">Nome</span><span class="sxs-lookup"><span data-stu-id="84dbf-139">Name</span></span>          | <span data-ttu-id="84dbf-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="84dbf-140">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="84dbf-141">Autorização</span><span class="sxs-lookup"><span data-stu-id="84dbf-141">Authorization</span></span> | <span data-ttu-id="84dbf-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84dbf-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="84dbf-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="84dbf-144">Response</span></span>

### <a name="csv"></a><span data-ttu-id="84dbf-145">CSV</span><span class="sxs-lookup"><span data-stu-id="84dbf-145">CSV</span></span>

<span data-ttu-id="84dbf-146">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="84dbf-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="84dbf-147">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="84dbf-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="84dbf-148">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="84dbf-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="84dbf-149">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="84dbf-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="84dbf-150">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="84dbf-150">Report Refresh Date</span></span>
- <span data-ttu-id="84dbf-151">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="84dbf-151">User Principal Name</span></span>
- <span data-ttu-id="84dbf-152">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="84dbf-152">Last Activity Date</span></span>
- <span data-ttu-id="84dbf-153">Excluído</span><span class="sxs-lookup"><span data-stu-id="84dbf-153">Is Deleted</span></span>
- <span data-ttu-id="84dbf-154">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="84dbf-154">Deleted Date</span></span>
- <span data-ttu-id="84dbf-155">Usou Web</span><span class="sxs-lookup"><span data-stu-id="84dbf-155">Used Web</span></span>
- <span data-ttu-id="84dbf-156">Usou Windows Phone</span><span class="sxs-lookup"><span data-stu-id="84dbf-156">Used Windows Phone</span></span>
- <span data-ttu-id="84dbf-157">Usou iOS</span><span class="sxs-lookup"><span data-stu-id="84dbf-157">Used iOS</span></span>
- <span data-ttu-id="84dbf-158">Usou Mac</span><span class="sxs-lookup"><span data-stu-id="84dbf-158">Used Mac</span></span>
- <span data-ttu-id="84dbf-159">Usou telefone Android</span><span class="sxs-lookup"><span data-stu-id="84dbf-159">Used Android Phone</span></span>
- <span data-ttu-id="84dbf-160">Usou Windows</span><span class="sxs-lookup"><span data-stu-id="84dbf-160">Used Windows</span></span>
- <span data-ttu-id="84dbf-161">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="84dbf-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="84dbf-162">JSON</span><span class="sxs-lookup"><span data-stu-id="84dbf-162">JSON</span></span>

<span data-ttu-id="84dbf-163">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84dbf-163">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="84dbf-164">O tamanho de página padrão para essa solicitação é de 2000 itens.</span><span class="sxs-lookup"><span data-stu-id="84dbf-164">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="84dbf-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84dbf-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="84dbf-166">CSV</span><span class="sxs-lookup"><span data-stu-id="84dbf-166">CSV</span></span>

<span data-ttu-id="84dbf-167">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="84dbf-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="84dbf-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84dbf-168">Request</span></span>

<span data-ttu-id="84dbf-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="84dbf-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="84dbf-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="84dbf-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="84dbf-171">C#</span><span class="sxs-lookup"><span data-stu-id="84dbf-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84dbf-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84dbf-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="84dbf-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84dbf-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="84dbf-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="84dbf-174">Response</span></span>

<span data-ttu-id="84dbf-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="84dbf-175">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="84dbf-176">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="84dbf-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="84dbf-177">JSON</span><span class="sxs-lookup"><span data-stu-id="84dbf-177">JSON</span></span>

<span data-ttu-id="84dbf-178">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="84dbf-178">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="84dbf-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84dbf-179">Request</span></span>

<span data-ttu-id="84dbf-180">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="84dbf-180">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="84dbf-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="84dbf-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="84dbf-182">C#</span><span class="sxs-lookup"><span data-stu-id="84dbf-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84dbf-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84dbf-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="84dbf-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84dbf-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="84dbf-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="84dbf-185">Response</span></span>

<span data-ttu-id="84dbf-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="84dbf-186">The following is an example of the response.</span></span>

> <span data-ttu-id="84dbf-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84dbf-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "usedWeb": false, 
      "usedWindowsPhone": false, 
      "usediOS": true, 
      "usedMac": false, 
      "usedAndroidPhone": false, 
      "usedWindows": true, 
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
