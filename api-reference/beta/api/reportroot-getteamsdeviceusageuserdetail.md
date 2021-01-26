---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: db365af8a666e128dc4047c204de05cab8b8f24f
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982958"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="a3e01-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="a3e01-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

<span data-ttu-id="a3e01-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3e01-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3e01-105">Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="a3e01-105">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3e01-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3e01-106">Permissions</span></span>

<span data-ttu-id="a3e01-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3e01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a3e01-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3e01-109">Permission type</span></span>                        | <span data-ttu-id="a3e01-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3e01-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a3e01-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3e01-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a3e01-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3e01-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a3e01-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3e01-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3e01-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3e01-114">Not supported.</span></span>                           |
| <span data-ttu-id="a3e01-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3e01-115">Application</span></span>                            | <span data-ttu-id="a3e01-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3e01-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="a3e01-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="a3e01-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a3e01-118">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="a3e01-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a3e01-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3e01-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="a3e01-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="a3e01-120">Function parameters</span></span>

<span data-ttu-id="a3e01-121">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a3e01-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="a3e01-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a3e01-122">Parameter</span></span> | <span data-ttu-id="a3e01-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3e01-123">Type</span></span>   | <span data-ttu-id="a3e01-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3e01-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a3e01-125">ponto</span><span class="sxs-lookup"><span data-stu-id="a3e01-125">period</span></span>    | <span data-ttu-id="a3e01-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3e01-126">string</span></span> | <span data-ttu-id="a3e01-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a3e01-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a3e01-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="a3e01-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a3e01-129">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a3e01-129">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="a3e01-130">data</span><span class="sxs-lookup"><span data-stu-id="a3e01-130">date</span></span>      | <span data-ttu-id="a3e01-131">Data</span><span class="sxs-lookup"><span data-stu-id="a3e01-131">Date</span></span>   | <span data-ttu-id="a3e01-132">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="a3e01-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="a3e01-133">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="a3e01-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="a3e01-134">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="a3e01-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="a3e01-135">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="a3e01-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="a3e01-136">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="a3e01-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a3e01-137">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="a3e01-137">The default output type is text/csv.</span></span> <span data-ttu-id="a3e01-138">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta $format OData definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="a3e01-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3e01-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3e01-139">Request headers</span></span>

| <span data-ttu-id="a3e01-140">Nome</span><span class="sxs-lookup"><span data-stu-id="a3e01-140">Name</span></span>          | <span data-ttu-id="a3e01-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3e01-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a3e01-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3e01-142">Authorization</span></span> | <span data-ttu-id="a3e01-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3e01-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a3e01-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3e01-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a3e01-146">CSV</span><span class="sxs-lookup"><span data-stu-id="a3e01-146">CSV</span></span>

<span data-ttu-id="a3e01-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="a3e01-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a3e01-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="a3e01-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a3e01-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a3e01-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a3e01-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="a3e01-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a3e01-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="a3e01-151">Report Refresh Date</span></span>
- <span data-ttu-id="a3e01-152">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="a3e01-152">User Principal Name</span></span>
- <span data-ttu-id="a3e01-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="a3e01-153">Last Activity Date</span></span>
- <span data-ttu-id="a3e01-154">Excluído</span><span class="sxs-lookup"><span data-stu-id="a3e01-154">Is Deleted</span></span>
- <span data-ttu-id="a3e01-155">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="a3e01-155">Deleted Date</span></span>
- <span data-ttu-id="a3e01-156">Usou Web</span><span class="sxs-lookup"><span data-stu-id="a3e01-156">Used Web</span></span>
- <span data-ttu-id="a3e01-157">Usou Windows Phone</span><span class="sxs-lookup"><span data-stu-id="a3e01-157">Used Windows Phone</span></span>
- <span data-ttu-id="a3e01-158">Usou iOS</span><span class="sxs-lookup"><span data-stu-id="a3e01-158">Used iOS</span></span>
- <span data-ttu-id="a3e01-159">Usou Mac</span><span class="sxs-lookup"><span data-stu-id="a3e01-159">Used Mac</span></span>
- <span data-ttu-id="a3e01-160">Usou telefone Android</span><span class="sxs-lookup"><span data-stu-id="a3e01-160">Used Android Phone</span></span>
- <span data-ttu-id="a3e01-161">Usou Windows</span><span class="sxs-lookup"><span data-stu-id="a3e01-161">Used Windows</span></span>
- <span data-ttu-id="a3e01-162">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="a3e01-162">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a3e01-163">JSON</span><span class="sxs-lookup"><span data-stu-id="a3e01-163">JSON</span></span>

<span data-ttu-id="a3e01-164">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3e01-164">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="a3e01-165">O tamanho de página padrão para essa solicitação é de 2000 itens.</span><span class="sxs-lookup"><span data-stu-id="a3e01-165">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="a3e01-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3e01-166">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a3e01-167">CSV</span><span class="sxs-lookup"><span data-stu-id="a3e01-167">CSV</span></span>

<span data-ttu-id="a3e01-168">A seguir está um exemplo que saída CSV.</span><span class="sxs-lookup"><span data-stu-id="a3e01-168">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a3e01-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3e01-169">Request</span></span>

<span data-ttu-id="a3e01-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3e01-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="a3e01-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3e01-171">Response</span></span>

<span data-ttu-id="a3e01-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a3e01-172">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a3e01-173">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="a3e01-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="a3e01-174">JSON</span><span class="sxs-lookup"><span data-stu-id="a3e01-174">JSON</span></span>

<span data-ttu-id="a3e01-175">A seguir está um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="a3e01-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a3e01-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3e01-176">Request</span></span>

<span data-ttu-id="a3e01-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3e01-177">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="a3e01-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3e01-178">Response</span></span>

<span data-ttu-id="a3e01-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a3e01-179">The following is an example of the response.</span></span>

> <span data-ttu-id="a3e01-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3e01-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


